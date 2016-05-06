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

  # Private Mode

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card-block">
          <div class="card-text">In <a href="https://help.github.com/enterprise/admin/guides/installation/enabling-private-mode/" target="_blank">private mode</a>, GitHub Enterprise requires every user to sign in to access the installation. To enable private mode: </div></br>
          <ul class="card-text">
            <li><a href="https://help.github.com/enterprise/admin/articles/accessing-the-management-console/" target="_blank">Access the Management Console</a></li>
            <li>click 'Settings'</li>
            <li>click 'Privacy'</li>
            <li>Select 'Private mode'</li>
          </ul>
        </div>
      </div>
      <div class="col-md-6">
        </br>
        <img src="/images/SIDEBAR-Privacy.png" class="img-resize"></br>
        <img src="/images/PRIVATE-Mode.png" class="img-resize">
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
          <div class="card-text">You can enable or disable <a href="https://help.github.com/enterprise/admin/articles/configuring-git-large-file-storage-for-a-repository/" target="_blank">Git LFS</a> on a per-repository basis: </div></br>
          <ul class="card-text">
            <li>As a site admin, sign in to your GitHub Enterprise instance at <code>http(s)://[hostname]/login</code></li>
            <li>In the upper-right corner of any page, click <span class="octicon octicon-rocket" aria-label="The rocket ship " title="The rocket ship "></span></li>
            <li>Search for the name of the repository</li>
            <li>In the left sidebar, click 'Advanced Settings'</li>
            <li>In the Key field, type <code>git-lfs</code></li>
            <li>In the Value field, type <code>true</code> or <code>false</code></li>
          </ul>
        </div>
      </div>
      <div class="col-md-6">
        </br>
        <img src="/images/ADVANCED-Settings.png" class="img-resize"></br>
        <img src="/images/GIT-LFS.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>