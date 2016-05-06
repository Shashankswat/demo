---
layout: slides
title: Installation and Configuration
permalink: /technical/installation-configuration/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Installation and Setup</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Installation and Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Section Goal:</strong></div>
            <div class="card-text">Understand the basics for installing GitHub Enterprise in the cloud and on premise.</div>
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
              <li>Install GitHub Enterprise</li>
              <li>Obtain and Upload a new license</li>
              <li>Upload a new SSH key</li>
              <li>Add LDAP Sync</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Topics and Agenda:</strong></div>
            <ul class="card-text">
              <li>Login as an LDAP User</li>
              <li>Access Org and Repo</li>
              <li>See Sync'd Teams</li>
              <li>Promote a User to Site Admin</li>
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

  # Install GitHub Enterprise

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>What you will need:</strong></div>
            <ul class="card-text">
              <li>An <a href="https://aws.amazon.com/" target="_blank">AWS account</a> capable of launching EC2 instances and creating EBS volumes.</li>
              <li>A GitHub Enterprise license file. To download an existing license file or request a trial license, visit <a href="https://enterprise.github.com/" target="_blank">enterprise.github.com</a>.</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Installation Instructions:</strong></div>
            <ul class="card-text">
              <li><a href="https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-aws/" target="_blank">Enterprise 2.4 AWS Installation Guide</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Configuration Instructions:</strong></div>
            <ul class="card-text">
              <li><a href="https://help.github.com/enterprise/admin/guides/installation/" target="_blank">Enterprise 2.4 Configuration Guide</a></li>
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

  # Select EC2

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/AWS_Management_Console-EC2.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Launch Instance

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-Launch.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise AMI

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Select a GitHub Enterprise AMI based on the <a href="http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html" target="_blank">AWS Region</a> you would like to launch the instance into.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text">
              <li>ap-northeast-1</li>
              <li>ap-southeast-1</li>
              <li>ap-southeast-2</li>
              <li>eu-central-1</li>
              <li>eu-west-1</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">AMI ID </div>
            <ul class="card-text">
              <li>ami-4d240e23</li>
              <li>ami-0818db6b</li>
              <li>ami-d84d16bb</li>
              <li>ami-abd2cec7</li>
              <li>ami-35319246</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text">
              <li>sa-east-1</li>
              <li>us-east-1</li>
              <li>us-west-1</li>
              <li>us-west-2</li>
              <li>us-gov-west-1</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">AMI ID </div>
            <ul class="card-text">
              <li>ami-0ade5966</li>
              <li>ami-0ec38964</li>
              <li>ami-bd741fdd</li>
              <li>ami-28617e49</li>
              <li>ami-2075c841</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">GovCloud Support: </div>
            <ul class="card-text">
              <li>AMIs are also available in the <a href="http://aws.amazon.com/govcloud-us/" target="_blank">AWS GovCloud (US) region</a>. This allows US customers with specific regulatory requirements to run GitHub Enterprise in a federally compliant cloud environment.</li>
              <li>For more information on AWS compliance with federal standards, see the <a href="https://aws.amazon.com/compliance/" target="_blank">AWS compliance page</a>.</li>
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

  # Select the AMI

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-AMI.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Choose an Instance

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">For on-premises deployments, based on your seat count we recommend these hardware configurations:</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Seats</strong></div>
            <ul class="card-text">
              <li>0-499</li>
              <li>500-2999</li>
              <li>3000-5000</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-2">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>vCPUs</strong></div>
            <ul class="card-text">
              <li>2</li>
              <li>4</li>
              <li>8</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-2">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Memory</strong></div>
            <ul class="card-text">
              <li>16 GB</li>
              <li>32 GB</li>
              <li>64 GB</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Storage</strong></div>
            <ul class="card-text">
              <li>100 GB</li>
              <li>250 GB</li>
              <li>500 GB</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-2">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Root</strong></div>
            <ul class="card-text">
              <li>80 GB</li>
              <li>80 GB</li>
              <li>80 GB</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">For AWS deployments, based on your seat count we recommend these instance types:</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
              <li>0 - 499</li>
              <li>500 - 2999</li>
              <li>3000 - 5000</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
              <li>r3.large</li>
              <li>r3.xlarge</li>
              <li>r3.2xlarge</li>
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

  # Select an Instance

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-Select-Instance.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Launch the Instance

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Once your instance is running, copy the VM's public DNS name and paste it into a web browser.  If the page doesn't load, try updating the AWS security group for your EC2 instance to allow https connections (port 443).</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-Review.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Attach Block Storage

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">After you've verified the instance, attach block storage of at least 10GB from the AWS EC2 Console.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-Volume.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # EBS Volume

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Make sure the EBS volume is in the same availability zone as your EC2 instance.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-EBS-Review.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Attach to EC2

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Attach the EBS volume to your EC2 instance.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/EC2-EBS-Attach.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Login

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Login or sign up for a trial at <a href="https://enterprise.github.com/login" target="_blank">enterprise.github.com/login</a> to obtain your license.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Login.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise License

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Download License (or appliance for an on-premises install).</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Download.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Navigate to the public DNS of the EC2 VM and continue to Setup, bypassing browser certificate warnings.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Setup.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Upload the GitHub Enterprise License file and create a Site Administrator password.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-License.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Select a New Install.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-New.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Under Hostname, test the domain settings.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Test.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Save settings and the instance will be configured.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Done.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Create an Admin Account.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Admin.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Create an Organization.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Org.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Add Organization Members (optional).</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Members.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Setup is Complete!

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/GHE-Home.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Upload New SSH Key

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Add your SSH public key to the list of authorized keys on the Management Console's settings page. </br>Open <code>https://{host}/setup/settings</code> in a browser and add your key to the list:</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/SSH-Keys.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # SSH Administration

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">SSH access allows you to run the <a href="https://help.github.com/enterprise/admin/articles/command-line-utilities/" target="_blank">GitHub Enterprise command line utilities</a> and is useful for troubleshooting, running backups with the GitHub Enterprise Backup Utilities, and for configuring replication.  Administrative SSH access is managed separately from Git SSH access and is accessible only via port 122.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Once your SSH key has been added to the list, connect to the instance over SSH as the "admin" user:</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><code>$ ssh -p 122 admin@github.example.com</br>Last login: Sun Nov  9 07:53:29 2014 from 169.254.1.1</br>admin@github-example-com:~$ █</code></div>
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

  # Enable LDAP

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">LDAP lets you authenticate GitHub Enterprise against your existing accounts and centrally manage repository access. <a href="https://help.github.com/enterprise/admin/guides/user-management/using-ldap/" target="_blank">Refer to the Enterprise 2.4 documentation</a> for instructions to configure LDAP Synchronization:</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/LDAP-Sync.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Promote Site Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Site administrators can promote any normal user account to a site administrator, as well as demote other site administrators to regular users. <a href="https://help.github.com/enterprise/admin/guides/user-management/promoting-or-demoting-a-site-administrator/" target="_blank">Refer to the Enterprise 2.4 documentation</a> for full instructions.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">SSH into your appliance and run ghe-user-promote with the username to promote:</div>
            <div class="card-text"><code>$ ghe-user-promote username</code></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <img src="/images/SITE-Admin.png" class="img-responsive">
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
              <li>Sign in to your GitHub Enterprise instance</li>
              <li>In the upper-right corner of any page, click <span class="octicon octicon-rocket" aria-label="The rocket ship " title="The rocket ship "></span></li>
              <li>Search for the name of the user</li>
              <li>In the left sidebar, click 'Admin'</li>
              <li>Site admin > Danger Zone, click 'Promote'</li>
              <li>Type a reason for promoting the user</li>
              <li>Click 'Promote'</li>
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