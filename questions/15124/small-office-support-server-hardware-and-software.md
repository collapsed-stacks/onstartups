## Small office "support" server- hardware and software?

- posted by: [MarkD](https://stackexchange.com/users/-1/4804-markd) on 2010-10-14
- tagged: `office`, `service`, `support`, `computers`
- score: 2

So I am in the process of launching a new venture.  The new company will be a niche consulting company centered around some complex simulation tools that have been developed, are the company will continue to expand them.  The startup funds are in the bank, and I am currently the sole active employee (and have been for the past few months).

However, I am getting to the point where I will be hiring a couple of people.  They are individuals I have worked with in the past, and are quite experienced in the field of interest.  While we all have the mathematical, engineering, and programming background necessary to get this thing moving, none of us have developed in a "non-academic" setting.

This leads to my problem- what do I need in terms of a server/software to support said development?  Each employee will have a Mac-based workstation.  We will also have a small Linux HPC cluster for running simulations.

The things that come to mind:

- A revision control system (I have used and am happy with SVN).
- Automated testing of checked in revisions.
- Incremental backups for each machine.
- Offsite backup (any particularly good services out there?).
- Accounting software (probably not on a server, but on my machine).

I am comfortable with a linux environment, but would also be happy with a mac-mini running OS X Server providing any services necessary.  So my questions are-

- What am I missing in the list above?
- Other than the revision control system, using Time Machine, and simple backups using rsync, I have no experience with any of the other points.  Any tips or suggestions?
- The current office will be three people, but I can see it eventually growing.  Are there services/policies I should be putting in place now to facilitate that growth?


## Answer 15126

- posted by: [Dan Dyer](https://stackexchange.com/users/-1/4221-dan-dyer) on 2010-10-14
- score: 1

<p>If you're happy with SVN then there's not really any need to use anything else.  Some developers prefer distributed systems such as Git and Mercurial, but you could always migrate to those later if required.</p>

<p>For continuous integration (automated testing), <a href="http://hudson-ci.org/" rel="nofollow">Hudson</a> is a good Open Source option.  <a href="http://www.jetbrains.com/teamcity/" rel="nofollow">TeamCity</a> is also pretty neat and is free for up to 20 users and projects.</p>

<p>For off-site back-up you could use <a href="http://aws.amazon.com/s3/" rel="nofollow">Amazon S3</a>.</p>

<p>One thing you don't mention is bug/issue tracking.  <a href="http://www.atlassian.com/software/jira/" rel="nofollow">JIRA</a> would probably be very useful for helping to manage your project(s) and it only costs $10 for up to 10 users (it starts to get pricey after that).</p>

<p>Maybe you would also find a wiki useful for collaborative documentation.  <a href="http://www.mediawiki.org/wiki/MediaWiki" rel="nofollow">Mediawiki</a>, the software that powers Wikipedia, is free, or for another $10 you can get a 10-user licence for <a href="http://www.atlassian.com/software/confluence/" rel="nofollow">Confluence</a>, which will integrate nicely with JIRA.</p>

<p>A cheaper alternative to buying/renting your own hardware to run these services would be to use one or more Virtual Private Servers.  One option is <a href="http://slicehost.com" rel="nofollow">Slicehost</a>, who I've used without complaint, though currently I prefer <a href="http://xtrahost.co.uk" rel="nofollow">Xtraordinary Hosting</a> as they offer more for the same money.</p>



## Answer 15137

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-10-15
- score: 0

One thing to think about is whetehr you should fully virtualize. I do that to a large success.I ahve a couple of by now (2nd in building) local office virtual server platforms (in addfition to some servers in a data center).

* A small cude
* an AMD 6 core Ahtlon goes a long way.
* Micro ATC boards can hold 16gb memory these days.
* Addd an Adapted 3405 RAID controller and
* A SuperMicro 2.5" disc cage that fits 8 dsics into 2x5.25 slot

I run the discs as 4x320gb in Raid 10 (OS, virtualization) and 4x500gb Raid 5 (file storage).

And you have quite a powerhouse. THen you can install virtual machines to your liking.

In my case the second is currently being built, and there is a 64gb higher end server in a data center for handling most of hte production (virtual workstations, database etc.).



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
