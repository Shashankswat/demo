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
              <li>Understanding webhooks, API, and apps</li>
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
            <li>GitLFS optionally supported</li>
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
            <li>Managed by IBM Bluemix Support</li>
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
            <li>Determining webhook/polling issues</li>
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
            <li>L1 handles a lot of API support</li>
            <li>Always attempt to re-recreate</li>
            <li>Sometimes issues are environmental</li>
            <li>Go the extra step for our customers</li>
            <li>You may receive customer feedback. Yay!</li>
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
            <li>OAuth2 via web flow/oauth api (Preview mode)</li>
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
            <li>Sizable portion of L1 Support</li>
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
            <li><a href="https://github.zendesk.com/">ZenDesk (Contacting us)</a></li>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Consideratiosn</strong></div>
            <ul class="card-text">
            <li>Upgrades typically take minutes</li>
            <li>Longest effort involves backups</li>
            <li>Check for upgrades in Management Console</li>
            <li>Prioritize security patches over all</li>
            <li>Customer has no access during upgrade</li>
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
            <li>Encourage customers to run backup-utils</li>
            <li>Experiment with major releases in labs</li>
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
            <li>3 Levels of Support</li>            
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

  # Escalation Paths internally and to GitHub

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Escalation</strong></div>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;L1 -> L2</strong></div>
            <ul class="card-text">
            <li>Customer cannot resolve</li>
            <li>Documentation cannot resolve</li>
            <li>Is actively preventing development</li>
            <li>Appliance setting may need change</li>
            <li>Infrastructure work needed</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;L2 -> GitHub</strong></div>
            <ul class="card-text">
            <li>Typically code related</li>
            <li>Issue internal to appliance</li>
            <li>Infrastructure ruled out</li>
            <li>Can not resolve within reasonable time</li>
            <li>Always provide Support Bundles!</li>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Escalation</strong></div>
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
            <li>Open a new ticket in GitHub ZenDesk https://git.io/voaUg</li>
            <li>Describe the issue, and steps taken to reproduce and troubleshoot</li>
            <li>Full error messages and screenshots are useful</li>
            <li>"Urgent" is reserved for production outages.</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>Generate a support bundle</strong></div>
            <ul class="card-text">
            <li>Download Support Bundle from http(s)://[your-hostname]/setup/support</li>
            <li>Upload bundle to https://git.io/voaUK using the new ticket number</li>
            <li>Alternatively, upload directly via SSH: <strong>ghe-support-bundle  -t ticket#</strong></li>
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
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>Opening Tickets with Enterprise Support</strong></div>
            <ul class="card-text">
            <li>Open a new ticket in GitHub Enterprise Support Portal: https://git.io/voaUgt</li>
            <li>Describe the issue, and steps taken to troubleshoot</li>
            <li>Full error messages and screenshots</li>
            <li>"Urgent" is reserved for production outages.</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>Upload a support bundle</strong></div>
            <ul class="card-text">
            <li>Download Support Bundle from http(s)://[hostname]/setup/suppor</li>
            <li>Using your ticket number, upload bundle to https://git.io/voaUK</li>
            <li>Alternatively, upload directly via command line: ghe-support-bundle  -t ticket#</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
   </footer>    
</textarea>
