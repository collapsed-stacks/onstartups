## Software audit for possible buyout

- posted by: [AvgJoe007](https://stackexchange.com/users/-1/13518-avgjoe007) on 2011-10-07
- tagged: `selling-business`
- score: 3

We are in the process of auditing a company with a view to buying them out. One of the key parts of this decision is the software they've written and modified over a long period of time. We always have the option of building our own, but we are all aware that it could take us longer to get operational if we built from scratch.

My question is rather specific. I come from a development / PM background, and have been asked to do a full audit of this company's software (which is a web application). We obviously want to know as much as possible about it if we are to go ahead and buy them out. Also, after a basic demo, their system seems to do what we want - BUT we do know that we'll need to modify it to a certain extent.

I am looking for a framework to work through in order to produce my final report. Its been really tough finding anything through google - most of it are just basic checklists at best. I would need a framework / document that deals with infrastructure, design, architecture, hosting etc.

Has anyone had experience with this? I would be very grateful if someone is willing to share their templates with me and am happy to offer a little Amazon reward if I can find the right kind of help!

Thanks in advance



## Answer 31207

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-10-08
- score: 1

<p>If the web application does what you want well, and is free of bugs then that is the first good sign. </p>

<p>So what you are looking for now is to determine it's maintainability, the competence level of the individuals who put it together, or their familiarization with the technologies they used?</p>

<p>I don't think there is any checklist for this; since the web moves at such a fast rate technologies are changing all the time. It wouldn't be uncommon for someone to build an application in a language or framework that was a little unfamiliar. But they should still be using some general best practices.</p>

<p>A good reference for general coding standards and best practices is the book <a href="http://www.cc2e.com/" rel="nofollow">Code Complete</a> - It's not a light read, but I think it is an essential one for programmers or anyone who was going to do a code evaluation.</p>

<ul>
<li>There are some <a href="http://www.cc2e.com/Page.aspx?nid=73" rel="nofollow">checklists</a> on the site, but not exactly what you are looking for.</li>
</ul>

<p>Next, to accurately evaluate the architecture of an application you would have to be familiar with the technology stack.  A PHP application could be architected completely different than a Ruby on Rails application or a .NET MVC application. A PHP app using Symfony or CakePHP would be completely different and have it's own set of conventions and standards.  </p>

<p>What may look weird at a general glance may be completely logical and preferred in that framework.</p>

<p>If you are looking to buy this company for a serious amount of money, and YOU are in charge of the evaluation and do not know the language / framework inside and out I would recommend consulting with someone who does.  </p>

<p>For a medium sized application it would probably only take an expert 3 - 8 hours to walk through the code enough to give you a decent opinion on whether the individuals who wrote this programmed it in a maintainable way, or if they were learning while they coded it, have global variables all over the place, is spagetti code and could be nightmare to maintain long term.</p>

<p>If you are a rockstar coder you could probably review any framework and have a gut feeling of whether they are doing silly things, HUGE methods with tons of if / elses versus breaking things up into very small easy to follow chunks. Is it object oriented, are variables and functions named well and easy to follow. Is it commented... is it written clearly enough to not even need comments (fine by me).  </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
