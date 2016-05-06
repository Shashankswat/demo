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

  # Migration Strategies
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
        </br>
       </div>
      </div>
    </div>
  </div>
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
          <ul class="card-text">
           <li>All history, all branches, all tags</li>
           <li>Branch and tag HEADs only</li>
           <li>Production HEAD only</li>
         </ul>
       </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-block">
        </br>
       </div>
      </div>
    </div>
  </div>

  # Migration Tools
  - CVS
      - [git-cvsimport command](https://github.com/git/git/blob/master/git-cvsimport.perl)
  - Clearcase
      - [git-cc tool](https://github.com/charleso/git-cc)
  - Subversion
      - [git-svn command](https://github.com/git/git/blob/master/git-svn.perl)
      - [svn2git tool](https://github.com/nirvdrum/svn2git) (adds tag conversion)
      - [`gh-migrator`](https://help.github.com/enterprise/admin/guides/migrations/importing-migration-data-to-github-enterprise/)
  - Perforce
      - [git-p4 command](https://github.com/git/git/blob/master/git-p4.py)
  - Agnostic
      - [git-import GitHub CLI tool](https://github.com/github/git-import) (TFS, Mercurial, Subversion)
      - [GitHub.com Importer](https://importer.github.com) (TFS, Mercurial, Subversion)

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