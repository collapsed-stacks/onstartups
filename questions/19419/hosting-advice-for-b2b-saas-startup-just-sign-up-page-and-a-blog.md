## Hosting advice for B2B SaaS Startup - just sign-up page, and a blog

- posted by: [Dhana](https://stackexchange.com/users/-1/6838-dhana) on 2011-01-26
- tagged: `saas`, `hosting`, `b2b`, `blog`
- score: 2

Ours is a B2B SaaS startup (LAMP stack). We are at a very early stage of the Startup. So, we don't need any dedicated hosting at this time. We have planned to use Amazon (not finalized though). In about a month's time we may need a Development environment (maybe on Amazon) for coding and testing and show to early customers.

For now, we want to get the website up and running - just with a sign-up page, and a simple blog - to attract traffic, do some A/B Testing. We want to scale up as we grow.

Can you advise what is the best plan for me ? Amazon EC2 is a good choice for a LAMP B2B SaaS for our current needs and upgrade it as we grow ?


## Answer 19435

- posted by: [John Sjölander](https://stackexchange.com/users/-1/5866-john-sj-lander) on 2011-01-26
- score: 2

<p>There's really no "right" answer for this question. But of course there are a variety of popular choices.</p>

<p>I suggest you <a href="http://jpf.github.com/domain-profiler/ycombinator.html?2010" rel="nofollow">research the preferred hosting choices of Y Combinator startups</a>.</p>

<p>At our company we're all in with Amazon AWS, and we're very happy with the flexibility and stability that has provided for us.</p>

<p>PS. You could also try starting A/B testing right away using <a href="http://www.performable.com/" rel="nofollow">Performable</a> or any other service useful for A/B testing.</p>



## Answer 19441

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-26
- score: 1

<blockquote>
  <p>For now, we want to get the website up and running - just with a sign-up page,</p>
</blockquote>

<p>Right now, just set up a static web page on a 10 USD/month shared webhosting somewhere. Or use a <a href="http://answers.onstartups.com/questions/14921/can-anyone-recommend-a-company-that-hosts-or-sells-landing-page-templates">service like Performable</a> (they seem to be moving away from landing pages ?). And register for Google Webmaster tools, and start getting your website indexed. Then switch to your 'real' hosting platform when you're ready and cancel the shared hosting account.</p>

<blockquote>
  <p>and a simple blog</p>
</blockquote>

<p>Self-hosted Wordpress takes some work. Hosted Wordpress is easy to get started with, but locks you in on the URL structure "blog.company.com" (because you need the separate hostname "blog" to point to the other provider). <a href="http://answers.onstartups.com/questions/7306/seo-dilemma-while-setting-up-blog">Think about SEO,</a> how much energy you'll really invest in blogging, and your in-house sysadmin skills, and make a decision and move on.</p>

<blockquote>
  <p>Amazon EC2 is a good choice for a LAMP B2B SaaS</p>
</blockquote>

<p>Sure it is. As would Linode, Rackspace dedicated servers, Rackspace Cloud, Gigenet servers, and a number of other hosting platforms be. Small- to mid-scale PHP hosting is ubiquitous.</p>

<p>What you should mainly think about is where <strong>you'll choose to split between in-house sysadmin responsibility</strong> (securing servers, patching servers, database administration, data backup), and external <em>fully managed</em> services.</p>

<p>(Nota bene: Amazon has completely different maintenance levels built into their different products. Their hosted load balancer and hosted MySQL are fully managed, but EC2 servers aren't managed by them at all (you must do backups, OS security patching, etc).)</p>



## Answer 19455

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-01-26
- score: 0

<p>I have loved Amazon EC2 however there is a little bit of a learning curve if you aren't comfortable with network admin stuff. If you want a nice front end on top of EC2 for a very low price, check out <a href="http://scalr.net" rel="nofollow">Scalr.net</a>.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
