---
layout: labs
title: End User Administration
---

# Pre-reqs
- Site Admin Credentials
  - sign in - `chewbacca`
  - password - `P@ssw0rd`

# Creating Organizations
- [Create a new organization](https://help.github.com/enterprise/user/articles/creating-a-new-organization-account/)
- Call this organization `development`

# Adding Teams
- [Create a new team](https://help.github.com/enterprise/user/articles/setting-up-teams/)
- Call this team `ruby developers`
- Use this LDAP Path `cn=ruby-experts,ou=developers,o=engineering,dc=gitaboard,dc=com`

- [Import a Team](https://help.github.com/enterprise/user/articles/setting-up-teams)
- Click import team
- In the search box, type `team`
- Click on `team-leads`, then press the `Import` button

# Add an individual contributor
- Sign out, if you are currently signed in as `chewbacca`
- Sign in as `solo`, password `P@ssw0rd`
- Account is now synced, sign out as `solo`
- Log in as `chewbacca`
  - In the dropdown, choose `development`
  - Click the botton on the right that says `view development`
  - Click the `People` tab
  - Click on the `Add Member` button
  - Enter `solo` in the `Search by username` search box, click on the `Han Solo` drop down
  - Add `solo` as a member

# Additional Tasks
- Create another organziation called operations
- Add the team `ansible-experts`

# Creating Repositories
- [Create a new repository](https://help.github.com/enterprise/user/articles/create-a-repo/) in `development`
- Call this repository `notifications`
- Mark this repository as `Private`
- Initialize the repository with a README
- Click Create Repository
- Add the `ruby-developers` team to the repository
  - Click on the `Settings` tab
  - Click on the `Collaborators and teams` tab
  - In the drop down, choose the `ruby developers` team
  - Give the `ruby developers` write access to the repository
  - Add the user `leia` as an `outside collaborator`

# Testing Access
- Sign out as `chewbacca`
- Sign in as `leia`
  - Go to the `development` organization
  - What repositories does `leia` have access to? why?

# Changing Default Permissions
- Sign out as `leia`
- Sign in as `chewbacca`
- Click on the `Settings` tab for the `development` organization
- Click on the `Member privileges` tab on the left
  - Uncheck the `Allow members to create repositories ...`
  - Make the default repository permissions `None`
- Sign out as `chewbacca`
- Sign in as `leia`
  - Go to the `development` organization
  - What repositories does `leia` have access to?  why?

# Explicit Access to Repositories
- Sign out as `leia`
- Sign in as `chewbacca`
- Click on the `Settings` for the `notifications` repository
- Click on the `Collaborators and teams` tab on the left
- In the `Collaborators` box at the bottom, type `leia`
- Change from `write` to `Read` in the drop-down box
- Make sure the team `ruby-developers` has `Write` permissions
- Verify `leia` now has access to the repository
- Verify `leia` only has read access to the repository
- What happens if `leia` tries to edit the `README`?

# Extra Credit
- Create a public repository
- What is the difference between a public and private repository?
- Why would a company create one over the other?
