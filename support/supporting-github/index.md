---
layout: slides
title: Supporting GitHub Enterprise
permalink: /support/supporting-github/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Supporting GitHub Enterprise</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  #Supporting GitHub Enterprise

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Support Agenda:</strong></div>
            <ul class="card-text">
              <li>GitHub Enterprise Appliance</li>
              <li>Site Admins</li>
              <li>Gathering Support Bundles and Diagnostics</li>
              <li>Integrations and WebHooks</li>
              <li>Documentation</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Support Agenda - Deep Dive:</strong></div>
            <ul class="card-text">
              <li>GitHub Enterprise Appliance Deep-Dive</li>
              <li>Management Console</li>
              <li>Reading Support Bundles and Diagnostics</li>
              <li>Understanding webhooks, API, and applications</li>
              <li>Upgrading GitHub Enterprise</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Sustainable Support and Best Practices</strong></div>
            <ul class="card-text">
              <li>GitHub's Support Structure</li>
              <li>Creating a Knowledge Base</li>
              <li>Escalating tickets and issues</li>
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>The GitHub Appliance</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Appliance

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;The GitHub Appliance</strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About</strong></div>
            <ul class="card-text">
              <li>Virtual image built on Linux delivered as a single appliance</li>
              <li>All necessary services and processes all held within</li>
              <li>Consistent experience from support perspective</li>
              <li>Maintenance of customer appliances supported by IBM DevOps Team</li>
              <li>Current release (May 2016) Enterprise 2.6</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;L1 Responsibilities</strong></div>
            <ul class="card-text">
            <li>Monitoring the appliance(s)</li>
            <li>Gathering Support Bundles and Diangnostics</li> 
            <li>Working with customers to enabling/disabling users on the appliance</li>
            <li>Enabling/disabling features on the appliance</li>
            <li>Running reports for our customers</li>
            <li>Being the face of GitHub at IBM!</li>
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

  # GitHub Enterprise Appliance - Deep Dive

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Appliance Deep Dive</strong></div>
            <ul class="card-text">
            <li>Note: Information up-to-date as of May 2016</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Appliance Deep Dive</strong></div>
            <ul class="card-text">
            <li>Server based on Ubuntu Server 12.04 LTS</li>
            <li>Two filesystems: User and Application, logically separated</li>
            <li>Variety of internal monitoring systems in place to feed external SNMP monitoring</li>
            <li>GitHub Enterprise is patched and updated regularly, pro-active</li>
            <li>Major releases every 3-4 months</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Appliance Deep Dive</strong></div>
            <ul class="card-text">
            <li>A variety of TCP/UDP protocols</li>
            <li>Monitoring set up via SNMP (+collectd)</li>
            <li>GitLFS natively supported (Encourage customers to enable this when onboarding!)</li>
            <li>Robust backup-utilities available to backup customer data</li>
            <li>Proxy server support available (Useful if customer is VIP'ing to Bluemix)</li>
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Site Admin and Management Console</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Site Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Site Admin</strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Features</strong></div>
            <ul class="card-text">
            <li>Used to manage the GitHub Enterprise installation</li>
            <li>Audit Logging for activity on the instance </li>
            <li>Run Reports to gather user, org and repository metrics</li>
            <li>Indexing gives view into ElasticSearch internal custer</li>
            <li>Manage custom applications that access the instance</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Features</strong></div>
            <ul class="card-text">
            <li>File Storage - See usage, and GitLFS store</li>
            <li>Admin Center - Manage global settings</li>
            <li>Manage/Invite/Suspend Users</li>
            <li>Promote/Remove users at Site Admins</li>
            <li>Enterprise Admin API exposes some of these features</li>
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

  # Site Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Management Console</strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Features</strong></div>
            <ul class="card-text">
            <li>Used to manage high-level GitHub Enterprise Settings</li>
            <li>Commonly referred to as 'Staff Tools'</li>
            <li>Manage Shell Access for Admins</li>
            <li>Configure DNS/NTP/IdP</li>
            <li>Check for Updates</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Features</strong></div>
            <ul class="card-text">
            <li>Monitoring Dashboard</li>
            <li>Maintenance Mode</li>
            <li>GitHub Pages Accessibility</li>
            <li>Subdomain Isolation</li>
            <li>Enable log/collectd forwarding</li>
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Support Bundles and Diagnostics</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Support Bundles

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Support Bundles</strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Use Cases</strong></div>
            <ul class="card-text">
            <li>Key for troubleshooting the appliance</li>
            <li>Sometimes user's issues will be system based</li>
            <li>Will need when escalating to L2/GitHub</li>
            <li>Useful to become comfortable with core components</li>
            <li>Helpful to share with customer</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;How to Gather</strong></div>
            <ul class="card-text">
            <li>Two ways</li>
            <li>From Staff Tools -> Support</li>
            <li>From command line: 'ghe-support-bundle'</li>
            <li>Can take several minutes to gather and compile</li>
            <li>On large appliances, can be several hundred megs in size</li>
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

  # Diagnostics

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Support Bundles</strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Use Cases</strong></div>
            <ul class="card-text">
            <li>Key for troubleshooting the appliance</li>
            <li>Finding performance issues</li>
            <li>Determining webhook/polling issues</li>
            <li>Report on core components</li>
            <li>Logfile size reporting</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;How to Gather</strong></div>
            <ul class="card-text">
            <li>Two ways</li>
            <li>http(s)://(INSTANCENAME)/setup/diagnostics</li>
            <li>From command line: 'ghe-diagnostics'</li>
            <li>Can take several minutes to gather and compile</li>
            <li>Great for providing to L2/GitHub for escalation</li>
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Reading Support Bundles and Diagnostics</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Deconstructing Support Bundles

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Support Bundles</strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Use Cases</strong></div>
            <ul class="card-text">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;How to Gather</strong></div>
            <ul class="card-text">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

    <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
    </footer>
   <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
   </footer>
</textarea>
