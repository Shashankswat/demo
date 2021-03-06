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
              <li>Integrations and Webhooks</li>
              <li>Documentation and Resources</li>
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
              <li>Understanding Webhooks, API, and apps</li>
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
              <li>Virtual appliance built on Linux</li>
              <li>Distributed as an image</li>
              <li>Fully self-contained, no external dependencies</li>
              <li>Consistent experience from a support perspective</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;MSP Responsibilities</strong></div>
            <ul class="card-text">
            <li>Monitoring the appliance(s)</li>
            <li>Gathering Support Bundles and Diagnostics</li>
            <li>Working with customers to enable/disable users on the appliance</li>
            <li>Enabling/disabling/configuring features on the appliance</li>
            <li>Running reports for customers</li>
            <li>Being the face of Support!</li>
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
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
            <li>Linux based appliance, running a customised Debian Jessie</li>
            <li>Two filesystems: System and Application Data, logically separated</li>
            <li>Variety of internal monitoring systems in place</li>
            <li>Patch releases every 2-4 weeks</li>
            <li>Feature releases every 3-4 months</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
            <li>External monitoring available via SNMP, collectd and Syslog</li>
            <li>Robust backup utilities suite available to backup customer data</li>
            <li>Proxy server support available</li>
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
            <li>Used to manage the GitHub application</li>
            <li>Audit Logging for activity on the appliance</li>
            <li>Run Reports to gather user, org and repository metrics</li>
            <li>Indexing gives view into ElasticSearch search indices</li>
            <li>Manage external applications that access the appliance</li>
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
            <li>Promote/Remove Site Admin users</li>
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
            <li>Used to manage high-level GitHub Enterprise appliance settings</li>
            <li>Managed by MSP</li>
            <li>Management Shell Access for MSP Admins</li>
            <li>Configure DNS/NTP/Auth/SSL/Monitoring</li>
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
  <h1>Diagnostics and Support Bundles</h1>

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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Diagnostics</strong></div>
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
            <li>Reporting on core components</li>
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
            <li>From Management Console Web: http(s)://[hostname]/setup/diagnostics</li>
            <li>From Management Console Shell: 'ghe-diagnostics'</li>
            <li>Can take several minutes to gather and compile</li>
            <li>Great for providing to GitHub for escalation</li>
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
            <li>Often needed when escalating to GitHub or offline analysis</li>
            <li>Investigating polling issues</li>
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
            <li>From Management Console Web: http(s)://[hostname]/setup/support</li>
            <li>From Management Console Shell: 'ghe-support-bundle'</li>
            <li>Can take several minutes to gather and compile</li>
            <li>On large appliances, can be several hundred megs to gigabytes in size</li>
            <li>'ghe-support-bundle -h' for help</li>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;What bundles contain</strong></div>
            <ul class="card-text">
            <li>Metadata and Diagnostics of GHE</li>
            <li>System logs</li>
            <li>Services supporting GHE</li>
            <li>Apps supporting the platform</li>
            <li>Database logging</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Notable Logs</strong></div>
            <ul class="card-text">
            <li>babeld.log</li>
            <li>exceptions.log</li>
            <li>production.log</li>
            <li>gitauth.log</li>
            <li>auth.log</li>
            <li>resque.log</li>
            <li>audit.log</li>
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

  # Deconstructing Diagnostics

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Diagnostics</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;What they contain</strong></div>
            <ul class="card-text">
            <li>Lightweight compared to support bunlde</li>
            <li>Appliance Performance Snapshot</li>
            <li>Licensing information</li>
            <li>Various system/network settings</li>
            <li>Infrastructure settings related to the VM</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
            <ul class="card-text">
            <li>Good for auditing the instance</li>
            <li>See customer utilization</li>
            <li>Audit the license count</li>
            <li>GitHub (L3) may request periodically</li>
            <li>Customer probably won't request</li>
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
  <h1>Integrations+Webhooks, The GitHub API, and custom applications</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Integrations

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Integrations</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Reasons Why</strong></div>
            <ul class="card-text">
            <li>Continous Integration</li>
            <li>Project Management</li>
            <li>ChatOps</li>
            <li>Approval gates</li>
            <li>Accelerate work in IDEs</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Setting up integrations</strong></div>
            <ul class="card-text">
            <li>Simple and straightforward</li>
            <li>Organization vs Repository</li>
            <li>Standardized format for messaging</li>
            <li>Easy to re-trigger messaging</li>
            <li>Easy to setup authentication</li>
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

  # WebHooks

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;WebHooks</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Reasons Why</strong></div>
            <ul class="card-text">
            <li>Trigger on event criteria</li>
            <li>Help enforce quality</li>
            <li>Auditing for large files</li>
            <li>Assist in scanning code after the commit</li>
            <li>Infrastructure automation</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Anatomy</strong></div>
            <ul class="card-text">
            <li>JSON formatted</li>
            <li>Always delivered via HTTP POST</li>
            <li>Split between headers and payload</li>
            <li>Headers "X-GitHub" contain SHA and event type</li>
            <li>Payload mix of git and GitHub data</li>
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

  # The GitHub API

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;The GitHub API</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Ways to access</strong></div>
            <ul class="card-text">
            <li>http(s)://instancename/api/v3/</li>
            <li>cURL for testing</li>
            <li>Libraries in major languages</li>
            <li>Auth at user level</li>
            <li>Tokens allow for scoped access</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Troubleshooting</strong></div>
            <ul class="card-text">
            <li>Always attempt to re-recreate issues</li>
            <li>Sometimes issues are environmental</li>
            <li>Go the extra step for our customers</li>
            <li>Provide sample scripts using octokit.rb</li>
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

  # Applications connecting to GitHub

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Applications</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Applications vs tokenized API</strong></div>
            <ul class="card-text">
            <li>Applications need to be registered</li>
            <li>OAuth2 via web flow/oauth api</li>
            <li>Access private data with user permission</li>
            <li>Preferred over Basic Authentication</li>
            <li>Access can be scoped</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div>
              <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
            </div>
            <ul class="card-text">
            <li>We provide excellent documentation</li>
            <li>Experiment for familiarity</li>
            <li>GitHub Support has your back!</li>
            <li>Please provide customer feedback to us</li>
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

  # OAuth Flow

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>Understanding OAuth Flow </strong></div>
            <ul class="card-text">
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;</strong></div>
           <img src="/images/oauth2_flow.png" height="50%" width="50%">          
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
  <h1>Documentation and Resources</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Documentation and Resources

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Documentation and Resources</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Using GitHub</strong></div>
            <ul class="card-text">
            <li><a href="http://git-scm.com/">Learning git</a></li>
            <li><a href="http://learngitbranching.js.org/">git Branching</a></li>
            <li><a href="https://www.youtube.com/playlist?list=PLg7s6cbtAD16MZFt8waA38gATo5jxcDEp">GitHub Integrations Playlist</a></li>
            <li><a href="https://guides.github.com/introduction/flow/">GitHub Flow</a></li>
            <li><a href="https://guides.github.com/activities/forking/">Introduction to Forking</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Supporting GitHub</strong></div>
            <ul class="card-text">
            <li><a href="https://developer.github.com/v3/">GitHub API Guides</a></li>
            <li><a href="https://enterprise.github.com/support">Contacting Enterprise Support</a></li>
            <li><a href="https://help.github.com/enterprise/2.6/admin/">GitHub Enterprise Admin Guide</a></li>
            <li><a href="https://help.github.com/enterprise/2.6/user/">GitHub Enterprise User Guides</a></li>
            <li><a href="https://help.github.com/enterprise/2.6/admin/guides/user-management/">GitHub Enterprise User Management</a></li>
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
  <h1>Upgrading GitHub Enterprise</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Documentation and Resources

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Upgrading GitHub Enterprise</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
            <ul class="card-text">
            <li>Upgrades typically take 5 to 10 minutes, but can be longer for feature releases</li>
            <li>Longest effort involves backups</li>
            <li>Prioritize security patches over all</li>
            <li>End-user access is not available during upgrade</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Best Practices</strong></div>
            <ul class="card-text">
            <li>Define an outage period</li>
            <li>Perform a backup-utils backup immediately before</li>
            <li>Experiment with new releases in labs</li>
            <li>Stagger upgrades across customer base</li>
            <li>No customer more than 2 major releases behind</li>
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
  <h1>Sustainablility and Best Practices to scale GitHub Support for MSPs</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub's Support Structure

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;GitHub's Support Structure</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Strategic</strong></div>
            <ul class="card-text">
            <li>World Class Support</li>
            <li>Respond + Resolve Quickly</li>
            <li>As few emails as possible</li>
            <li>Bring in help early</li>
            <li>Own customer feedback</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Tactical</strong></div>
            <ul class="card-text">
            <li>Shift-based around the clock support</li>
            <li>Defined urgent/non-urgent response times</li>
            <li>Contribute to release QA</li>         
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

  # Creating a Knowledge Base

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Creating a Knowledge Base</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Customer-Facing</strong></div>
            <ul class="card-text">
            <li>Create a series of how-tos for common issues</li>
            <li>Use your expertise to win our customers</li>
            <li>Reguarly update software release pages</li>
            <li>Update with trends seen for proactive support</li>
            <li>Reach out to our customers</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Internal</strong></div>
            <ul class="card-text">
            <li>Run metrics regularly against issue tracker and each instance</li>
            <li>Create canned replies for customers</li>
            <li>Define escalation paths</li>
            <li>Define support time and handoff</li>
            <li>Keep GitHub Escalation info handy</li>
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

  # Escalating to GitHub Enterprise Support

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Escalating to GitHub Enterprise Support</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>Opening Tickets</strong></div>
            <ul class="card-text">
            <li>Open a new ticket in GitHub Zendesk: https://enterprise.github.com/support</li>
            <li>Describe the issue, and steps taken to reproduce and troubleshoot</li>
            <li>Full error messages and screenshots are useful</li>
            <li>"Urgent" is reserved for production outages</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>Generate/Upload a support bundle</strong></div>
            <ul class="card-text">
            <li>Download Support Bundle from http(s)://[your-hostname]/setup/support</li>
            <li>Upload directly via SSH: <strong>ssh -p 122 admin@hostname -- 'ghe-support-bundle -t ticket-id'</strong></li>
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
