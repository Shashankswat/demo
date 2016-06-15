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
            <dl class="card-text">
              <dt>All history, all branches, all tags</dt>
                <dd>With Meta Data</dd>
                <dd>SCM Tags</dd>
                <dd>Could spin down previous SCM tool after completion</dd>
              <dt>Branch and tag HEADS</dt>
                <dd>Latest revision in repository</dd>
                <dd>Client could be using a multi-branching strategy</dd>
                <dd>May keep legacy VCS server running for legacy applications</dd>
            </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <dl class="card-text">
            <dt>Production HEAD Only</dt>
              <dd>Less need for historical revisions</dd>
              <dd>Less need for other branches</dd>
              <dd>May maintain legacy VCS for N time</dd>
            </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Effort</strong></div>
            <ul class="card-text">
              <li>HIGH.  Compliance and regulation consideration</li>
              <li>MEDIUM. May continue to license legacy VCS</li>
              <li>LOW-MEDIUM. May have no need for non-HEAD code</li>
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

  #Migration Tools
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
              <dt>History</dt>
                <dd>OSS - Released in 1990, released under GNU</dd>
                <dd>Latest revision of CVS -- July 2006</dd>
              <dt>Architecture</dt>
                <dd>Client-Server Model</dd>
                <dd>Support for branching</dd>
                <dd>Delta Compression like git</dd>              
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common reasons for migrating</strong></div>
          <ul>
            <li>Legacy, no active development</li>
            <li>No collaboration features for developers</li>
            <li>Revisions in a commit are per-file, forcing use of tags for relation</li>
            <li>Commits are non-atomic by design</li>
            <li>Branching not encouraged in CVS</li>
            <li>No support for distributed version control</li>
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

  # Using cvs-import
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Using cvs-import</strong></div>
              <dl>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Using cvs-import</strong></div>
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
                <dt>History</dt>
                  <dd>Initial release 1992</dd>
                  <dd>Acquired by IBM in 2003</dd>
                <dt>Architecture</dt>
                  <dd>Centralized VCS</dd>
                  <dd>Windows based UI</dd>
                  <dd>Multi-Server Deployment</dd>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common reasons for migrating</strong></div>
              <dl>
              <dt>End-User Reasons</dt>
                <dd>Very Slow</dd>
                <dd>Non Atomic Commits</dd>
                <dd>Hard to Create new files</dd>
                <dd>Branching/Views are heavyweight</dd>
              <dt>Administrator Reasons</dt>
                <dd>Expensive -- 360k annual cost assuming 90 users</dd>
                <dd>Poor 3rd party integrations</dd>
                <dd>Time investment to teach significant</dd>             
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

  # Using git-cc
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Using git-cc</strong></div>
              <dl>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Using git-cc</strong></div>
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
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Migration Tools Deep Dive</h1>

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
