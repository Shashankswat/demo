---
layout: slides
title: Installation and Configuration
permalink: /technical/installation-configuration/install-guides/azure/
---

<textarea id="source">
  ---
  class: title-top

  # Install GitHub Enterprise - Azure

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>What you will need:</strong></div>
            <ul class="card-text">
              <li>An <a href="https://azure.microsoft.com/" target="_blank">Azure account</a> capable of provisioning new machines</li>
              <li>A GitHub Enterprise license file. To download an existing license file or request a trial license, visit <a href="https://enterprise.github.com/" target="_blank">enterprise.github.com</a>.</li>
              <li>If you're setting up instances via the command line, you'll need <a href="http://azure.microsoft.com/en-us/documentation/articles/xplat-cli/">Azure CLI</a> installed locally on your machine</li>
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
             <li><a href="https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-azure/" target="_blank">Enterprise Azure Installation Guide</a></li>
             <li><a href="http://azure.microsoft.com/en-us/pricing/details/virtual-machines/#Linux">Azure VM Overview</a></li>
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

  # Supported Regions

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">GitHub Enterprise is supported in the following Azure Regions</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text" style="list-style-type: none; padding-left: 0px;">
            <small>
            <li><code>Central US</code></li>
            <li><code>East US</code></li>
            <li><code>East US 2</code></li>
            <li><code>South Central US</code></li>
            </small>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text" style="list-style-type: none; padding-left: 0px;">
            <small>
            <li><code>West US</code></li>
            <li><code>North Europe</code></li>
            <li><code>West Europe</code></li>
            </small>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text" style="list-style-type: none; padding-left: 0px;">
            <small>
            <li><code>East Asia</code></li>
            <li><code>SE Asia</code></li>
            <li><code>Japan East</code></li>
            </small>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Region ID </div>
            <ul class="card-text" style="list-style-type: none; padding-left: 0px;">
            <small>
            <li><code>Japan West</code></li>
            <li><code>Aus East</code></li>
            <li><code>Aus West</code></li>
            </small>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Azure Federal: </div>
            <ul class="card-text">
              <li>GitHub Enterprise is available in Azure Federal. This allows US Federal customers with specific regulatory requirements to run GitHub Enterprise in a federally compliant cloud environment.</li>
              <li>For more information on AWS compliance with federal standards, see the <a href="https://azure.microsoft.com/en-us/overview/clouds/government/" target="_blank">Azure Federal page</a>.</li>
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
            <div class="card-text">For Azure deployments, based on your seat count we recommend these instance types:</div>
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
              <li>Standard_DS3</li>
              <li>Standard_DS12</li>
              <li>Standard_DS14</li>
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

  # Obtaining the Virtual Machine

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>To deploy to Azure, you can deploy from the GitHub Enterprise portal, the Azure dashboard, or the command line</strong></div>
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
            <img class="card-text" class="img-responsive" src="/images/vm-download.png">
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block"> 
            <div class="card-block"> 
            <img class="card-text" class="img-responsive" src="/images/vm-azure.png">
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
