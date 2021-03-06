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

  # Deploying the Virtual Machine

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

  # Deploying the Virtual Machine

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
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <img class="card-text" class="img-resize" src="/images/ghe-azure-template.png">
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

  # Creating the VM in the Azure Dashboard

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Creation via the Dashboard</strong></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
            <li>On the Azure Template page click <code>Save</code></li>
            <li>To configure, click <code>Edit Parameters</code></li>
            <li>In the <i>Account Prefix</i> field, create a name for the instance</li>
            <li>Select the Region</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
            <div class="card-block"> 
            <ul class="card-text">
            <li>Select the VM Size as per the recommendations</li>
            <li>Enter the disk size for your expected seat count</li>
            <li>Click <code>OK</code> ✨</li>
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

  # Creating/Saving a resource group for the VM

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Creating a Resource Group</strong></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
            <li>Click <code>"Or create new"</code> under "Configure Required Settings</li>
            <li>Create a name for the group</li>
            <li>Select the Region for your group. Does not need to match VM region</li>
            </ul>
          </div>
        </div>
      </div>
        <div class="col-md-6">
        <div class="card">
            <div class="card-block"> 
            <ul class="card-text">
            <li>Click <code>Pin to Starboard</code></li>
            <li>Click <code>Create</code></li>
            <li>Wait approx 5 minutes for the VM to show up</li>
            </ul> 
          </div>
          </div>
        </div>
      </div>
      <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Disk Encryption: </strong>An encrypted data volume provides an extra level of security by ensuring that any data you write to your instance is protected. There's a slight peformance impact when using encrypted disks. If you decide to encrypt your volume, we strongly recommend doing so before starting your instance for the first time. For more information, see <a href="https://azure.microsoft.com/en-us/documentation/articles/key-vault-manage-with-cli/">the guide on using Azure's Key Value encryption.</a> Instead of creating a new resource group, you can <a href="https://help.github.com/enterprise/admin/guides/installation/installing-github-enterprise-on-azure/#creating-a-new-resource-group-for-the-vm-and-data-disk">provide the name of the resource group you created earlier.</a>z</div>
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

  # Creating the VM in the command line

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Creation via the Command Line</strong></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
            <li>Ensure aws cli is running in asm mode: <code>azure config mode asm</code></li>
            <li>Create a <code>Premium LRS</code> storage account: <code>azure storage account create NAME -l REGION --type PLRS</code></li>
            <li>Find the latest GitHub VM: <code>azure vm image list | grep GitHub</code></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
            <div class="card-block"> 
            <ul class="card-text">
            <li>Create the VM: <code><br />azure vm create \<br />
                                 --vm-size vm_size \<br />
                                 --location "region" \<br />
                                 --userName ignoreduser \<br />
                                 --password ign0redP@ss \<br />
                                 vm_name \<br />
                                 appliance_image_name</code></li>
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

  # Configuring the security group

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Creation via the Command Line</strong></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <ul class="card-text">
            <li><code>azure vm endpoint/<br /> 
                               create-multiple vm_name/ <br /> 
                               122,<br />
                               80,<br />
                               8080,<br />
                               443,<br />
                               8443,<br />
                               9418,<br />
                               25,<br />
                               161:161:udp,<br />
                               1194:1194:udp</code></li> 
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

  # Select an Instance

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <img src="/images/ghe-azure-hostname.png" class="img-responsive">
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
