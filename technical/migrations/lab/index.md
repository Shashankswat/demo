---
layout: labs
title: Migrating from SVN to Git
---

# Prepare

### Linux and macOS users:
Make sure you can SSH into your instance using the command `ssh -p 122 -i /<PATH TO YOUR>/keyfile.pem admin@<YOUR HOSTNAME>` in Terminal

### Windows users
Make sure you can issue the Windows equivalent to the above command, or configure your favourite SSH client to be able to connect to:
  - Hostname: `<YOUR HOSTNAME>`
  - Port: `122`
  - User: `admin`
  - Authentication: `Certificate`
  - Certificate Location: `<DRIVE LETTER>:\<PATH TO YOUR>\keyfile.pem`

# Perform the migration
## Create a local copy of the svn repository converted to a git repository.
- As a site admin, SSH into your GitHub Enterprise instance, using the appropriate method for your platfom (Linux, macOS, Windows)
- Create a direcory called `migrations`
    - `mkdir migrations`
- Change the working directory to `migrations`
    - `cd migrations`
- Make a raw clone of the project using the command below, specifying the URL of the source project, and a path to a temporary repository:
    `git-import-svn-raw http://ldap.gitaboard.com:8090/svn/SampleProject notifications.git --user gitaboard --password gitaboard`

## Remap the original users in svn to the users in your GitHub Enterprise instance
- Copy the `raw-authors.csv` file for editing
  - `cp notifications.git/git-import/raw-authors.csv ./authors.csv`
  
<details>
<summary>OLD STUFF</summary>
<p>
- Create a file called `authors.txt`
  - Edit the file and add the following 3 lines
  - `lee.faus = Luke Skywalker <luke@gitaboard.com>`
  - `nicolas.byl = Chewbacca <chewbacca@gitaboard.com>`
  - `matthias.wiesen = Leia <leia@gitaboard.com>`
  - `gitaboard = Han Solo <solo@gitaboard.com>`
  - Save the file
- Create a directory called `notifications`
- Change the working directory to `notifications`
- Perform an SVN migration
  - `svn2git http://ldap.gitaboard.com:8090/svn/SampleProject --authors ../authors.txt --trunk / --nobranches --notags`
- Add a remote to your GitHub Enterprise URL
  - `git remote add origin http://luke@{serverurl}/development/notifications.git`
  - `git push --force --all origin`

## If you are having problems with the self signed certificate
If you are getting a certificate error when trying to perform the above `git push` command, you can disable SSL certificate checking for the `notifications-git` repository only, or for all repositories within your local `git` installation. For this lab we recommend you change only for the `notifications-git` repository:
- Change the working directory to `notifications-git`
- Issue the command `git config http.sslVerify "false"`
- Try the affected `git push` command again.

## If your company requires a proxy to connect to the internet
See the [following StackOverflow discussion](http://stackoverflow.com/questions/15095561/cannot-do-git-svn-fetch-behind-proxy)

</p>
</details>

## Optional/Extra Credit
- Run some `svn` commands in your `git` repositories
 - What happens? Why?

# Validate
- Open a browser to your GitHub Enterprise instance
  - `http://{serverurl}/development/notifications`
  - Click on the dropdown for branches, list out the branches
  - Who are all of the commits listed as in `https://github.com/leefaus/notifications`
  - Who are all of the commits listed as in `http://{serverurl}/development/notifications`
