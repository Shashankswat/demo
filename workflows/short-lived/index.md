---
layout: slides
title: Task Based Workflows
permalink: /workflows/short-lived/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Task Based GitHub Workflow</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Why Task Based Workflows (5-10 Person Teams)
  
  .nocard[
  - Map branch to task
  - Short lived branches can be merged or closed
  - Share between a subset of team members
  - Short lived branches allow for experimentation
  - CI on tracking branches provides automated reviews
  - Quick peer reviews
  - History maintained on *master* [merge]
  ]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  #Setting Up Your Workstation

  ```sh
    > git clone https://github.com/leefaus/notifications && cd notifications
    > git config -l
    > git config -l --local
    remote.origin.url=https://github.com/leefaus/notifications
    remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
    branch.master.remote=origin
    branch.master.merge=refs/heads/master

    > git config --global user.name "Lee Faus"
    > git config --global user.email "leefaus@me.com"
    > git config --local user.email "leefaus@github.com"
  ```

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Task-Based Workflow

  <img src="/images/devops-flow.png" class="img-responsive">

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  #Creating Branches Locally

  ```sh
    # create a branch off currently checked out branch
    > git branch add-post-to-user
    > git checkout add-post-to-user
    # create a branch off currently checked out branch and checkout
    > git checkout -b add-post-to-user
    # create a branch off currently checked out branch and checkout (contextual ref:)
    > git checkout -b feature/add-post-to-user
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

  <img src="/images/pull-request-screenshot.png" class="img-responsive">

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
