## Unsuccessful job posting, what did I do wrong? What should I focus on?

- posted by: [Incognito](https://stackexchange.com/users/-1/11587-incognito) on 2011-07-11
- tagged: `recommendations`, `jobs`, `recruiting`, `hire`
- score: 4

First, *it is not my intent to abuse the Q&A forum to hire people, I'm asking about what I've done wrong. I've removed my company name, details, and industry from the posting below.*

I'm a new company looking to get someone with software development skills. 12 calendar days ago, I posted a job for a Web developer.

This is the first hire I've ever needed to do, and really starting to feel the weight of spreading myself too thin, and really disappointed with my results from my methods.

I decided to post directly to our internal website, and include an online interview.

I've had 250~ page views to the posting, and my bounce rate is near 100% in the first 10 seconds.

I'm not in a software region (ie, San Francisco, Mountain view, etc.), but figured that someone would have applied.

I posted the job to facebook, twitter, forrst, hackernewsjobs, craigslist, kijiji, and reddit. I was successful in getting highly localized hits (almost 90% of visitors in 50km of the office).

I've had 0 persons apply to this job, and I cannot find feedback from anyone on how to improve this.

***I've censored out the industry, company name, location, and contact details, but here's the text I used.*** 

----------

**Job Description**

Example is a new company specializing in consulting services specific to technology in the Example industry.

We are presently looking for a web developer with strong JavaScript skills and a good knowledge of Postgres, HTML, CSS, and PHP. You may be working on several projects per year, and have feedback into the design process of projects. You will be the other half of a development team, and should have a great understanding of tools that are used. Your shift will be Monday-Friday, for a standard working day. There is potential for telecommuting as well as working weekends instead, but not initially.

**Responsibilities:**

Your primary responsibility will involve minor work in the design phase and major work in the development phase.

Your secondary responsibility will range in task, but be related to building and maintaining software. You should be comfortable refactoring bad code, resolving issues with performance, setting up miscellaneous software, finding bugs, fixing bugs, and maintaining code.

Your tertiary responsibility will involve dealing with documentation, resolving minor hardware issues, and keeping the development and production systems free of problems, as well as speaking with users of the software if there is a need.

**Skills**

**Primary**

* English fluency and communication skills.
* Problem solving abilities, related to the product being developed.
* JavaScript. You must have excellent JavaScript skills. We do quality checks with jshint, and a light approach to unit testing.
* You should be comfortable enough with jQuery that you can write your own plugins.
Web languages on modern and legacy browsers. You must be able to hand-write HTML and CSS (SASS and/or LESS are also acceptable), and understand CSS frameworks. We do validation using csslint, W3C Validator, and lastly in-the-browser testing.
* Postgres. You should understand general SQL concepts such as relationships and normalization. Standard SQL queries involving joins, where clauses, calculations, procedural calls. We're not implicitly looking for someone who knows how to write procedures and administrate, but it is a great asset. We're mostly looking for your ability to write efficient queries and succinct schema.
* PHP5. You should understand how to write a PHP class. Most of the PHP used is for calling the database and returning JSON, with part of it towards generating some pages. Moving forward, any noscript content will depend on bridging this concept.
* Good research skills. Few people know everything, but you must be able to find that information quickly, or know the right places to ask.

**Secondary**

* You should be able to write and understand C# code in an ASP.NET environment.
* Refactoring without premature optimization.
* How to deal with security while preserving data integrity. For instance, XXS exploits, SQL injection, or otherwise.
* Linux command line. We're not expecting you to know advanced VIM features, but you should know the basic command line.

**Tertiary**

* Knowing how to administrate webservers, specifically Apache and IIS, potentially node.js in the future.
* We are migrating from Microsoft SQL and MySQL towards postgres, it would be an asset if you knew the differences.
* We use GIT as a source control, and viewgit and gitosis to deal with repositories. You should know basic source control practices.
* Our software could run in VirtualBox, VM Ware and/or Hyper-V.
* You should know how SSH works, be it from something like putty, or a linux terminal.
* We use Redmine to track bugs, features, and otherwise.
* We use DokuWIKI to keep internal notes. Knowing how markdown and a wiki works is useful.




## Answer 27418

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-07-11
- score: 6

When I read this, i have only two things which might prevent me before applying. 

In germany, if somebody writes "probably weekend work" it means "you have to work at least 1 weekend per month, maybe more often". Sometimes working weekends can happen. If it is more an exception than a rule, I would remove it. Exceptions happen, but (personally speaking) I don't want to work for a company on my weekends on a regular basis.

If you really need that, tell about how you compensate the weekend work. Can I have free time weekdays? Maybe I missed this (language thing), but if not, I would be interested in that.

The second thing is, you have a very hard skill set. I would remove anything which can be learned in no time. for example, Redmine. I have no clue about redmine, but I am pretty sure I can work with it after 30 minutes. No need to mention, except it is very cool (I don't think it is). Git is cool, by the way. I would write: Able to use GIT or willing to learn.

You are looking for an administrator, who is a JavaScript Guru has good PHP knowledge and is even able to programm C#/.NET (if you can read it, you can probably write it). You are good with Windows && Linux. And of course Postgres, MySQL and yeah, MS SQL would be good.

How likely is it that you ever meet such a guy? He is either very senior and has good luck that he can meet most of you requirements. Or well, not a clue.

I would recommend you to reduce the skill set. I would leave in the primary skill set. That is perfectly acceptable. PHP5 and PostgreSQL as backend, JavaScript in frontend. Have in mind that experts in JavaScript usually have so much work that they are really no experts in Postgres or other backend technologies.

I would delete off the most of the other two sections, except those which are really important to you or are cool (GIT is cool, again).

You can check out the secondary and teritary knowledge in a call or a meeting. Maybe there is a nice competent, and willing guy who does not match perfectly but is willing to learn and you like him so much, that you'll forgive him he has never used Linux before

Good luck!
Christian


## Answer 27422

- posted by: [tomeduarte](https://stackexchange.com/users/-1/6408-tomeduarte) on 2011-07-11
- score: 4

I'm a developer and systems administrator, with 5 years experience. I'm very proactive about learning and I don't think I know everything you want. Most people won't be able to apply except for senior rockstar developers and that's going to be hard to find.

Please keep in mind that the list below is my opinion only. That does not mean every developer out there agrees.

As to the listing itself, I think you can improve on this:

 - most developers like **specifics**. Don't spend two paragraphs saying what can be listed as 5 or 6 list items;
 - schedule. 9-to-5 weekday job? Stay simple, say it like that. I can trade weekends for weekdays? Great, but be clear that 1) it's my choice 2) it's a trade, not overtime;
 - no need for three levels: just `Required` and `Great to have`;
 - be specific about the tools and state those I need to develop for e.g. saying `Dokuwiki` doesn't tell me if I'll need to develop plugins for it - and they're a pain.
 - it's most important you get someone who knows the must-haves and is willing to learn than trying to find Mr. Right.


----------

I'd try something along the lines of:

**Job Description**

Example is a new company specializing in consulting services specific to technology in the Example industry.

We are looking for a web developer with strong JavaScript skills and a good knowledge of related web-development technologies: HTML, CSS, PHP and PostgresSQL. You'll be working in a team with our founder - you'll have an opinion on projects design and get feedback whenever you need it.

There is potential for telecommuting and working on weekends (in exchange for weekdays) if you wish after we get comfortable working together.

**Responsibilities**

*( I made no changes here, your text's perfect)*

Your primary responsibility will involve minor work in the design phase and major work in the development phase.

Your secondary responsibility will range in task, but be related to building and maintaining software. You should be comfortable refactoring bad code, resolving issues with performance, setting up miscellaneous software, finding bugs, fixing bugs, and maintaining code.

Your tertiary responsibility will involve dealing with documentation, resolving minor hardware issues, and keeping the development and production systems free of problems, as well as speaking with users of the software if there is a need.

**Skills**

***Must-have***

 - Be fluent in English
 - Be willing to learn how to work with technologies if needed - nothing far-fetched, things like `MS SQL`, `Apache` or `IIS`, `Node.js`
 - Strong `JavaScript` skills
 - `jQuery`, including plugin authoring
 - `HTML` and `CSS`: you can use `Less`/`Sass` if you like.
 - `PostgresSQL`
 - We use `git` as version control. Basic git workflows, or equivalent knowledge of other DVCS systems.
 - `PHP5` to support a `JSON` webservices architecture. 

***Good to have***

 - Security mindset: be aware of what `XSS`, `SQLi` and related attacks are, and how to prevent them
 - Refactoring skills
 - `C#` coding on a `.NET` environment
 - Basic `Linux` command-line skills

***You will learn***

We use several different internal tools for managing our projects and servers, and you'll learn them easily:

 - `Redmine` for tracking bugs, features, etc
 - `Dokuwiki` for keeping notes (hint: `Markdown`)
 - `SSH` for accessing servers
 - Virtualization software: `VirtualBox`, `VMWare` and/or `Hyper-V`.

----------

Feel free to adapt the above to your listing if you find it useful.

Good luck with your hiring.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
