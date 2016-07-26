---
layout: slides
title: Advanced Administration
permalink: /workflows/forked/
---

<textarea id="source">
  class: title-slide

  .mega-octicon.octicon-mark-github[# Innersourcing and Forked Repositories]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  ---
  class: title-slide

  .mega-octicon.octicon-mark-github[# Inner Source Methodology]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  ---
  class: title-top

  # What is Inner Source?  

  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Open source origins</h3>
								<ul>
									<li>non-systematic process</li>
									<li>distributed development</li>
									<li>collaborative approach</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Common constraints</h3>
								<ul>
									<li>geography</li>
									<li>time-zones</li>
									<li>cultural</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]	

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Who else is doing it
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>NASA (JPL)</h3>
								<ul>
									<li>Research Driven Software Development</li>
									<li>Developers work across team</li>
									<li>Code sharing</li>
									<li>Code-Reuse</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Paypal</h3>
								<ul>
									<li>Literally wrote the book</li>
									<li>Based on an academic study</li>
									<li>Hosts an annual Inner Source Summit</li>
									<li>Saw an increase in Developer Efficiency</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]	

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Tenets of Open Source
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
								<ul>
									<li>Open access to Source Code</li>
									<li>Transparent Dev Environments</li>
									<li>Peer Review of Contributions</li>
									<li>Informal Communication</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
								<ul>
									<li>Self-Selected Motivated Contributors</li>
									<li>Frequent Release Cycle w/Early Feedback</li>
									<li>Around the Clock Development</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-slide

  .mega-octicon.octicon-mark-github[# Inner Source Applied]

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Open Access to Source Code and Artifacts
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Developers are solving the same problems</li>
									<li>Curb re-invention of the wheel</li>
									<li>See other technologies and tools in-use</li>
									<li>Encourages collaboration</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>How?</h3>
								<ul>
									<li>Repositories public by default</li>
									<li>Allow cross-organiziational users to join</li>
									<li>Allow organic team creation</li>
									<li>Allow Read-Write Access for Users Across Repositories</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Transparent Development Environments
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>See how other teams manage</li>
									<li>Do all have DEV/QA/UAT Environments?</li>
									<li>Are some teams utilizing IoC?</li>
									<li>What tools are other teams using?</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>How?</h3>
								<ul>
									<li>Utilize Infrastructure Automation as much as possible</li>
									<li>Maxmise freedom on workstations, not release/prelease env</li>
									<li>Enforce standards in the pipeline</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>	
  ---
  class: title-top

  # Peer Review of Contributions
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Find bugs early and often</li>
									<li>Generate collaboration immediately</li>
									<li>Build fresh perspective</li>
									<li>Utilize the entire sum of your team's knowledge</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>How?</h3>
								<ul>
									<li>Pull Requests opened on the first commit in a branch</li>
									<li>Allow outside teams to subscribe and comment on issues</li>
									<li>Break code within a branch</li>
									<li>Encourage other teams to write new unit-tests</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>	
  ---
  class: title-top

  # Informal Communication Channels
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Move away from Daily Stand-Ups</li>
									<li>Less reliance on caverns of email</li>
									<li>Maintain flow when developer is in the groove</li>
									<li>Maintain team-feel even w/remote employees</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>How?</h3>
								<ul>
									<li>Use line comments on code in PRs</li>
									<li>Use Chat for team communication</li>
									<li>Use video chat for hangouts</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Self-Selected Motivated Contributors
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Teams identify leaders vs experts</li>
									<li>Sometimes leaders != experts. That's okay!</li>
									<li>Expertise identified in the day-to-day</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Encourages equality among team-members</li>
									<li>Encourages organic team creation and growth</li>
									<li>Teams already have an idea of who is a leader and/or expert</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Frequent Release Cycle with Early Feedback
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Increase delivery frequency</li>
									<li>Decrease time spent idle</li>
									<li>Bring team into release conversations</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>How?</h3>
								<ul>
									<li>Utilize tools like Jenkins/TeamCity/Etc for CI</li>
									<li>Use post/pre-receive hooks to trigger builds instead of polling</li>
									<li>Code and build iteratively</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
  ---
  class: title-top

  # Around the clock development
  .container[
  	.row[
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>Why?</h3>
								<ul>
									<li>Developers may be geo-distributed</li>
									<li>Developers work better at different times</li>
									<li>'9-5' can hinder efficiency</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  		.col-md-6[
  			.card[
  				.card-text[
  					.card-block[
						<section>
							<h3>How?</h3>
								<ul>
									<li>Allow/Encourage Developers to WFH/Alternative Hours</li>
									<li>Give 24 hours of PR Reviews and Feedback</li>
									<li>Use a system of async slow/fast and sync for comms</li>
									<li>PR Review, Slack, Phone/In-Person</li>
								</ul>
						</section>
  					]
  				]
  			]
  		]
  	]]
  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>

  <footer>
    <div class="octicon-spacer"><span class="octicon octicon-logo-github"></span><span class="tagline">how people build software</span></div>
  </footer>
</textarea>
