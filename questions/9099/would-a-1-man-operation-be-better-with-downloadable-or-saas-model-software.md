## Would a 1-man operation be better with downloadable or Saas model software?

- posted by: [UnStartup](https://stackexchange.com/users/-1/2189-unstartup) on 2010-03-10
- tagged: `saas`, `software`, `website`
- score: 8

If you are a 1-man show (to begin with, and want to stay small), would you be better suited to selling downloadable software or would a hosted version be more idea?

With hosted, you don't have to worry too much about product support when it comes to installation etc.

But with hosted you have to worry about uptime.

What do you guys think?

I don't personally know of too many Saas type web applications run by 1 person, so I thought i'd ask here.


## Answer 9114

- posted by: [Bill Paetzke](https://stackexchange.com/users/-1/2694-bill-paetzke) on 2010-03-11
- score: 5

<p><strong>Go SAAS.</strong>  </p>

<p>There are less dependencies on the customer. And deployment is simpler for you.</p>

<p>You must support your product regardless of its format. Support includes FAQ, knowledge base, forums, answering emails, etc.</p>

<p>Read Patrick McKenzie's blog, <a href="http://www.kalzumeus.com/" rel="nofollow">MicroISV on a Shoestring</a>, for more info.  He started a one-man software company in 2006, was profitable in his first month, and is going strong four years later. Originally, his product was a desktop app. Then he converted it to a web app. And he said he greatly favored the web app product experience.  In fact, he wrote an article on <a href="http://www.kalzumeus.com/2009/09/05/desktop-aps-versus-web-apps/" rel="nofollow">why he was done making desktop apps</a>.</p>



## Answer 9110

- posted by: [GRex](https://stackexchange.com/users/-1/2475-grex) on 2010-03-11
- score: 4

It's hard to give a good answer to this one coz it's about what the customers want as opposed to what you want :)


## Answer 9115

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2010-03-11
- score: 3

GRex nailed it.  Do what your target market wants.  Not a single customer will care that you chose the platform because it was easier for you to develop.

Also be aware, most people on here see web-based apps as the solution for all problems, so expect most answers here to be "web app."

Bill Paetzke's answer includes a reference to the McKenzie's interesting article about why he was done with desktop apps.  I read the article, and it always struck me as one very long list of reasons from strictly a developer's point of view of why web apps are better.  Not one mention of the customer point of view until the very end, where he switches roles and speaks as a customer:

*I love desktop applications.  I prefer them to web apps almost any chance I get. You can keep your Google Docs, Excel is superior in almost every way.*

He then says how much his users love desktop applications because of functionality web apps do not have (cut and paste that works, double click files to open them, and so on).

If you take away the bias of talking strictly from a developer point of view, the article does make a strong argument that if you have a choice (if the market will accept it), then make a web app.  I generally agree with that.  So long as we don't redefine problems to fit our solution, we will be ok.

Honestly speaking, I'm happy so many people are focused on web apps.  It leaves huge holes in the markets that will not put up with the many limitations of web apps.


## Answer 9119

- posted by: [Andy Brice](https://stackexchange.com/users/-1/2322-andy-brice) on 2010-03-11
- score: 2

Some problems are best suited to a rich UI, other to a web app. You should pick whichever is the best fit for your product/market/customers. 


## Answer 9109

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2010-03-11
- score: 1

I've worked on both types of applications, and from the support standpoint I prefer web apps. The uptime issues can be mitigated by decent monitoring and notifications, as well as things like automated restarts and a failover setup. With downloadable software it's harder to resolve support problems as you don't control the environment the software runs in and you have limited insight into it.

In my experience, most of the problems with web apps were caused by new releases or insufficient hardware capacity, things that are mostly under your control. If the application has been running for a while, it will most likely continue to run unless there is a hardware failure or a sudden spike in traffic.


## Answer 9121

- posted by: [Mike](https://stackexchange.com/users/-1/2696-mike) on 2010-03-11
- score: 0

You've got a pack of great answers so far...

My only addition to this thread is that I don't think that you can run a successful company with 1 pair of hands only, no matter if you product is SaaS or on-premise.

You can't assume that SaaS doesn't give you problems: you'll just be changing from installation to configuration issues. But you'll always need to give support to your customers.

Is 1 man enough to create a product, launch it and support it? I honestly don't think so.


## Answer 9132

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-03-11
- score: 0

Start with what you are good at. You may need to improve in some areas, but if you've never created a web app, I'd think twice about having my only source of income dependent on your first one. 

A market with tech-savy users may be better for a lone developer because they can handle many problems on their own or with minimal direction (Registry Setting Changes?). Some users are more 9-5, so they don't expect off-hour support.

If you are using a host for a SAAS app that provides maintenance on your site, the "1 man shop" becomes a little more ambiguous.

The distribution and installation can be more trouble on a desktop app, but you don't have to worry "as much" about security, performance implicatons of multi-user environment, webbots & crawlers, backups (you may need to provide a utility for a user), providing data to customers who want to cancel, browser compatability.

Another consideration is going to be your revenue model. Most people accept the recurring payment model for SAAS, but it may take a little more salesmanship on your end to convince a desktop app user to keep paying for a service aggreement. Ease of payment collection can present problems; the market will determine what you can get away with.



## Answer 9379

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-03-19
- score: 0

I suggest what others have also suggested, go with a hosted solution if you are a solo entrepreneur. 

With a hosted solution (SaaS), you are in control of the environment where the software runs so it is easier when troubleshooting and maintaining your application(s). Also, you won't have to worry about offering technical support for people having trouble installing/running your software.

Good luck!


## Answer 27997

- posted by: [Nilesh](https://stackexchange.com/users/-1/6985-nilesh) on 2011-07-26
- score: 0

I recently finished developing a web based application. Right now I am packaging it with a portable webserver so users can use it on their desktop. I have also hosted it online for free usage. I want to go SAAS but not sure if I can handle all the stuff that is needed to maintain the uptime. I believe once you collect payment, there needs to be a SLA and what if the application goes down when the customer is doing something critical.

I will continue doing the desktop downloadable and monitor how the free usage is going. There are so many things needed if you go SAAS.

server Monitoring
automated backups and restore
constant security checks
etc

For desktop or user hosted solution there is no such additional thing.

just my 2c


## Answer 27998

- posted by: [Nick](https://stackexchange.com/users/-1/11400-nick) on 2011-07-26
- score: 0

Definitely go with the SAAS route.

Downloadable software is a deployment nightmare. You have to worry about different operating systems, hardware compatibility, and etc. The combination of things can go wrong is endless. Worst of all, it's impossible to diagnose the problem because most potential customers give up after 1st failure.

I'm running a hybrid of downloadable software and SAAS. My downloadable app allows users to use my webservice. I wish I could go all out "browser-only" because it has been a nightmare especially when you have limited resources.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
