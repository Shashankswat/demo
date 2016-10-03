---
layout: labs
title: Installation and Setup Lab
---

# Installation and Setup

## Prerequisites
- Make sure you have a GitHub.com User ID
- Ensure you GitHub.com User ID is added to the [Partners Enablement Repository](https://github.com/githubpartners/enablement)
- Download the [GitHub Enterprise License](https://github-partner-enablement.herokuapp.com/license/github-enterprise.ghl)

## Provisioning Your AWS Instance
- [Directions](https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-aws/#requirements)
- Provision an `r3.large` instance
- Choose the [AMI ID](https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-aws/#selecting-the-github-enterprise-ami) closest to your location
- Make sure you add the Secondary EBS Volume (10G)
- Add the corresponding [Security Group](https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-aws/#creating-a-security-group)
- Download your `***.pem` file to you `${home_directory}/.ssh` folder **don't lose this**
- Access `https://{hostname}/setup` from your browser

## Basic Configuration
- Create a password
- Upload the license file

# Adding Users and Teams with LDAP/SYNC

## LDAP Settings
- `host` - `ldap.gitaboard.com`
- `port` - `389`
- `domain search user` - `cn=admin,dc=gitaboard,dc=com`
- `domain search password` - `G1t@B0@rd`
- `administrators group` - `site-admins`
- `domain base`:
  - `o=engineering,dc=gitaboard,dc=com`
  - `o=operations,dc=gitaboard,dc=com`

## Setting Up LDAP
- [LDAP Configuration](https://help.github.com/enterprise/admin/guides/user-management/using-ldap/)

## Additional Settings
- [Basic Configuration](https://help.github.com/enterprise/admin/guides/installation/basic-configuration/)
- Check `Synchronization`
- Check `Synchronize Emails`
- Check `Enable Pages`
- Check `Public Pages`
- Login to appliance `http://{hostname}/login`
  - Username - `chewbacca`
  - Password - `P@ssw0rd`

## Extra Credit
- Create a github pages site for your personal account
- Create a github pages site for project in your personal account
