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

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Section Goal:</strong></div>
            <div class="card-text">Understand Advanced GitHub Enterprise administration topics.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Topics and Agenda:</strong></div>
            <ul class="card-text">
              <li>Publish logs</li>
              <li>Search auditing for users actions</li>
              <li>Suspend users</li>
              <li>User impersonation</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Topics and Agenda:</strong></div>
            <ul class="card-text">
              <li>Validate git-lfs</li>
              <li>Access audit logging via API</li>
              <li>Enable GitHub replication</li>
              <li>GitHub backup and DR</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Useful Commands

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Connect to <a href="https://help.github.com/enterprise/admin/guides/installation/administrative-shell-ssh-access/" target="_blank">SSH</a> using port 122:</strong></div>
            <ul class="card-text">
              <li><code>ghe-announce</code> - sets a banner at the top of every GitHub Enterprise page</li>
              <li><code>ghe-maintenance</code> - put the instance into maintenance mode</li>
              <li><code>ghe-user-csv</code> - dumps a list of all the users in the installation in CSV format</li>
              <li><code>ghe-system-info</code> - responds with JSON of instance health stats</li>
              <li><code>ghe-license-info</code> - responds with JSON of of the currently installed license</li>
              <li><code>ghe-set-password</code> - set a new password to log into the Management Console</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Not available when LDAP sync is enabled:</strong></div>
            <ul class="card-text">
              <li><code>ghe-user-promote</code></li>
              <li><code>ghe-user-demote</code></li>
              <li><code>ghe-user-suspend</code></li>
              <li><code>ghe-user-unsuspend</code></li>
              <li><code>ghe⇥⇥</code> - view all commands</li></br>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Audit Logs

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">GitHub Enterprise keeps logs of audited user, repository, and system events. You can use these logs to debug your installation as well as to comply with internal security mandates and external regulations. A number of user-initiated actions are audited, including:</div>
            <ul class="card-text">
              <li>creating or deleting a repository</li>
              <li>creating or deleting an organization</li>
              <li>adding or removing an email address</li>
              <li>adding or removing an SSH key</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">All audited system events—including all pushes and pulls—are logged to <code>/var/log/github/audit.log</code>.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">All audit information is logged to the <code>audit.log</code> file in the <code>github-logs</code> directory of any <a href="https://help.github.com/enterprise/admin/guides/installation/troubleshooting/#support-bundle" target="_blank">Support Bundle</a>. If <a href="https://help.github.com/enterprise/admin/articles/log-forwarding/" target="_blank">log forwarding</a> is enabled, you can stream this data to an external syslog stream consumer such as Splunk or logstash. All entries from this log use the "github_audit" keyword and can be filtered using that.</div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Suspending Users

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">You can <a href="https://help.github.com/enterprise/admin/guides/installation/troubleshooting/#support-bundle" target="_blank">suspend</a> users GitHub Enterprise accounts to open up seats in your site license while preserving the issues, comments, repositories, gists, and other data they created. Suspended users cannot sign into your instance, nor can they push or pull code.  When you suspend a user, the change takes effect immediately with no notification to the user. <strong>If the user attempts to pull or push to a repository, they'll receive this error:</strong></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">
              <div class="card-text"><code>
                $ git clone git@[hostname]:john-doe/test-repo.git</br>
                Cloning into 'test-repo'...</br>
                ERROR: Your account is suspended. Please check with your installation administrator.</br>
                fatal: The remote end hung up unexpectedly</br></code></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # High Availability Cluster Configuration

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">In this <a href="https://help.github.com/enterprise/admin/guides/installation/high-availability-cluster-configuration/" target="_blank">configuration</a>, a fully redundant secondary GitHub Enterprise instance is kept in sync with the primary instance via replication of all major datastores.</div>
            <ul class="card-text">
              <li>Fully redundant GitHub Enterprise instance</li>
              <li>Automated setup of one-way, asynchronous replication of all datastores</li>
              <li>Active/Passive cluster configuration</li>
              <li>DNS failover</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">The replication and failover features included in GitHub Enterprise 2.4 should <strong>only</strong> be used for:</div>
            <ul class="card-text">
              <li>Software crashes</li>
              <li>Primary system hardware failures</li>
              <li>Virtualization host system failures</li>
              <li>Logically or physically severed network at the primary site</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Backups

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Before you begin using GitHub Enterprise in a production capacity, you should set up a backup host, schedule automated backups, and develop a recovery plan as part of an overall <a href="https://help.github.com/enterprise/admin/guides/installation/backups-and-disaster-recovery/" target="_blank">automated backups plan.</a></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
              <li>Download the latest <a href="https://help.github.com/enterprise/admin/guides/installation/backups-and-disaster-recovery/" target="_blank">github/backup-utils</a> release and extract on the backup host</li>
              <li>Copy the included <code>backup.config-example</code> file to <code>backup.config</code> and open in an editor</li>
              <li>Set the <code>GHE_HOSTNAME</code> value and the <code>GHE_DATA_DIR</code> value</li>
              <li>Open <code>https://[hostname]/setup/settings</code> and add the backup host's SSH key</li>
              <li>Run <code>bin/ghe-host-check</code> to verify SSH connectivity</li>
              <li>Run <code>bin/ghe-backup</code> to perform an initial full backup</li>
              <li>Schedule regular backups on the host using <code>cron(8)</code> or similar</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Disaster Recovery

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">In the event of prolonged outage or catastrophic event at the primary site, basic operations of your GitHub Enterprise environment can be <a href="https://help.github.com/enterprise/admin/guides/installation/backups-and-disaster-recovery/#backup-scheduling-and-recovery-point-objective" target="_blank">restored</a> by performing a restore from the backup host.</div>
            <code>
              $ ghe-restore 169.154.1.1</br>
              Starting restore of 169.154.1.1 from snapshot 20141111T174152</br>
              Connect 169.154.1.1 OK (v2.0.0)</br>
              Enabling maintenance mode on 169.154.1.1 ...</br>
              Restoring Git repositories ...</br>
              Restoring GitHub Pages ...</br>
              Restoring MySQL database ...</br>
              Restoring Redis database ...</br>
              Restoring SSH authorized keys ...</br>
              Restoring Elasticsearch indices ...</br>
              Restoring SSH host keys ...</br>
              Completed restore of 169.154.1.1 from snapshot 20141111T174152</br>
              Visit https://169.154.1.1/setup/settings to configure the recovered appliance.
            </code>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>