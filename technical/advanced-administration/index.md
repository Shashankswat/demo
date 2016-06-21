---
layout: slides
title: Advanced Administration
permalink: /technical/advanced-administration/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Advanced Administration</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Advanced Administration

  .container[
  .row[
  .col-md-12[.card[.card-block[.card-text[**Section Goal:**]
  .card-text[Understand Advanced GitHub Enterprise administration topics.]
  ]]]]
  .row[
  .col-md-6[.card[.card-block[**Topics and Agenda**
  .card-text[
  - Backups
  - Restores
  - High Availability
  - Disaster Recovery
  - Clustering]]]]
  .col-md-6[.card[.card-block[**...**
  .card-text[
  - Site Admin Console
  - Command Line Access
  - Upgrades
  - Auditing Usage
  - Creating A Support Pack]]]]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Backups

  .container[
  .row[
  .col-md-12[.card[
  .card-block[
  .card-text[Before you begin using **GitHub Enterprise** in a production capacity, you should set up a backup host, schedule automated backups, and develop a recovery plan as part of an overall [automated backups plan.](https://help.github.com/enterprise/admin/guides/installation/backups-and-disaster-recovery/")]]]]
  .col-md-12[
  ```sh
  git clone https://github.com/github/backup-utils && cd backup-utils
  cp backup.config-example backup.config
  atom backup.config
  bin/ghe-host-check
  bin/ghe-backup
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  ---
  class: title-top

  # Backup Continued

  .container[
  .row[
  .col-md-12[.card[
  .card-block[
  .card-text[
  - Edit `GHE_HOSTNAME`
  - Edit `GHE_DATA_DIR`
  - Add SSH Key for Backup Server
  - Add a `cron` job for backup
  ]]]]
  .col-md-12[
  ```sh
  sudo atom /etc/crontab
  0 * * * * /opt/backup-utils/bin/ghe-backup
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Restoring Data

  .container[
  .row[
  .col-md-12[
  ```sh
  $ ghe-restore 169.154.1.1
  Starting restore of 169.154.1.1 from snapshot 20141111T174152
  Connect 169.154.1.1 OK (v2.0.0)
  Enabling maintenance mode on 169.154.1.1 ...
  Restoring Git repositories ...
  Restoring GitHub Pages ...
  Restoring MySQL database ...
  Restoring Redis database ...
  Restoring SSH authorized keys ...
  Restoring Elasticsearch indices ...
  Restoring SSH host keys ...
  Completed restore of 169.154.1.1 from snapshot 20141111T174152
  Visit https://169.154.1.1/setup/settings to configure the recovered appliance.
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Disaster Recovery

  .container[
  .row[
  .col-md-12[.card[
  .card-block[
  .card-text[
  - [Disaster Recovery](https://help.github.com/enterprise/admin/guides/installation/backups-and-disaster-recovery/#backup-scheduling-and-recovery-point-objective)
  - Edit `GHE_RESTORE_HOST`
  - Add SSH Key for Backup Server
  - Add a `cron` job for backup
  ]]]]
  .col-md-12[
  ```sh
  sudo atom /etc/crontab
  0 */4 * * * /opt/backup-utils/bin/ghe-restore
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # High Availability Overview

  .container[.img-responsive[![high availability](/images/github-ha.png)]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # High Availability Configuration

  .container[
  .row[
  .col-md-12[
  .card[.card-block[.card-text[
  In this [configuration](https://help.github.com/enterprise/admin/guides/installation/high-availability-cluster-configuration/), a fully redundant secondary GitHub Enterprise instance is kept in sync with the primary instance via replication of all major datastores.
  - Fully redundant GitHub Enterprise instance
  - Automated setup of one-way, asynchronous replication of all datastores
  - Active/Passive HA configuration
  - Manual DNS failover

  The replication and failover features included in GitHub Enterprise should **only** be used for:
  - Software crashes
  - Primary system hardware failures
  - Virtualization host system failures
  - Logically or physically severed network at the primary site
  ]]]]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Sample Configuration Steps

  .container[
  .row[
  .col-md-12[
  ```sh
  $ ghe-repl-setup 169.254.1.1
  $ ghe-repl-start
  $ ghe-repl-status
  $ ghe-repl-status -v
  $ ghe-repl-stop
  $ ghe-repl-promote
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Clustering

  .container[
  .row[
  .col-md-12[
  .card[.card-block[.card-text[
  This [configuration](https://help.github.com/enterprise/admin/guides/clustering/initializing-the-cluster/) is only for customers with over 10.000 users.  This requires your sales representative to work with the GitHub Product team to generate a clustering license to be used.
  - Only for companies with > 10.000 developers
  - Get you updated license from GitHub
  - Deploy the appliance a minimum of 3 times
  - Configure the `cluster.conf` on the first node
  - Run the `ghe-cluster-config-init` command to copy the `cluster.conf` to the other nodes
  ]]]]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Site Admin Overview

  .container[.img-responsive[![site admin](/images/site-admin-overview.png)]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Useful Commands

  .container[
  .row[
  .col-md-6[
  .card[.card-block[.card-text[
  Connect via [**SSH**](https://help.github.com/enterprise/admin/guides/installation/administrative-shell-ssh-access/) to perform administrative tasks
  - `ghe-announce` - sets a banner at the top of every GitHub Enterprise page
  - `ghe-maintenance` - put the instance into maintenance mode
  - `ghe-upgrade` - upgrade the appliance
  - `ghe-set-password` - set a new password to log into the Management Console
  - `ghe-storage-extend` - extend the data volume to a larger size
  - `ghe-support-bundle` - prepare a compressed upload of stats of the virtual appliance for support
  - `ghe⇥⇥` - view all commands
  ]]]]
  .col-md-6[
  .card[.card-block[.card-text[
  Not available when **LDAP sync** is _enabled_:
  - `ghe-user-promote`
  - `ghe-user-demote`
  - `ghe-user-suspend`
  - `ghe-user-unsuspend`
  ]]]]
  ]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Upgrading the Appliance

  .container[
  .row[
  .col-md-12[
  .card[.card-block[.card-text[
  GitHub produces fixes every 3 weeks for _z_ releases, every 3 months for _y_ releases and every 18mo-2y for _x_ releases.  In the case of a security vulnerability, we will update the codebase and ask customers to update their appliances immediately.  You will receive this email notification if you are listed as a GitHub appliance administrator in the [GitHub Enterprise Dashboard](https://enterprise.github.com/).  This is also the location you go to for getting the [latest release information and package downloads](https://enterprise.github.com/releases/) for an [upgrade](https://help.github.com/enterprise/2.6/admin/guides/installation/upgrading-the-github-enterprise-virtual-machine/#preparing-to-upgrade).
  ]]]]
  .col-md-12[
  ```sh
  $ cd /tmp
  $ wget \
    https://github-enterprise.s3.amazonaws.com/esx/updates/github-enterprise-esx-2.6.3.pkg
  $ ghe-upgrade github-enterprise-esx-2.6.3.pkg
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Audit Logs

  .container[
  .row[
  .col-md-12[
  .card[.card-block[.card-text[
  GitHub Enterprise keeps logs of audited user, repository, and system events. You can use these logs to debug your installation as well as to comply with internal security mandates and external regulations. A number of user-initiated actions are audited, including:
  - Creating or deleting a repository
  - Creating or deleting an organization
  - Adding or removing an email address
  - Adding or removing an SSH key

  All audited system events, **including all pushes and pulls**, are logged to `/var/log/github/audit.log`  You can also choose to [forward these logs](https://help.github.com/enterprise/admin/articles/log-forwarding/) to a third party system like Splunk or Logstash.
  ]]]]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Getting Support

  .container[
  .row[
  .col-md-12[
  .card[.card-block[.card-text[
  With the purchase of GitHub Enterprise, the customer is entitled to support.  Customers contact GitHub via our [GitHub Enterprise Dashboard](https://support.enterprise.github.com/anonymous_requests/new).  One of the common requests users will get is to generate a support pack.  This is a collection of resources from the appliance that helps us to troubleshoot what problems the appliance the having.  **No repository source code is sent to GitHub in the Support Pack**.
  ]]]]
  .col-md-12[
  ```sh
  $ ghe-support-bundle
  --> Saving support bundle to '/tmp/github-support-bundle-20160621094833.tgz'...
  --> Done.
  ```
  ]]]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

</textarea>
