## What kind of project collaboration tools are used in a lean startup

- posted by: [priya](https://stackexchange.com/users/-1/14907-priya) on 2011-12-08
- tagged: `hosting`, `project-management`, `lean`, `project`
- score: 2

We would like to understand the kind of tools which are used by other startup(s) for maintaining their projects.

1. Project hosting (SVN or Git) - We have finalized on using Git.
2. Email collaboration - We would like the capability to send group emails, but would also like this to be searchable (Google Apps lets you create groups, but they aren't searchable much similar to what is available in groups.google.com. Should we be creating our mailing lists on groups.google.com instead (by marking it as private). Is this a good idea, how others are doing this?
3. Feature / Task / Bugs / Release management.
4. Project specific docs management.
5. Sometimes we involve early customers to be part of this engagement, so that they can provide feedback, where-in they get access to some portions of the project and not all information
6. Support (email, voice) / Feedback management

We have around 10-20 users and would like a solution which addresses the above needs and costs less. Appreciate your input(s) on this topic.

Note: We use google apps for email, calendar capabilites. If there are some good app(s) on top of Google Apps, we would definitely want to consider them.

We have looked at unfuddle, assembla, GForge so far. Not so comfortable with unfuddle, GForge and assembla seems to be costly for our needs, would prefer a solution which works out cheaper for 10-20 users + 10-15 projects.



## Answer 33482

- posted by: [Roland Pokornyik](https://stackexchange.com/users/-1/7198-roland-pokornyik) on 2011-12-08
- score: 1

2 - Google apps

3 - For release management: 
free kanban tool: 

https://trello.com or 

try versionone: http://www.versionone.com/
- we are using versionone (which is free till 10 users)

4 - For doc management you can use Google Docs or Mediawiki



## Answer 33485

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2011-12-08
- score: 1

<p>2) Consider Google+. We've switch to that, people can use whatever email to get notifications from the system. The conversation thread is then easily accessible online.</p>

<p>5 + 6) Maybe <a href="http://uservoice.com/" rel="nofollow">Uservoice</a>?</p>



## Answer 33744

- posted by: [Mike Eng](https://stackexchange.com/users/-1/15037-mike-eng) on 2011-12-14
- score: 1

<p>1 - <a href="https://github.com" rel="nofollow">Github</a> or <a href="http://beanstalkapp.com/" rel="nofollow">Beanstalk</a></p>

<p>3 - <a href="http://www.pivotaltracker.com/" rel="nofollow">PivotalTracker</a> or <a href="http://trac.edgewall.org/" rel="nofollow">Trac</a></p>

<p>6 - <a href="http://getsatisfaction.com/" rel="nofollow">Get Satisfaction</a></p>



## Answer 33745

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-12-14
- score: 1

1. I use bitbucket: www.bitbucket.org. Can do git and hg and is pretty long time free even for private repos.

2. Gmail only, have Contact groups. Works for small teams fine. I have tried google groups in private, worked for me. I just don't want to share sensitive data, because groups has had some security flaws (remember the spamming time)...

3. Kanbanery.com, I have Mantis installed but want to go to Jira (it is cheap for less users). Release management is done via Maven and the release plugin for me, thats enough. I use Archiva for artifacts.

4. Maven Site. Docs are under version control and shipped with my app. For temporary data I use a wiki on my own webspace

5. I have made something similar, but not found the right answer. I have used a combination of google docs (which sucked) and communication over the bugtracker. surprisingly the latter one worked excellent

6. have not tried, but I hear good things of Zendesk. Personally I use GTalk, Twitter, Email, Phone.

A little bit off topic, but the last tool in my stack is Time & Bill, which I have developed myself. The upcoming team module will let you track your collegs times. Let me know if you want to join the beta test early next year.


## Answer 41700

- posted by: [Sachin Shekhar](https://stackexchange.com/users/-1/17838-sachin-shekhar) on 2012-08-30
- score: 0

1. Github

2. Host own phpBB website

3. Trac and Producteev

4. Evernote (premium version has full-access notebook sharing and version history features; you'll get discount for team)

6. Get Satisfaction



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
