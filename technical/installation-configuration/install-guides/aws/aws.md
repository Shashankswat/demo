---
layout: slides
title: Installation and Configuration
permalink: /technical/installation-configuration/install-guides/aws/
---

<textarea id="source">
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
            <a name="aws"></a>
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
        <img src="/images/AWS_Management_Console-EC2.png" class="img-responsive">
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

  # GitHub Enterprise AMI 2.7.0

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
              <li>ami-521dda33</li>
              <li>ami-c5ad73a6</li>
              <li>ami-99ac99fa</li>
              <li>ami-ee19ee81</li>
              <li>ami-deeb85ad</li>
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
              <li>ami-24138448</li>
              <li>ami-59fc6f4e</li>
              <li>ami-7bc7871b</li>
              <li>ami-6e04cd0e</li>
              <li>ami-879d22e6</li>
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
        <img src="/images/EC2-security-group.png" class="img-responsive" height="75%" width="75%">
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1><a href="/technical/installation-configuration/enterprise-setup">GitHub Enterprise Setup</a></h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer> 
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>
