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
- Create a new directory called `migrations`

# GitHub as an SVN Repository
- Change the working directory to `migrations`
- Create a directory called `notifications-svn`
- Change the working directory to `notifications-svn`
- `svn checkout https://github.com/leefaus/notifications`

# Converting an existing SVN Repository to Git
- Change the working directory to `migrations`
- Create a file called `authors.txt`
  - Edit the file and add a line
  - `lee.faus = Luke Skywalker <luke@gitaboard.com>`
  - `nicolas.byl = Chewbacca <chewbacca@gitaboard.com>`
  - `matthias.wiesen = Leia <leia@gitaboard.com>`
  - Save the file
- Create a directory called `notifications-git`
- Change the working directory to `notifications-git`
- Perform an SVN migration
  - `svn2git https://github.com/leefaus/notifications --authors ../authors.txt`
  - Press `p` to accept the certificate for `github.com`
  - NOTE: There is a [known issue](https://github.com/nirvdrum/svn2git/issues/51) with svn2git in the certificate acceptance process. If the process hangs after typing `p`, continue to hit `p` + `enter` until the process starts.
- Add a remote to your GitHub Enterprise URL
  - `git remote add origin http://luke@{serverurl}/development/notifications.git`
  - `git push --force --all origin`

## If you are having problems with the self signed certificate
If you are getting a certificate error when trying to perform the above `git push` command, you can disable SSL certificate checking for the `notifications-git` repository only, or for all repositories within your local `git` installation. For this lab we recommend you change only for the `notifications-git` repository:
- Change the working directory to `notifications-git`
- Issue the command `git config http.sslVerify "false"`
- Try the affected `git push` command again.


# Validate
- Open a browser to your GitHub Enterprise instance
  - `http://{serverurl}/development/notifications`
  - Click on the dropdown for branches, list out the branches
  - Who are all of the commits listed as in `https://github.com/leefaus/notifications`
  - Who are all of the commits listed as in `http://{serverurl}/development/notifications`
