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

  # Migrating to GitHub Enterprise

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Section Goal:</strong></div>
            <div class="card-text">Migrations to GitHub Enterprise.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Topics and Agenda:</strong></div>
            <ul class="card-text">
              <li>Understand common legacy version control systems</li>
              <li>Understand commonly used tools</li>
              <li>Perform a migration</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
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
                <dd> - <a href="https://import.github.com">GitHub.com Importer</a> (TFS, Mercurial, Subversion)</dd>
                <dd> - <a href="https://help.github.com/enterprise/admin/guides/migrations/importing-migration-data-to-github-enterprise/">gh-migrator</a></dd>
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

  # Subversion (SVN)
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;History</strong></div>
              <ul>
                <li>Released by CollabNet in 2000</li>
                <li>Released as an improvement to CVS</li>
                <li>Accepted in Apache Incubator in 2004</li>
              </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common reasons for migrating</strong></div>
              <ul>
                <li>Renaming Files/Dirs not consistent (Copy + Delete)</li>
                <li>No modification time of files</li> 
                <li>Centralized Version Control Model</li>
                <li>No idea of committing locally</li>
                <li>Support for tagging limited</li>
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

  # Perforce
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About Perforce</strong></div>
              <ul>
                <li>Originally released in 1995</li>
                <li>Can be configured as a CVS/DVCS</li> 
                <li>Underlying revision control is proprietary, option for git</li>
                <li>Branching is inter-file like SVN</li>
                <li>Used considerably in the gaming industry</li>
              </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common reasons for migrating</strong></div>
              <ul>
                <li>Automerging of merge-conflicts results in lost work</li>
                <li>Every branch is a heavyweight copy</li>
                <li>Branching requires user-defined-mapping</li>
                <li>No support for stashing/cherry-picking</li>
                <li>Result of merge in Perforce has no relation to merged items</li>
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

  # Mercurial (Hg)
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About Mecurial</strong></div>
              <ul>
                <li>Released in 2005 due to BitKeeper changes</li>
                <li>Platform is Python Based</li>
                <li>Similar history to git</li>
                <li>BitBucket was originally Hg under-the-hood</li>
              </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Reasons for migrating</strong></div>
              <ul>              
                <li>Branches require all prior history</li>
                <li>Branch management isn't unified -- Separate repos vs branches w/in repo</li>
                <li>Learning curve is higher with Hg</li>
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
  <h1>Migration Tools Deep Dive</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  #git-cvsimport

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About the tool</strong></div>
             <ul>
               <li>Built into git</li>
               <li>Uses cvsps2, not cvsps3</li>
               <li>Imports CVS repository to Git repo, or incrementally import into existing git repo</li>
               <li>Targeted towards an incremental update from CVS</li>
               <li>Splitting cvs log into patchsets is done by cvsps2</li>
             </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
          <ul>
            <li>Initial import creates master off of main CVS branch</li>
            <li><i>git merge</i> needs to be run on branches</li>
            <li>Protect imports by using a named remote</li>
            <li>Successful import exits 0</li>
            <li>If code was previously imported, HEAD can contain wrong information</li>
            <li>Refer to documentation for known issues with timestamps</li>
            <li>Empty branches are not imported</li>
            <li>Mulitple tags on same revision are not imported</li>
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

  # Using git-cvsimport

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common Flags</strong></div>
            <ul>
              <li>-d CVSROOT CVS_Module: Specifies root dir and module to import</li>
              <li>-C TARGET_DIR: Specifies target dir, PWD if blankt</li> 
              <li>-r REMOTE Remote to import this CVS repo into</li>
              <li>Note: Moves all CVS branches into remotes/:remote/:branch akin to way git clone uses origin by default</li>
              <li>-o BRANCH_FOR_HEAD - Use if you want to import into a different branch if you want to import HEAD elsewhere</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common Flags Cont'd</strong></div>
          <ul>
            <li>-i No checkout. Keeps working dir and index untouched and does not create if not existent</li>
            <li>-k - Kill keywords. Extracts files with -kk from CVS archive. Recommended, but off by default</li>
            <li>-s Substitutes slashes with a string char of choice</li>
            <li>-a Import all commits, otherwise commits that have a timestamp of less than 10 minutes previous</li>
            <li>-L Limit commits imported by N factor</li>
            <li>-v Verbose mode</li>
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

  #cvs2git

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About the tool</strong></div>
             <ul>
               <li>3rd party import tool</li>
               <li>Needs direct (Not just remote) access to CVS Repo</li>
               <li>Dependent on Python 2.4 or later (Incompatible with Python 3</li>
               <li>Better for clean-cut situation</li>
               <li>Requires git 1.5.4.4 or later</li>
             </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
          <ul>
            <li>Cannot represent a CVS Repo 100% faithfully</li>
            <li>Tool will attempt to create a branch off a single source, but will use a merge from multiple sources if not</li>
            <li>If cvs2git can't create a tag from a single revision, will create a separate branch to fix, but does not delete</li>
            <li>Does not check for legal branch names</li>
            <li>Only converts one project at a time</li>
            <li>Does not convert ignore files</li>          
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

  #ClearCase Migration

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
             <ul>
              <li>History should be imported separately from code</li>
              <li>Base Clearcase vs UCM</li>
              <li>Base ClearCase does not have atomic commits</li>
              <li>ClearCase history does not have transactional integrity</li>
              <li>History will routinely be inconsistent</li>
              <li>Each file change is an individual commit</li>
              <li>Combine commits by time if no conflicts, and author is matched against the CQ record</li>
              <li>Find and ignore incomplete labels. Will break git commands</li>
              <li>Branch hierarchy may need to be manually built</li>
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

  #Subversion - svn2git

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About the tool</strong></div>
             <ul>
              <li>Open-sourced importing tool</li>
              <li>Dependent on git-svn, and ruby</li>
              <li>Ensures branches and tags are imported meaningfully</li>
              <li>Ensures trunk is HEAD, not based on last commit in repo</li>
             </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
          <ul>
            <li>Tags are tied to commit in SVN, thus may not show up in master</li>
            <li>May have issues authenticating on command line for protected repos (Use stored pwd)</li>
            <li>If using a committer's file, every committer must be mapped, otherwise will fail</li>
            <li>Only allows default tag directory</li>       
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

  #Using svn2git

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common Flags</strong></div>
             <ul>
              <li>--rebase : Rebases the existing project against SVN</li>
              <li>--trunk PATH : Define the path for TRUNK</li>
              <li>--branches PATH : Define the path for Branches</li>
              <li>--tags PATH : Define the tags path</li> 
              <li>--rootistrunk : Use if root of the repo is TRUNK and there are no tags or branches</li>
              <li>--notrunk : Do not import trunk</li>
              <li>--nobranches : Do not import branches</li>
              <li>--notags: Do not import tags</li>
              <li>--no-minimize-url : Accept URLs as-is</li>             
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

  #Using svn2git cont'd

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common Flags</strong></div>
             <ul>
              <li>--revision START_REV[:END_REV] : Start importing from SVN at a certain start and end</li>
              <li>--metadata : Include metadata in git logs (svn-git-id)</li>
              <li>--authors : Include an optional file for author mapping (Otherwise use ~/.svn2git/authors)</li>
              <li>--exclude : Regex pattern to exclude directories</li>
              <li>--verbose : Verbose logging</li>        
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

  #Perforce - P4

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;About the tool</strong></div>
             <ul>
              <li>Tool built into git</li>
              <li>Used to create git repositories from P4 repos</li> 
              <li>Can be used as a bridge for P4 users as well moving to git</li>
              <li>A separate client needed to utilize the above functionality</li>
             </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Considerations</strong></div>
          <ul>
            <li>Client needed for options other than cloning or syncing</li>
            <li>Changesets from p4 are imported using git fast-import</li>
            <li>Each commit imported by the tool indicates P4 location and change number. Used by P4 sync</li>
            <li>Branches is different in Perforce, thus use --detect-branches if repo has clean subdirs</li>
            <li>git p4 creates one pack file for each invocation of p4 sync</li>
          </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  ---
  class: title-top

  #Using git-p4

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Common Commands</strong></div>
          <ul>
            <li>Clone - Creates new git dir from existing p4 directory (HEAD from p4 represented as one commmit)</li>
            <li>Sync - Sync the local git repo for changes from the remote p4 depot. Represented as commits</li>
            <li>Rebase - Merges changes from p4 from remote depot into local. Local commits placed on top</li>
            <li>Submit - Submits changes from local repot to P4 remote depot</li>
          </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  ---
  class: title-top

  #Using git-p4 cont'd

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Useful flags</strong></div>
          <ul>
            <li>--branch REF : (Sync) Specify a new ref to sync into, instead of master</li>
            <li>--detect-branches : (Sync) Execute the branch detection algorithm in a given p4 depot</li>
            <li>--bare : (Clone) Perform a bare clone of a p4 depot</li>
            <li>-M: (Submit) Detects renamed files</li>
            <li>--preserve-user : (Submit) - Re-author the change. Requires p4 admin access</li>
          </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
  ---
  class: title-top

  #Agnostic tools

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;GitHub Importer</strong></div>
          <ul>
            <li>Importer tool for GitHub.com</li>
            <li>Closed Sourced tool we self-built</li>
            <li>Normalizes integration input for many other VCS systems</li>
          </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;gh-migrator</strong></div>
          <ul>
            <li>Shell utility</li>
            <li>Used to migrate from GitHub.com -> GHE</li>
            <li>Can migrate between two GHE instances</li>
          </ul> 
          </div>
        </div>
      </div>
    </div>
  </div>
  ---
  class: title-top

  #Migration Documentation
  
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Documentation</strong></div>
              <dl>
                 <dt>CVS</dt>
                  <dd><a href="http://git-scm.com/docs/git-cvsimport">git-cvsimport</a></dd>
                  <dd><a href="http://git-scm.com/docs/gitcvs-migration">Git CVS Migration</a></dd>
                 <dt>ClearCase</dt>
                  <dd><a href="http://therub.org/2013/07/19/clearcase-to-git/">ClearCase to git migration</a></dd>
                 <dt>Subversion</dt>
                  <dd><a href="http://git-scm.com/docs/git-svn">git-svn documentation</a></dd>
              </dl>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
          <div class="card-img-top text-left"><span class="mega-octicon octicon-checklist"></span><strong>&nbsp;Documentation</strong></div>
              <dl>
                 <dt>Perforce</dt>
                  <dd><a href="http://www.perforce.com/perforce/doc.current/manuals/git-fusion/">Git-Fusion Perforce Sync</a></dd>
                  <dd><a href="http://www.perforce.com/blog/120113/git-perforce-client">Git as a Perforce client</a></dd>
                  <dd><a href="http://answers.perforce.com/articles/KB/2790/?q=git-p4&l=en_US&fs=Search&pn=1">git-p4 documentation</a></dd>
                 <dt>Agnostic</dt>
                  <dd><a href="http://git-scm.com/book/en/v2/Git-and-Other-Systems-Migrating-to-Git">Migrating to git</a></dd>
                  <dd><a href="https://help.github.com/articles/importing-from-subversion/#importing-a-subversion-project-using-githubs-importer">Importing from SVN with GitHub importer</a></dd>
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
  <h1><a href="/technical/migrations/lab/">Migrations Lab</a></h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

</textarea>
