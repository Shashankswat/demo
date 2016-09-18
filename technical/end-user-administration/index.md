---
layout: slides
title: End User Administration
permalink: /technical/end-user-administration/
---


<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>End User Administration</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # End User Administration

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Section Goal:</strong></div>
            <div class="card-text">Administration of GitHub Enterprise.</div>
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
              <li>Create an Organization</li>
              <li>Create a Team</li>
              <li>Create a Repository</li>
              <li>Secure a Repository</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Topics and Agenda:</strong></div>
            <ul class="card-text">
              <li>Notifications and @ Mentions</li>
              <li>Git Large File Storage</li>
              <li>Benefits of git-lfs</li>
              <li>Enable git-lfs</li>
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

  # Create an Organization

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card-block">
          <div class="card-text">An <a href="https://help.github.com/enterprise/admin/guides/user-management/creating-organizations/" target="_blank">organization</a> is a collection of user accounts that owns repositories. To create an organization: </div></br>
          <ul class="card-text">
            <li>click your profile photo > 'Settings'</li>
            <li>settings sidebar, click 'Organizations'</li>
            <li>Organizations, click 'New organization'</li>
            <li>give the organization a name</li>
            <li>Enter the contact email</li>
            <li>Click 'Create organization'</li>
          </ul>
        </div>
      </div>
      <div class="col-md-6">
        <img src="/images/ACCOUNT-Settings.png" class="img-resize"></br>
        <img src="/images/SETTINGS-ORg.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Organization Settings

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">As a Site Admin, you have a high level overview of the repository</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-org-settings.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Organization Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">The Org Admins screen provides various functionality</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-org-admin-1.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Organization Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Scope things such as GitLFS and Git SSH on a per-org basis</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-org-admin-2.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Organization Users and Teams

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Manage users and teams in the Organization Admin Screen</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-org-users-and-teams.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Thinking about Organizations
  <div class="container">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">What and Why Orgs?</h4>
          <ul class="card-text">
            <li>A collection of user accounts that own repositories</li>
            <li>Logically silo users at business-unit level, or team leve</li>
            <li>Helps manage the collaboration within the scope of an org</li>
            <li>Can use org-level webhooks</li> 
          </ul>
        </div>
      </div>
        <div class="card">
        <div class="card-block">
          <h4 class="card-title">Ideas for Organization Creation</h4>
          <ul class="card-text">
            <li>Allow users to create organizations</li>
            <li>Orgs are relatively silo'd - No @mentions</li>
            <li>Decide early how Orgs are to be created</li>
            <li>By Application group? By technology? By department?</li>
            <li>Best of both worlds: Allow users to create orgs, but have defined orgs</li>
            <li>User accounts can be converted to orgs</li>
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

  # Create a Team

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card-block">
          <div class="card-text"><a href="https://help.github.com/enterprise/admin/guides/user-management/creating-teams/" target="_blank">Teams</a> give organizations the ability to create groups of members and control access to repositories. Team members can be granted read, write, or admin permissions to specific repositories. To create a team: </div></br>
          <ul class="card-text">
            <li>click your profile photo > 'Your profile'</li>
            <li>Organizations, click your org icon</li>
            <li>click 'Teams' under your org</li>
            <li>click 'New team'</li>
            <li>decide if it will be 'Visible'</li>
            <li>click 'Create team'</li>
          </ul>
        </div>
      </div>
      <div class="col-md-6">
        </br>
        <img src="/images/ORG-Teams.png" class="img-resize"></br>
        <img src="/images/TEAM-New.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Team Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Have a high level overview of members of teams</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-team-admin.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Team Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Easy access to your team from the org homepage</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-team-tab.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Team Homepage

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">A team page, in action</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-team-page.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  ---
  class: title-top

  # Create a Repository

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card-block">
          <div class="card-text">You can <a href="https://help.github.com/enterprise/user/articles/creating-a-new-repository/" target="_blank">create a new repository</a> on your personal account or any organization where you have sufficient permissions. To create a repository: </div></br>
          <ul class="card-text">
            <li>click <span class="octicon octicon-plus" aria-label="Plus symbol " title="Plus symbol "></span> > 'New repository'</li>
            <li>select the account</li>
            <li>type a name</li>
            <li>choose Public or Private</li>
            <li>click 'Create repository'</li>
          </ul>
        </div>
      </div>
      <div class="col-md-6">
        </br>
        <img src="/images/REPO-Create.png" class="img-resize"></br>
        <img src="/images/REPO-Name.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Securing a Repository
  <div class="container">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Reasons to Secure a Repository</h4>
          <ul class="card-text">
            <li>Protect your code</li>
            <li>Prevent bad code being introduced</li>
            <li>Disable history-destroying force pushes and merges</li>
            <li>Helps new employees feel empowered to experiment</li>
            <li>Prevent IP/API keys from being stored in code</li>
          </ul>
        </div>
      </div>
        <div class="card">
        <div class="card-block">
          <h4 class="card-title">Methods to Secure a Repository</h4>
          <ul class="card-text">
            <li>Protected Branches</li>
            <li>Required Statuses</li>
            <li>Branch Permissions</li>
            <li>GPG Signed Commits</li>
            <li>Outside Collaborators</li>
            <li>Pre-Receive Hooks</li>
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

  # Notification Emails

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
          <div class="card-text">You can choose to receive <a href="https://help.github.com/articles/configuring-notification-emails/" target="_blank">notification emails</a> about changes made to any repository, issue, or pull request that you have access to.  GitHub sends multipart emails, which contain both HTML and plain text copies of the email content.  We'll automatically format Markdown, @mentions, emojis, hash-links, and more: </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/NOTIFICATION_Emails.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Git Large File Storage

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
          <div class="card-text"><strong>An open source Git extension for versioning large files</strong></div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
          <div class="card-text"><a href="https://git-lfs.github.com/" target="_blank">Git Large File Storage (LFS)</a> replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise. </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GIT-LFS-Overview.gif" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Git LFS Features

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
          <h4><span class="octicon octicon-file-binary"></span> Large file versioning:</h4>
            <ul class="card-text"><li>Version large files—even those as large as a couple GB in size—with Git.</li></ul>
          <h4><span class="octicon octicon-repo"></span> More repository space:</h4>
            <ul class="card-text"><li>Host more in your Git repositories. External file storage makes it easy to keep your repository at a manageable size.</li></ul>
          <h4><span class="octicon octicon-cloud-download"></span> Faster cloning and fetching:</h4>
            <ul class="card-text"><li>Download less data. This means faster cloning and fetching from repositories that deal with large files.</li></ul>
          <h4><span class="octicon octicon-git-branch"></span> Same Git workflow:</h4>
            <ul class="card-text"><li>Work like you always do on Git—no need for additional commands, secondary storage systems, or toolsets.</li></ul>
          <h4><span class="octicon octicon-lock"></span> Same access controls and permissions:</h4>
            <ul class="card-text"><li>Keep the same access controls and permissions for large files as the rest of your Git repository when working with a remote host like GitHub.</li></ul>
        </div>
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Configure Git Large File Storage

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card-block">
          <div class="card-text">You can enable or disable <a href="https://help.github.com/enterprise/admin/articles/configuring-git-large-file-storage-for-a-repository/" target="_blank">Git LFS</a> on a per-repository or organization basis: </div></br>
          <b>For an Organzation:</b>
          <ul class="card-text">
            <li>As a site admin, sign in to your GitHub Enterprise instance at <code>http(s)://[hostname]/login</code></li>
            <li>In the upper-right corner of any page, click <span class="octicon octicon-rocket" aria-label="The rocket ship " title="The rocket ship "></span></li>
            <li>Click on <code>Organizations</code> in the left sidebar and click the link to your org</li>
            <li>In the left sidebar, click <code>Admin</code></li>
            <li>Toggle the <code>disable</code> button</li>
          </ul>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card-block">
          <div class="card-text"></div><br><br><br>
          <b>For a Repository:</b>
          <ul class="card-text">
            <li>As a site admin, sign in to your GitHub Enterprise instance at <code>http(s)://[hostname]/login</code></li>
            <li>In the upper-right corner of any page, click <span class="octicon octicon-rocket" aria-label="The rocket ship " title="The rocket ship "></span></li>
            <li>Search for the name of the repository</li>
            <li>In the right sidebar, click 'Git-LFS'</li>
            <li>Toggle the <code>disable</code> button</li>
          </ul>
        </div>
      </div>
      </div>
  </div>
  ---
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1><a href="/technical/end-user-administration/lab/">End User Administration Lab</a></h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>
