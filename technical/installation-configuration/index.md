---
layout: slides
title: Installation and Configuration
permalink: /technical/installation-configuration/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>GitHub Enterprise Architecture and Installation</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Enterprise Architecture and Installation

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Section Goal:</strong></div>
            <div class="card-text">Understand GitHub Enterprise's architecture and Installation (On-Prem/Cloud)</div>
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
              <li>The GitHub Enterprise Appliance</li>
              <li>Components of the Appliance</li>
              <li>Installation Offerings</li>
              <li>Licensing</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Topics and Agenda:</strong></div>
            <ul class="card-text">
              <li>Provisioning and Configuration</li>
              <li>Authentication</li>
              <li>GitHub Pages</li>
              <li>Monitoring</li>
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

  # GitHub Enterprise Appliance

  <div class="container">
  <div class="row">
    <div class="col-md-12">
      <div class="card">
        <div class="card-block">
          <div class="card-text">
            <span class="octicon octicon-organization card-img-top"></span><b>GitHub Enterprise: How businesses build software</b>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Features</h4>
          <ul class="card-text" style="list-style: none;">
          <li><span class="octicon octicon-heart"></span> Delivered as a single virtual image</li>
          <li><span class="octicon octicon-heart"></span> No public internet access needed</li>
          <li><span class="octicon octicon-heart"></span> Behind the firewall</li>
          <li><span class="octicon octicon-heart"></span> Take advantage of OSS Collaboration</li>
          <li><span class="octicon octicon-heart"></span> Choose your authentication</li>
          </ul>
        </div>
      </div>
        <div class="card">
        <div class="card-block">
          <h4 class="card-title">Benefits</h4>
          <ul class="card-text">
            <li>Streamlined Installation</li>
            <li>Less overhead for Admins</li>
            <li>Lightweight Infrastructure</li>
            <li>Industry-Standard Install Stack</li>
            <li>Single-appliance scaling</li>  
          </ul>
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

  # GitHub Enterprise Components

  <div class="container">
    <div class="col-md-12">
      <div class="card">
        <div class="card-block">
          <div class="card-text">
            <img src="/images/enterprise-deep-dive.png" style="max-width: 90%; height: auto;">
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

  # Installation Offerings

  <div class="container">
  <div class="row">
    <div class="col-md-12">
      <div class="card">
        <div class="card-block">
          <div class="card-text">
            <span class="octicon octicon-organization card-img-top"></span><b>GitHub Enterprise Installation Offerrings</b>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Platforms</h4>
          <ul class="card-text" style="list-style: none;">
          <li><span class="octicon octicon-checklist"></span> VMware</li>
          <li><span class="octicon octicon-checklist"></span> Xen/KVM/Hyper-V</li>
          <li><span class="octicon octicon-checklist"></span> Amazon Web Services</li>
          <li><span class="octicon octicon-checklist"></span> Microsoft Azure</li>
          <li><span class="octicon octicon-checklist"></span> Google Cloud Platform</li>
          </ul>
        </div>
      </div>
        <div class="card">
        <div class="card-block">
          <h4 class="card-title">Things to ask 🤔</h4>
          <ul class="card-text">
            <li>Do you currently run a virtualized environment?</li>
            <li>Do you currently host in the cloud?</li>
            <li>Have you designated an internal Product Owner for GHE?</li>
            <li>Are you consdering GHE as a SaaS Product?</li>
            <li>How are you planning to manage support?</li>  
          </ul>
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

  # Licensing

  <div class="container">
  <div class="row">
    <div class="col-md-12">
      <div class="card">
        <div class="card-block">
          <div class="card-text">
            <span class="octicon octicon-organization card-img-top"></span><b>GitHub Enterprise Licensing</b>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">License Offerings</h4>
          <ul class="card-text">
            <li>Annual license</li>
            <li>Multi-Year license</li>
            <li>Minimum 10 users per license</li>
            <li>No value-adding of services -- All In</li>
            <li>Base price: $250 pp/py</li>
          </ul>
        </div>
      </div>
        <div class="card">
        <div class="card-block">
          <h4 class="card-title">Obtaining a License</h4>
          <ul class="card-text">
            <li>Trial License - 45 days</li>
            <li>enterprise.github.com</li>
            <li>Links for appliance download</li>
            <li>Links to Support Portal</li>
            <li>Resources/Cases Studies/Knowledge Base</li>
          </ul>
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

  # enterprise.github.com login

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

  # GitHub Enterprise Download: https://enterprise.github.com/releases/x.y.z/download

  <div class="container">
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Provisioning and Installation</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1><a href="install-guides/aws/">Amazon Web Services</a></h1>
  <h1><a href="install-guides/azure/">Microsoft Azure</a></h1>
  <h1><a href="https://help.github.com/enterprise/2.9/admin/guides/installation/">On-Prem</a></h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Install GitHub Enterprise - AWS

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
             <li><a href="https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-aws/" target="_blank">Enterprise AWS Installation Guide</a></li>
             <li><a href="http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/LaunchingAndUsingInstances.html" target="_blank">Launching EC2 Instances</a></li>
             <li><a href="http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html">Managing EBS Volumes</a></li>
             <li><a href="http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-network-security.html">Using Security Groups</a></li>
             <li><a href="http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-vpc.html">Using VPCs</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Configuration Instructions:</strong></div>
            <ul class="card-text">
             <li><a href="https://help.github.com/enterprise/admin/guides/installation/" target="_blank">Enterprise Configuration Guide</a></li>
             <li><a href="https://help.github.com/enterprise/2.12/admin/guides/installation/network-configuration">Network Configuration</a></li>
             <li><a href="https://help.github.com/enterprise/2.12/admin/guides/installation/updating-the-virtual-machine-and-physical-resources">Updating VM Resources</a></li>
             <li><a href="https://help.github.com/enterprise/2.12/admin/guides/user-management/authenticating-users-for-your-github-enterprise-instance/">Authentication Guides</a></li>
             <li><a href="https://help.github.com/enterprise/2.12/admin/guides/installation/system-resource-monitoring-and-alerting">System/Resource Monitoring</a></li>
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

  # Install GitHub Enterprise - AWS

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/AWS_quickstart.png" class="img-responsive">
      </div>
    </div>
      <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <p class="card-text">
              <strong>AWS quickstarts provide a CloudFormation template to auto-provision GitHub Enterprise instances into new, or existing VPCs ✨</strong>
            </p>
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

  # Install GitHub Enterprise - AWS

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

  # GitHub Enterprise Supported Regions

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
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text">
              <li>ap-northeast-1/2</li>
              <li>ap-southeast-1/2</li>
              <li>ap-south-1</li>
              <li>eu-central-1</li>
              <li>eu-west-1/2</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text">
              <li>sa-east-1</li>
              <li>us-east-1/2</li>
              <li>us-west-1/2</li>
              <li>us-gov-west-1</li>
              <li>ca-central-1</li>
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

  # Choosing an Instance

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
              <li>200 GB</li>
              <li>200 GB</li>
              <li>200 GB</li>
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

  # Creating a security group
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><a href="https://help.github.com/enterprise/2.12/admin/guides/installation/installing-github-enterprise-on-aws/#creating-a-security-group">Creating Security Groups (Detailed)</a></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Ports</div>
            <ul class="card-text">
              <li>8443 (TCP)</li>
              <li>8080 (TCP)</li>
              <li>122 (TCP)</li>
              <li>443 (TCP)</li>
              <li>80 (TCP)</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Ports</div>
            <ul class="card-text">
              <li>22 (TCP)</li>
              <li>9418 (TCP)</li>
              <li>25 (TCP)</li>
              <li>1194 (UDP)</li>
              <li>161 (UDP)</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Thoughts</div>
            <ul class="card-text">
              <li>UDP Traffic is Reserved for HA/Backups</li>
              <li>Save this for reference</li>
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

  # Attach Block Storage

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">After you've verified the instance, attach block storage of at least 100GB from the AWS EC2 Console.</div>
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
       <div class="card">
        <div class="card-block">
         <div class="card-title">
          <img src="/images/EC2-Review.png" class="img-resize">
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

  # GitHub Enterprise Setup

  <div class="container">
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
            <div class="card-title">Your AWS key will auto-fill. This gives limited shell access to GitHub Enterprise</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-ssh.png" class="img-responsive">
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
            <div class="card-title">Add your SSH public key to the list of authorized keys on the Management Console's settings page. <br/>Open <code>https://{host}/setup/settings</code> in a browser and add your key to the list:</div>
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

  # NTP Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Defaults to System-defined NTP Servers. Change here if another NTP server is required</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-ntp.png" class="img-responsive">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Authentication Setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Choose an authentication method. Best practice avoiding built-in authentication</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ec2-auth.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Enable LDAP/LDAP Sync

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
           <div class="card-text">LDAP lets you authenticate GitHub Enterprise against your existing accounts and centrally manage repository access. <a href="https://help.github.com/enterprise/admin/guides/user-management/using-ldap/" target="_blank">Refer to the Enterprise documentation</a> for instructions to configure LDAP Synchronization. Allows for Role-Based Access Control for team members and team roles</div>
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

  # Privacy Settings and Private/Public Mode

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">SSL is heavily encouraged. If GHE is accessible via the internet, public mode can not be turned on.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-privacy.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Privacy Settings and Private/Public Mode

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Enable/Disable GitHub Pages. Pages can also be Public, so users don't need a license to see the website</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-pages.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Email setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Required for email notifications</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-email.png" class="img-resize">
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Monitoring setup

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-title">Various logging methods supported</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-monitoring.png" class="img-resize">
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
            <div class="card-text"><code>$ ssh -p 122 admin@github.example.com<br/>Last login: Sun Nov  9 07:53:29 2014 from 169.254.1.1<br/>admin@github-example-com:~$ █</code></div>
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

  # Promote Site Admin

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
           <div class="card-text">Site administrators can promote any normal user account to a site administrator, as well as demote other site administrators to regular users. <a href="https://help.github.com/enterprise/admin/guides/user-management/promoting-or-demoting-a-site-administrator/" target="_blank">Refer to the Enterprise documentation</a> for full instructions.</div>
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
  ---
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Authentication</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # External Authentication
  <div class="container">
    <div class="col-md-12">
    <div class="row">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
        <div class="card-title"><h3>CAS</h3></div>
        <p class="card-text"><strong>CAS</strong> is an SSO Protocol for the internet. Services like Apereo provide CAS as a means of a single source of truth for user authentication</p>
        </div>
       </div>
        <div class="card">
        <div class="card-block">
          <div class="card-title"><h3>LDAP</h3></div>
          <p class="card-text"><strong>LDAP</strong> is a directory service protocol commonly used in enterprise organizationss. Active Directory supports LDAP to GHE</p>
        </div>
      </div>
      <div class="card">
        <div class="card-block">
        <div class="card-title"><h3>SAML</h3></div>
        <p class="card-text"><strong>SAML</strong> is an XML based language for exchanging authentication. Commonly, users of SAML will federate multiple idPs into a single SAML source.</p>
        </div>
      </div>
    </div>
    </div>
    <div class="row">
    <div class="card">
        <div class="card-block">
        <div class="card-title"><h3>Built in Authentication</h3></div>
        <p class="card-text">GitHub Enterprise ships with authentication, but it is strongly encouraged to integrate with a customer's existing idP</p>
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

  # CAS Considerations

  <div class="container">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Considerations</h4><br />
          <ul class="card-text" style="font-size: 24px;">
            <li>Usernames are alphanumeric w/dashes</li>
            <li>Usernames created from email address</li>
            <li>If multiple usernames normalize, 1st one wins</li>
            <li>Strongly recommended to use SSL</li>
            <li>SSL cert installed on GHE</li>
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

  # LDAP Considerations

  <div class="container">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Considerations</h4>
          <ul class="card-text">
            <li>Usernames can only be alphanumeric</li>
            <li>Non-alphanumeric characters are normalized to dashes</li>
            <li>Changes to LDAP accounts are not automatic, unless sync is enabled</li>
            <li>Manually sync via the console or via API trigger</li>
            <li>With LDAP sync enabled, any user can search the LDAP tree</li>
            <li>Restrict this functionality with restricting the permissions of the DSU</li>
            <li>Support for the following group classes: group, groupOfNames, groupOfUniqueNames, posixGroup</li>
            <li>These classes can be nested</li>
          </ul>
        </div>
      </div>
        <div class="card">
        <div class="card-block">
          <h4 class="card-title">Settings and Attributes</h4>
          <ul class="card-text">
            <li>Encryption - Plain, SSDL/LDAPS, or StartTLS</li>
            <li>Domain Search User - LDAP User that performs lookups</li>
            <li>Domain Search Password - Password for the above account</li>
            <li>Administrators Groupd</li>
            <li>Domain base</li>
            <li>Restricted User Group </li>
            <li>User ID - Typically uid, or sAMAccountName</li>
            <li>Profile Name - Name to appear on the profile page</li>
            <li>SSH keys</li>
            <li>GPG Keys</li>
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

  # SAML Considerations

  <div class="container">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Considerations</h4>
          <ul class="card-text" style="font-size: 24px;">
            <li>GitHub Enterprise utilizes SAML 2.0</li>
            <li>Usernames must be alphanumeric, dashes allowed</li>
            <li>Metadata available at <code>http(s)://[hostname]/saml/metadata</code></li>
            <li>SSH/GPG keys can be stored via SAML for GHE</li>
            <li>Site Admins can be granted through SAML admin tag</li>
            <li>SAML users must be suspended from GHE if suspended from idP</li>
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
  <h1>GitHub Pages</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # GitHub Pages Overview

  <div class="container">
    <div class="col-md-12">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
          <h4 class="card-title">Considerations</h4>
          <ul class="card-text" style="font-size: 24px;">
            <li>Static sites hosted on GitHub Enterprise</li>
            <li>Can be public or private</li>
            <li>Built on Jekyll</li>
            <li>Can use pre-built template</li>
            <li>Can also use markdown</li>
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

  # Types of GitHub Pages
  <div class="container">
    <div class="col-md-12">
    <div class="row">
    <div class="card-group">
      <div class="card">
        <div class="card-block">
        <div class="card-title"><h3>User</h3></div>
        <p class="card-text">Users can have a GH Pages site setup tied to their username. Always hosted under the <code>https://pages.[hostname]/[username]</code> if you create a repo with <code>[username].[hostname]</code>. Hosted on the master branch</p>
        </div>
       </div>
        <div class="card">
        <div class="card-block">
          <div class="card-title"><h3>Organization</h3></div>
          <p class="card-text">Similar to a User Page, but this is scoped to an Organization on GitHub Enterprise</p>
        </div>
      </div>
      <div class="card">
        <div class="card-block">
        <div class="card-title"><h3>Project</h3></div>
        <p class="card-text">A project repo can also have it's own GH Pages, hosted under the <code>gh-pages</code> branch in the project</p>
        </div>
      </div>
    </div>
    </div>
    <div class="row">
    <div class="card">
        <div class="card-block">
        <div class="card-title"><h3>Thinking about GH Pages</h3></div>
        <p class="card-text">Customers use GitHub Pages to level-up documentation, enhance projects, and help give insight to organizations. Encourage your customers to experiment!</p>
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
  <h1><a href="/technical/installation-configuration/lab/">Installation and Configuration Lab</a></h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>
