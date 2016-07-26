---
layout: slides
title: Advanced Administration
permalink: /workflows/securing/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Securing Branches</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Why Secure a Branch?

  - Protect a Branch from Force Pushing
  - Specify teams or users allowed to merge
  - Use Required Statuses to disallow failed code
  - A secured branch should be 100% deployable
  - Help Developers break bad habit of committing directly to master

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Protected Branches
 
  - Disables `git push --force`
  - Prevents irrevocable changes
  - Branches can not be deleted
  - Can be used in tandem with Required Statuses

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Required Statuses
 
  - Tag commits with a status
  - `SUCCESS` `FAILURE` `ERROR` `PENDING`
  - Commonly used with Continuous Integration
  - Commonly multiple checks are used with Status API
  - CI, Code Review, Approval Gates
  - API is available

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Branch Restrictions

  - Separate from Protected Branches
  - Prevents `who` can push to a branch
  - Scoped to User/Team
  - Can even include Admins
  - Common uses include Approval Teams
  - Give junior developers merge rights later

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Ultra Protection Scenario

  - Branch has webhook for CI 
  - Developer submits good/bad code
  - CI reports back to Status API
  - Even if the code passes, still cannot merge
  - Approved pusher still can't merge if there are merge conflicts
  
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>		
</textarea>
