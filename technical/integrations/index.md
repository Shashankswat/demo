---
layout: slides
title: Integrating with GitHub Enterprise
permalink: /technical/integrations/
---

<textarea id="source">
  class: title-slide

  <span class="mega-octicon octicon-mark-github"></span>
  <h1>Integrations: Webhooks and APIs</h1>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Integrations: Webhooks and APIs

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><strong>Section Goal:</strong></div>
            <div class="card-text">Enabling a CI/CD workflow with GitHub Enterprise.</div>
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
              <li>Webhooks</li>
              <li>APIs</li>
              <li>Integrations Directory</li>
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

  # Webhooks

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><a href="https://help.github.com/articles/about-webhooks/" target="_blank">Webhooks</a> provide a way for notifications to be delivered to an external web server whenever certain actions occur on a repository or organization.</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Webhooks can be triggered whenever a variety of actions are performed on a repository or an organization. For example, you can configure a webhook to execute whenever:</div>
            <ul class="card-text">
              <li>A repository is pushed to</li>
              <li>A pull request is opened</li>
              <li>A GitHub Pages site is built</li>
              <li>A new member is added to a team</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Using the GitHub API, you can make these webhooks update an external issue tracker, trigger CI builds, update a backup mirror, or even deploy to your production server.</div></br>
            <div class="card-text">For help on building a webhook, including a full list of actions you can associate with, visit our <a href="https://developer.github.com/webhooks/" target="_blank">Developer guide</a>.</div>
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

  # API

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">GitHub Enterprise supports the same powerful API available on GitHub.com as well as its own set of API endpoints. You can find a list of these endpoints <a href="https://developer.github.com/v3/enterprise/" target="_blank">here.</a></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">All API endpoints—except Management Console API endpoints—are prefixed with the following URL: <code>http(s)://hostname/api/v3/</code></div></br>
            <div class="card-text"><a href="https://developer.github.com/v3/enterprise/management_console/" target="_blank">Management Console</a> API endpoints are only prefixed with a hostname: <code>http(s)://hostname/</code></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <div class="card-block">
            <div class="card-text">Enterprise API endpoints accept the same authentication methods as the GitHub.com API. Specifically, you can authenticate yourself with <a href="https://developer.github.com/v3/oauth/" target="_blank">OAuth tokens</a> (which can be created using the Authorizations API) or <a href="https://developer.github.com/v3/#basic-authentication" target="_blank">basic authentication</a>.</div>
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

  # Integrations Directory

  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <a href="https://github.com/integrations" target="_blank"><img src="/images/Integrations_Directory.png" class="img-responsive"></a>
      </div>
    </div></br>
    <div class="row">
      <div class="col-md-4">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><span class="octicon octicon-code"></span> Integrations / <a href="https://github.com/integrations/feature/code" target="_blank">Code</a></div>
            <div class="card-text">GitHub works with the tools you use to write code and deliver software, including editors, IDEs, and continuous integration services.</div>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><span class="octicon octicon-git-pull-request"></span> Integrations / <a href="https://github.com/integrations/feature/collaborate" target="_blank">Collaborate</a></div>
            <div class="card-text">Use GitHub with the apps and services that help you chat, track your progress, and work better with your team.</div></br>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card">
          <div class="card-block">
            <div class="card-text"><span class="octicon octicon-rocket"></span> Integrations / <a href="https://github.com/integrations/feature/ship" target="_blank">Ship</a></div>
            <div class="card-text">Deploy software directly from your repositories using continuous deployment services.</div></br>
          </div>
        </div>
      </div>
    </div>
  </div>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>