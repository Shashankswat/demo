# GitHub Partner Enablement

 - [Technical Collateral](https://gh-enablement.herokuapp.com/)

## Prerequisites
 - [GitHub account](https://github.com/join)
 - [Enterprise license](https://enterprise.github.com/login)
 - [AWS account](https://aws.amazon.com/)
 - [Basic Git Knowledge](https://try.github.io/levels/1/challenges/1)
- Install Subversion
- Install Git
- Install Ruby

## Agenda  
30m - **Business Concept Setting**

---  
30m - **GitHub Enterprise Installation and Setup**  
1h - **GitHub Setup Lab**  

---
10m - **Break**

---
30m - **End User Administration Concepts**  
1h - **End User Administration Lab**

---
45m - **Migrating to GitHub Enterprise**  
45m - **Migration Lab (SVN to GitHub)**

---
1h - **Lunch**

---
45m - **Integrations: Webhooks, API's**  
45m - **Integrations Lab**  

---
10m - **Break**

---
30m - **GitHub Advanced Administration**  
1h - **Advanced Administration Lab**

---
15m - **Expectations**  

## Acknowledgements
- built with [middleman](https://middlemanapp.com/)
- rendered for slide shows through [remark](http://remarkjs.com/)
- responsive formatting via [bootstrap](http://v4-alpha.getbootstrap.com/)  
- exported to PDF using [decktape](https://github.com/astefanutti/decktape)  

Access to published collateral is limited to members of the [GitHub Partners](https://github.com/githubpartners) repository by [jekyll auth](https://github.com/benbalter/jekyll-auth).

## Building this Repository
- Install [Ruby](https://github.com/rbenv/rbenv), [RubyGems](https://github.com/rubygems/rubygems), and [Bundler](https://github.com/bundler/bundler)
- `git clone https://github.com/githubpartners/enablement`
- `gem install middleman`
- `cd resources`
- `bundle install`
- `bundle exec middleman server`
- Open Browser to [http://localhost:4567](http://localhost:4567)

## Known Issues
 - For OSX 10.11 El Capitan, if Middleman fails to install or run properly it may be an [issue](https://github.com/eventmachine/eventmachine/issues/643) with the eventmachine gem.  If you have [Homebrew](http://brew.sh/) installed this command should correct the problem: `brew link openssl --force`
