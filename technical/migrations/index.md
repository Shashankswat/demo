---
layout: slides
title: Migrating to GitHub Enterprise
permalink: /technical/migrations/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Migrating to GitHub Enterprise</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Migrations 
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common migration paths</strong></div>
            <ul class="card-text">
              <li>All history, all branches, all tags</li>
              <li>Branch and tag HEADS only</li>
              <li>Production HEAD only</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Effort and Use Case</strong></div>
            <ul class="card-text">
              <li>HIGH. Common use case for firms with lots of regulation and compliance</li>
              <li>MEDIUM. Common use case when firm may need to roll back code, but may still license previous VCS to retain history</li>
              <li>LOW-MEDIUM. Common use case when customer isn't concerned about code that isn't HEAD, or for meta-data </li>
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

  #Common Migration Tools
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common migration paths</strong></div>
              <dl>
               <dt><b>CVS</b></dt>
                <dd> - <a href="https://github.com/git/git/blob/master/git-cvsimport.perl">git-cvsimport</a></dd>
               <dt><b>Clearcase</b></dt>
                <dd> - <a href="https://github.com/charleso/git-cc">git-cc</a></dd>
               <dt><b>Subversion</b></dt>
                <dd> - <a href="https://github.com/git/git/blob/master/git-svn.perl">git-svn</a></dd>
                <dd> - <a href="https://github.com/nirvdrum/svn2git">svn2git</a>(adds tag conversion)</dd>
                <dd> - <a href="https://help.github.com/enterprise/admin/guides/migrations/importing-migration-data-to-github-enterprise/">gh-migrator</a></dd>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common migration paths</strong></div>
              <dl>
               <dt><b>Perforce</b></dt>
                <dd> - <a href="https://github.com/git/git/blob/master/git-p4.py">git-p4</a></dd>
               <dt><b>Agnostic</b></dt>
                <dd> - <a href="https://github.com/github/git-import">git-import GitHub CLI tool</a>(TFS, Mercurial, Subversion)</dd>
                <dd> - <a href="https://importer.github.com">GitHub.com Importer</a> (TFS, Mercurial, Subversion)</dd>
              </dl>
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

  #CVS

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About CVS</strong></div>
              <dl>
               </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About cvs-import</strong></div>
              <dl>              
              </dl>
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

  # ClearCase
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About ClearCase</strong></div>
              <dl>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About cc-import</strong></div>
              <dl>              
              </dl>
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

  # Subversion (SVN)
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About Subversion</strong></div>
              <dl>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About the tools</strong></div>
              <dl>              
              </dl>
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

  # Perforce
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About Perforce</strong></div>
              <dl>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About the tools</strong></div>
              <dl>              
              </dl>
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

  # Other tools
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;The Tools</strong></div>
              <dl>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Things to Consider</strong></div>
              <dl>              
              </dl>
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
  # Migration Documentation

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
        </br>
       </div>
      </div>
    </div>
  </div>

  - CVS
    - [git-cvsimport documentation](http://git-scm.com/docs/git-cvsimport)
    - [Git CVS migration documentation](http://git-scm.com/docs/gitcvs-migration)
  - Clearcase
    - [Clearcase to Git migration blog post](http://therub.org/2013/07/19/clearcase-to-git/)
  - Subversion
    - [git-svn documentation](http://git-scm.com/docs/git-svn)
  - Perforce
    - [Git Fusion Perforce sync feature](http://www.perforce.com/perforce/doc.current/manuals/git-fusion/)
    - [Git as a Perforce client](http://www.perforce.com/blog/120113/git-perforce-client)
    - [Perforce git-p4 documentation](http://answers.perforce.com/articles/KB/2790/?q=git-p4&l=en_US&fs=Search&pn=1)
  - Agnostic
    - [Migrating to Git](http://git-scm.com/book/en/v2/Git-and-Other-Systems-Migrating-to-Git)
    - [From `svn` (Subversion)](https://help.github.com/articles/importing-from-subversion/#importing-a-subversion-project-using-githubs-importer)
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Customer Story

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
        </br>
       </div>
      </div>
    </div>
  </div>

  - Software Company in Washington, DC
  - 12yrs of history in Clearcase, Clearquest
  - Multiple VOB Servers
  - Global presence with Clearcase Multi-site

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>
