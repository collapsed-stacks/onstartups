## Would like some feedback on JIRA, Intervals, Unfundle, and other bug/issue tracking packaged

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2010-01-12
- tagged: `bug-tracking`, `software`, `crm`
- score: 1

I would like to get your opinion on bug/issue tracking packages.

In my last software dev company we used JIRA with one of the flavors of Subversion. That was in 2007, so a lot has changed since and there are many more players out there.

So JIRA I am familiar with, but I am also looking at Intervals (myintervals.com, which integrates with Quickbooks), Unfundle, and there is also Assembla. Subversion or Git integration is almost a must. Integration with Freshbooks is something we are considering. CRM integration will be somewhere down the line, once we kick Salesforce to the curb.

Would love to hear some feedback/opinion on the packages mentioned.

P.S. I am not a dev, I am looking at this more from business person point of view, so please forgive me if I am not going deep in the tech requirement portion.

TO CLARIFY:
All the packages I am mentioning have one feature we need - issue tracking. I realize some have code repositories, some project management, etc. etc. etc.
What I am trying to achieve is:

1. Find out what general reputation each of those packages have
2. How well issue/bug tracking features work on those packages
3. How well the mentioned main feature would fit with CRM, code repository, and time-tracking pieces we need to complete the puzzle.

Addition 2:
Most devs are working in Python and some of the sub-flavors of it.


## Answer 6414

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-01-12
- score: 1

<p>I have used Trac and elementool, but my current favorite is <a href="http://www.fogcreek.com/FogBugz/" rel="nofollow">Fogbugz</a>. </p>

<p>You should read about it from their own site - as I can't know exactly what features you will want/need.</p>

<p>The support is great. </p>

<p>EDIT:</p>

<p>On closer inspection it seems that your question is a hodge-podge of requests.  </p>

<p>I think you will need to define exactly what it is you are looking for rather than throwing around names of issue trackers, time tracking software and code repositories.  </p>

<p>FOLLOW UP</p>

<p>I suspect the majority of the ones you mention will work fine for your needs.  </p>

<p>I am happy with the time tracking feature of Foggbugz as well as its integration with other tools.  (note there are plugins - like one for time tracking for fogbugz.)</p>

<p>I am not sure what level of "CRM" you need, but you can communicate with clients and sales leads using fogbugz.  I also think the company that makes the software uses it to manage the job/resume/candidate workflow internally.</p>

<p>I am not affiliated with them - I am just a user and it is the tool I am most familiar with.</p>

<p>All the others you mention will integrate with version control systems and all will work fine as issue trackers.  </p>

<p>I am ignorant about their functionality for time tracking and CRM.</p>



## Answer 6433

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-12
- score: 1

<p>In my experience, you shouldn't try to integrate the <em>development tools</em> (Subversion, issue tracker etc) with the <em>business / sales tools</em> (Salesforce, accounting etc). First off, typically there is no out-of-the-box facility for integrating tools from the two worlds. Second, the business value isn't actually there.</p>

<p>In a past job I set up <a href="http://www.atlassian.com/studio/" rel="nofollow">Jira Studio</a>, the hosted version of Atlassian's bugtracker, wiki, Subversion, code viewer and more. It worked well, and Atlassian's support was great. My main dislike with Atlassian's products is their user interface; it is complicated and tends to overwhelm the user with options. This can be mitigated with end user training.</p>

<p>I have played around with Fogbugz, and I'm an avid reader of Joel Spolsky and the BoS forum. Forgbugz is currently my favorite system for pure bug- &amp; task-tracking, because its AJAX user interface is impressively well done, and permits a fast and intuitive approach to working with issues and tasks. It's wiki etc feel less feature-rich and impressive to me.</p>

<p>An interesting, up-and-coming player is <a href="http://www.jetbrains.com/youtrack/" rel="nofollow">YouTrack</a> from Jetbrains. It has a very keyboard-centric approach, think of it as a custom command line for issue tracking. I could see this working very well with programmers.</p>

<p>As I see it, the <strong>industry is converging on "programmer productivity suites"</strong>, i.e. multi-functional packages that handle several programming-centric needs. My 'positioning' of the packages right now is:</p>

<ul>
<li>Fogbugz: Best user experience, best for smaller - midsized teams. A little behind on the "suite" part, next step is their <a href="http://fogcreek.com/kiln/" rel="nofollow">Kiln SCM &amp; peer review</a> tool.</li>
<li>Atlassian: Best for larger companies which need deep feature set. Very mature "suite" right now, most functionality covered. Steep learning curve, much to gain from heavily customizing their applications for your company's needs, and from educating users.</li>
</ul>



## Answer 6438

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2010-01-13
- score: 0

I haven't used Fogbugz, though it does look nice, but one of the nicer systems I used was taking advantage of open-source, in that you can modify the code, and give it back.

So, one company had tied Subversion with Bugzilla, so that when the developer fixed a problem and committed it, you could see the changes in Bugzilla, so you could group bugs to be fixed in a sprint (using scrum), and tasks in that sprint, and as tasks were done the submission of the code could help keep track of what went where.

So, once you have a clear idea as to what you want to do, then you may be able to find that people have ways to tie different applications together to build up what you are looking for.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
