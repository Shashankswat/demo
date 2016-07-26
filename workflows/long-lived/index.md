---
layout: slides
title: Integration Branches
permalink: /workflows/long-lived/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Integration Branch Based GitHub Workflow</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Long Running Branch Based Workflows (> 10 Person Teams)

  .nocard[
  - Map branch to a set of tasks, sprint or environment
  - Long running is *time based*, not *task based*
  - CI on integration branch creates multi-team, integrated packages
  - History tracked on *integration* branch
  - Merge/Rebase from integration to master through squash commits for clean releases
  - Tag/Release off *master*
  ]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: full-screen

  <img src="/images/devops-flow.png" class="img-responsive">

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: full-screen

  <img src="/images/long-running-branches-screenshot.png" class="img-responsive">

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  #Creating Branches Locally

  ```sh
    # create a branch off currently checked out branch
    > git branch add-post-to-user development
    > git checkout add-post-to-user
    # create a branch off currently checked out branch and checkout
    > git checkout -b add-post-to-user development
    # create a branch off currently checked out branch and checkout (contextual ref:)
    > git checkout -b feature/add-post-to-user development
  ```

  <footer>
   <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  #Commits

  ```sh
    # create a branch off currently checked out branch and checkout
    > git checkout -b add-post-to-user
    > atom .
    ###
    # make a bunch of edits
    ###

    # Add all new files or you can add them specifically
    > git add -A
    > git add config/routes.rb

    # Commit all changed files or commit them individually
    > git commit -am "added path to routes.rb"
    > git commit config/routes.rb -m "added path to routes.rb"
  ```

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Pushing Changes to GitHub

  ```sh
    # Push changes recently committed to a tracking branch
    > git push origin add-post-to-user
    # Push changes recently committed to different branch
    > git push origin add-post-to-user:master
    # Sample result                                                        
    Username for 'http://faushouse.vm': chewbacca
    Password for 'http://chewbacca@faushouse.vm':
    Counting objects: 3, done.
    Delta compression using up to 4 threads.
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 313 bytes | 0 bytes/s, done.
    Total 3 (delta 2), reused 0 (delta 0)
    To http://faushouse.vm/republic/calculator
    * [new branch]      add-post-to-user -> add-post-to-user
    ```
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: full-screen

  <img src="/images/pull-request-choice.png" class="img-responsive">

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-slide

  <span class="mega-octicon octicon-device-desktop"></span>
  <h1>Demo</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>
