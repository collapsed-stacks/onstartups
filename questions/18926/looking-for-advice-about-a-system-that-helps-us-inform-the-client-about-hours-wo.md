## Looking for advice about a system that helps us inform the client about hours worked and project status

- posted by: [beginning_steps](https://stackexchange.com/users/-1/6373-beginning-steps) on 2011-01-13
- tagged: `tools`, `project-management`
- score: 1

As a startup we have few clients who are billed on time/hour basis and some on the percentage of project completed basis. Now regarding the reporting to the client as of now we were following the process of sending an email to the client in excel spreadhseet or some other format of the work done, percentage completed and the number of hours spent of getting the project to that stage. But we realised lately that it is a very primitive way of reporting and it is taking away some of our productive time.

We are looking for a kind of solution where at the EOD we will update the dashboard for all the clients in one go and then we will sent a generic email to all of them stating that dashboard is updated and if they want they can log-in and view the details of the project progress/ cost etc. etc. So basically what I am looking for is a simple web based (preferably 3rd party) solution where we can use that tool/application to create unique user id for each of our client and then update the dashboard at the end of the day which they can view after logging into their account. They can as well leave a comment but not change any VITAL statistics like hours etc.

Is there any readymade application of this type already there? If there is one it will be great if you can share the details of the same as it will help save lot of time and also help us to maintain a better customer service

Hope to get your feedback and advice...

Best, Neel


## Answer 18928

- posted by: [tomeduarte](https://stackexchange.com/users/-1/6408-tomeduarte) on 2011-01-13
- score: 1

<p>You should look at <a href="http://redmine.org" rel="nofollow">redmine</a>, it does exactly what you need with minimal setup.</p>

<p>It's a web based project management tool with:</p>

<ul>
<li>tasks</li>
<li>roadmaps</li>
<li>forums</li>
<li>several other modules (each can be enabled per-project)</li>
<li>plugins - lots of them (see <a href="https://github.com/search?type=Repositories&amp;q=redmine" rel="nofollow">github</a> and <a href="http://www.redmine.org/plugins" rel="nofollow">official list</a>)</li>
<li>version control integration (git, svn, etc) that can update tasks automatically</li>
</ul>

<p>There's <strong>time tracking built in by default</strong> - per task and per project -, multiple projects and sub-projects (no depth limitation).
You can also setup roles for your customers - e.g. can only do X, Y and Z and user accounts can be assigned to specific projects, which is what you want.</p>

<p>My suggestion is:</p>

<ul>
<li>setup redmine and</li>
<li>create a role for customers, and give that role permission to comment on tasks of projects they belong to.</li>
<li>add a user account for each customer and add them to the relevant projects.</li>
<li>maybe look into installing a plugin for automatic "progress" reminder daily.</li>
</ul>

<p>I also recommend you look around the available plugins as there's very good stuff out there. You should maybe start with <a href="https://projects.littlestreamsoftware.com/projects" rel="nofollow">Eric Davis's plugins</a> - he was release manager until maybe a month ago and has very good plugins.</p>

<p>Keep in mind there's a lot I haven't said here about redmine: you could even setup a workflow so that your customers need to "validate" a UI mockup if you want to dig into the configuration.</p>

<p>All this can be done from the administration interface, have a look at the <a href="http://www.redmine.org/projects/redmine/wiki/Guide" rel="nofollow">user guide</a>.</p>

<p>P.S.: I have been using redmine for a couple years now and it's proven solid. I have used it both software and non-software related businesses and it's worked well.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
