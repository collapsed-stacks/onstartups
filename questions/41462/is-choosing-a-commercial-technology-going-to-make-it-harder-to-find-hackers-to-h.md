## Is choosing a commercial technology going to make it harder to find hackers to hire?

- posted by: [Xananax](https://stackexchange.com/users/-1/14476-xananax) on 2012-08-18
- tagged: `outsourcing`, `conflicts`, `bootstrap`
- score: 1

I am currently working as a tech advisor for a start-up. We tried composing a dev team for a while, but were unable to find talented people.  
We got a proposal from a company to build our app, backed up with Magento. The idea is to go with that, and find our team while version 1 is being built by that company.

Magento sorta fits our needs, but it's not ideal. Any other CMS would do just as well. I am myself more of a node kind of guy, advocate of open-source, and so on; I dislike CMSs, and would rather go with a framework. In particular, our project would greatly benefit from a noSQL database, and Magento works on SQLs backends.  
this said, I am willing to put aside philosophical matters for the sake of the project. "Fast iterations will always beat ideal iterations" and all that stuff.

However, I am weary about one thing:  
###How easy is it to build a tech team after the project has started?

Here is my reasoning:

  - Talented devs are already scarce
  - Choosing any particular tech restricts your potential hires, but this can be a good thing: restricting your tech to node or perl means you are actually widening your percentage of possibly talented devs. But Magento is not exactly the type of technology that hackers are enthusiastic about.
  - Any really good dev is a creative person who has an inflated ego (myself included) and I will have a hard time convincing them of jumping in the bandwagon, when all the tech choices are already made, to basically *improve* an app, as opposed to creating it from the ground up.

My options:

  1. Not take the company's contract, and continue trying to build a team, with the risk of not reaching our milestones in time
  2. Take the company's contract, but insist for them to use technologies that fit our ethos better, in order to be able to attract like-minded people, with the risk of imposing on them technologies they are not familiar with.
  3. Just forget about ever building an internal team, and try to work out a long-term deal.

This is a cornerstone of our project's development and I am weary of taking the wrong decision.


## Answer 41463

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2012-08-18
- score: 1

<p>I am going to be devil's advocate here and say you are putting up artificial barriers.</p>

<blockquote>
  <p>How easy is it to build a tech team after the project has started?</p>
</blockquote>

<p>From what I have seen - no difference in <em>effort</em> required, only <em>how</em> you build the team differs. Different technical talent likes to work on different problems, so you just need to calibrate and educate <em>yourself</em> how you will approach the recruiting.</p>

<blockquote>
  <p>Talented devs are already scarce</p>
</blockquote>

<p>Yes, if you are going to do what the masses do (look for only CSers, 100% spec fit, %0 ramp-up time expectation, same geographic location, market to same usual 20-25 white/asian single male demographic).</p>

<blockquote>
  <p>Choosing any particular tech restricts your potential hires, but this can be a good thing: restricting your tech to node or perl means you are actually widening your percentage of possibly talented devs. But Magento is not exactly the type of technology that hackers are enthusiastic about.</p>
</blockquote>

<p>Do you really want to work with developers who have platform fetish? Maybe I have been lucky or maybe it is Midwest and East coast kind of thing, but I know of more tech agnostic devs than those with the platform fetishes. "I will use whatever we need to and whatever gets the job done" is usually what I want and do hear, which results in an immediate offer letter from us.</p>

<blockquote>
  <p>Any really good dev is a creative person who has an inflated ego (myself included) and I will have a hard time convincing them of jumping in the bandwagon, when all the tech choices are already made, to basically improve an app, as opposed to creating it from the ground up.</p>
</blockquote>

<p>So having been both a talent agent (yes, like in entertainment talent agent) and responsible for bringing on talent for tech companies I work(ed) with, I challenge you to consider that you may not be giving credit to creatives they deserve. Yes, there are plenty of egos, but those are usually stuck working on projects that get into enormous scope and feature creep. There are far more bright, smart, gifted engineering artists (what I call them) who want to work with other gifted people. Magento, MySQL, etc. are just tools. Right team can make masterpieces with any tool.</p>

<p><strong>Focus less on tools and more on the business problem. Less philosophy and more building what solves problems and pays bills.</strong></p>

<p>Much more fun with hackathons and "play" with any tools can be had when payroll is met, bills are paid, and there are some additional resources.</p>

<p>Here are couple of articles I have written that may be useful to you:</p>

<p><a href="http://theoperationsguy.com/stars-vs-constellations-3-steps-building-solid-high-performing-teams" rel="nofollow">Stars vs. Constellations – 3 Steps to Building Solid High-Performing Teams</a></p>

<p><a href="http://theoperationsguy.com/how-hire-talent-without-paying-recruiters" rel="nofollow">How To Hire Top Talent Without Paying Recruiters</a></p>



## Answer 41464

- posted by: [Andrew Smith](https://stackexchange.com/users/-1/18504-andrew-smith) on 2012-08-18
- score: 0

For your particular problem, you can outsource significant number of issues into the cloud first. For example, EdgeCast runs Magento at blazing fast performance, and assures cashing levels, security and so on, which also solves global replication and management.

Secondly, there are low-cost cluster databases, which solve significant problem too, like Amazon RDS.

When you have this already installed, you have 50% of your job completed, and now you need to establish dev cycle. For this you require (single CMS), a developer who does OO PHP, and when he familiarizes a bit with it (you can ask for Magento devs), ask him to upload some small module or feature to it, using the mentioned CDN, while using high security for the cluster SQL and module permission (encryption). Then try to discuss security and data isolation issues, what is secure token and PCI requirements for payment card processing, and there you go.

You can use cloud for development, to get it right, and the Magento is done by writing modules in OO PHP, at the same time you need to be aware about security permissions, SQL security, PHP application security and so on, so actually using CDN is a great boost to the very important features of such solution.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
