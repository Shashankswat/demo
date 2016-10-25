---
layout: labs
title: Migrating from SVN to Git
---

# Prepare

- Ruby
  - Mac/Linux - https://github.com/rbenv/rbenv#readme
  - Windows - http://rubyinstaller.org/
  - Need Ruby `2.2.4`
- `gem install svn2git`

**Windows users:** if the `gem` command does not work, it is likely that you do not have the appropriate certificate on your system. 
  This will be evidenced by an error message containng something similar to the following:
  `Gem::RemoteFetcher::FetchError: SSL_connect returned=1 errno=0 state=SSLv3 read server certificate B: certificate verify failed`
This is fixed by:
  - Downloading the cacert.pem file from: http://curl.haxx.se/docs/caextract.html,
  - Placing it an appropriate area on your hard drive
  - Issuing the following command in a command prompt:`SET SSL_CERT_FILE=<PATH TO .pem FILE>`
  - Try the gem command again.
  
For example, with `cacert.pem` downloaded as `C:\Ruby200\cacert.pem`, issue `SET SSL_CERT_FILE=C:\Ruby200\cacert.pem`
See http://help.rubygems.org/discussions/problems/11732-ssl-problems-with-rubygems-on-windows for more information.

- Create a new directory called `migrations`

# Downloading an SVN Repository
- Change the working directory to `migrations`
- Create a directory called `notifications-svn`
- Change the working directory to `notifications-svn`
- `svn checkout http://ldap.gitaboard.com:8090/svn/SampleProject --username gitaboard` (Password same as username)

# Converting an SVN Repository to Git
- Change the working directory to `migrations`
- Create a file called `authors.txt`
  - Edit the file and add the following 3 lines
  - `lee.faus = Luke Skywalker <luke@gitaboard.com>`
  - `nicolas.byl = Chewbacca <chewbacca@gitaboard.com>`
  - `matthias.wiesen = Leia <leia@gitaboard.com>`
  - Save the file
- Create a directory called `notifications`
- Change the working directory to `notifications`
- Perform an SVN migration
  - `svn2git http://ldap.gitaboard.com:8090/svn/SampleProject --authors ../authors.txt --rootistrunk --username gitaboard`
- Add a remote to your GitHub Enterprise URL
  - `git remote add origin http://luke@{serverurl}/development/notifications.git`
  - `git push --force --all origin`

## If you are having problems with the self signed certificate
If you are getting a certificate error when trying to perform the above `git push` command, you can disable SSL certificate checking for the `notifications-git` repository only, or for all repositories within your local `git` installation. For this lab we recommend you change only for the `notifications-git` repository:
- Change the working directory to `notifications-git`
- Issue the command `git config http.sslVerify "false"`
- Try the affected `git push` command again.

## Optional/Extra Credit
- Run some `svn` commands in your `git` repositories
 - What happens? Why?

# Validate
- Open a browser to your GitHub Enterprise instance
  - `http://{serverurl}/development/notifications`
  - Click on the dropdown for branches, list out the branches
  - Who are all of the commits listed as in `https://github.com/leefaus/notifications`
  - Who are all of the commits listed as in `http://{serverurl}/development/notifications`
