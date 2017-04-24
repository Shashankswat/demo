---
layout: labs
title: Migrating from SVN to Git
---

# Prepare

### Linux and macOS users:
Make sure you can SSH into your instance using the command `ssh -p 122 -i /{PATH TO YOUR}/keyfile.pem admin@{serverurl}` in Terminal

### Windows users
Make sure you can issue the Windows equivalent to the above command, or configure your favourite SSH client to be able to connect to:
  - Hostname: `{serverurl}`
  - Port: `122`
  - User: `admin`
  - Authentication: `Certificate`
  - Certificate Location: `<DRIVE LETTER>:\<PATH TO YOUR>\keyfile.pem`

#### Note - you should have already tested the above in an earlier lab.

# Perform the migration
## Create a 'local' copy of the svn repository converted to a git repository, on your GitHub Enterrpise instance.
- As a site admin, SSH into your GitHub Enterprise instance, using the appropriate method for your platfom (Linux, macOS, Windows)
- In the directory you are now in on your GitHub Enterprise instance, create a directory called `migrations`
    - `mkdir migrations`
- Change the working directory to `migrations`
    - `cd migrations`
- Make a raw clone of the project using the command below, specifying the URL of the source project, and a path to a temporary repository:
  - `git-import-svn-raw http://ldap.gitaboard.com:8090/svn/SampleProject notifications.git --user gitaboard --password gitaboard`

## Remap the original users in svn to the users in your GitHub Enterprise instance
- Look at the `raw-authors.csv` file
  - `less notifications.git/git-import/raw-authors.csv`
    - You can see that there is a line for each commit and it will list the `ID` and the `NAME`. In this repository all commits are made by the same person: `gitaboard@4b8cc709-3b1e-4a39-9d75-0916ae99683d,gitaboard`
 
 - To map authors from the original repository to an email address and name of a user in GitHub Enterprise.
   - create a new CSV file with the columns `ID`,`(ignored)`,`GIT_EMAIL`,`GIT_NAME`, which replaces the author information for anything by `ID` with `GIT_EMAIL` and `GIT_NAME`.
     - call the file `authors.csv`
     - add the following line:
   `gitaboard@4b8cc709-3b1e-4a39-9d75-0916ae99683d,gitaboard,solo@gitaboard.com,Han Solo`
    - Save the file
  - Rewrite the authors and branches using the CSV file:
    - `git-import-rewrite --flavor svn --authors authors.csv notifications.git`
  - Change the working directory to `notifications.git`
    - `cd notifications.git`
  - Add a remote to your GitHub Enterprise URL
    - `git remote add origin http://{serverurl}/development/notifications.git`
    - `git push --force --all origin` 
    - use the username `chewbacca` with password `P@ssw0rd`
 
 ## If you are having problems with the self signed certificate
If you are getting a certificate error when trying to perform the above `git push` command, you can disable SSL certificate checking for the `notifications.git` repository. For this lab we recommend you change only for the `notifications.git` repository:
  - Make sure you are in the `notifications.git` directory
  - Issue the command `git config http.sslVerify "false"`
  - Try the affected `git push` command again.

## Finishing up
- delete the migrations directory:
  - `cd ~`
  - `rm -rf migrations`
- sign out of your SSH session
- make a copy of the notifications repository on your local drive
  - change to the directory you want the local repository to be stored in
  - issue the command:
    - `git clone https://{serverurl}/development/notifications.git`

## Optional/Extra Credit
- Run some `svn` commands in your local `git` repositories
 - What happens? Why?

# Validate
- Open a browser to your GitHub Enterprise instance
  - `http://{serverurl}/development/notifications`
  - Click on the dropdown for branches, list out the branches
  - Who are all of the commits listed as in `https://github.com/leefaus/notifications`
  - Who are all of the commits listed as in `http://{serverurl}/development/notifications`
