## How to pick a platform for a startup web 2.0 app?

- posted by: [aryanved](https://stackexchange.com/users/-1/512-aryanved) on 2009-10-12
- tagged: `technology`, `web2.0`, `web`, `application`, `getting-started`
- score: 20

I am looking for recommendatins from the successfull entreprenurs on this forum to advise me on the best software technology platform to develop my web2 webapp on.

The web2 app will potentially be high transaction site

The contenders are:

- J2EE with Postgress
- PHP with MySQL
- Ruby on Rails and MySQL
- PHP with Amazon AWS and SimpleDB
- Microsoft .Net platform

Please help me
Thanks


## Answer 834

- posted by: [James Avery](https://stackexchange.com/users/-1/288-james-avery) on 2009-10-12
- score: 30

It doesn't matter. There are hugely successful companies built with all the technologies you have listed here. Pick the one you know best and build something great.


## Answer 992

- posted by: [raminf](https://stackexchange.com/users/-1/404-raminf) on 2009-10-12
- score: 13

The more important question is how easy is it for you to find developers under each of those technologies in your area? Each option will scale and do the job, but if you get to the point where you need to hire people to work on it then it's important to plan a bit ahead and not box yourself in.

From a technical point of view, one issue to consider is how you're going to deploy the site. If you're going to have dedicated hardware then any of these will work. But if you're starting with a shoe-string budget, then you'll want to pick a technology where you can find cheap and easy hosting services. Also consider how easy it will be to move to another hosting provider once you outgrow your first one.

The cheapest and easiest will be a simple shared hosting site with PHP and MySQL. Just about every hosting service supports this. You may want to use some sort of pseudo object-oriented framework like CakePHP to help write cleaner code. PHP is really easy to get going with but it's also easy to write unreadable spaghetti code.

There are more specialized sites out there that support Rails (like EngineYard and Heroku). These will probably cost more than vanilla PHP/MySQL hosting services but Rails is a nice platform with a lot of community support and a ton of add-on modules to get things up and running quickly.

As for PHP with Amazon AWS and SimpleDB, these fall under the broad category of slice-based virtual hosting services (like Rackspace). You can set up multiple server slices for your DB, application, and web-server and add more as you go to help you scale. You are given a bare OS to put whatever you want on, so you're not really limited to PHP or MySQL. Also, consider that you can mix and match services, so you can put your video files or static images on S3, but your app on, say, Rackspace, or tech support on AWS but your main app somewhere else.

Personally, I'd stay away from J2EE and .Net (let the flamewars begin :-) mostly because there's more choice with the other technologies when it comes to hosting.

You may also want to take a look at Google AppEngine. It uses Python and their own framework, but it's pretty good for quick-n-dirty web-serice development.


## Answer 836

- posted by: [dlynton](https://stackexchange.com/users/-1/482-dlynton) on 2009-10-12
- score: 6

<p>James is right, the framework really doesn't matter. You will probably want to shop around for programmers before you make a decision. The development cost will definitely vary based on which language you choose. For example, vb.net is the most popular language last I checked, so you may get cheaper programmers. However, in my experience you'll find more "amateurish" programmers writing in vb.</p>

<p>My opinion, .net mvc is an excellent platform and very underrated. It's very much like ruby on rails, except you benefit from the maturity and millions of $$s of investment put into the .net framework. The latest version of c# is very terse, and linq makes for an outstanding data layer. Watch Rob Conery's videos on the <a href="http://www.asp.net/learn/mvc-videos/">ecommerce starter kit</a> and by the fourth video you'll see why .net mvc is so awesome.</p>

<ol>
<li>You don't need a paid version of Visual Studio, you can use the free Visual Web Developer.</li>
<li>.net mvc is open source, although you shouldn't have to touch the source to make it work for you.</li>
<li>the .net framework is very mature and widely used in the enterprise. it's object oriented and visual studio is a great IDE</li>
<li>SQL server express is free and very powerful</li>
<li>Like RoR, you have full control of the html output. Unlike asp.net webforms that vomit viewstate and hidden form controls, mvc is mean and lean</li>
<li>built-in support for jquery</li>
</ol>

<p>We have created some really great apps with .net mvc and development time has been much faster than with webforms. However, you will find developers on other platforms that could do the same thing, maybe in the same time period or less. So again, it really doesn't matter except when you decide who you want to hire for the job.</p>

<p>I am biased and cannot give you a fair comparison. We have used PHP and Rails apps before, but have done very little coding with them. Also, I would not give you the same level of endorsement for developing .net webforms apps because the end product is just not as elegant.</p>



## Answer 2612

- posted by: [Kyle Hodgson](https://stackexchange.com/users/-1/1111-kyle-hodgson) on 2009-10-28
- score: 4

I'd like to think that Developer productity is the only thing that matters- but I've seen what happens to the hosting bill in a Microsoft environment when your scale needs suddenly go from 2 servers (1 db 1 web) to 4 (2 db 2 web).  It isn't pretty licensing multiple MSSQL Enterprise servers, so you have to scale up instead of out.  You can go a long way with this, but at a certain point it's way cheaper to scale out - unless you're having to pay for licensing on a flock of web servers. Almost any Open source platform is preferable.

This article has an example of what I'm talking about described nicely.


http://www.codinghorror.com/blog/archives/001195.html


## Answer 842

- posted by: [WebThinker](https://stackexchange.com/users/-1/506-webthinker) on 2009-10-12
- score: 3

Is your idea proven? Or  you wanna launch fast then get feedback, iterate fast? Is there any funding constraint?

I am experienced Java Developer  & Architect. I am confident enough to design and scale any java website. BUT STILL I am targeting ROR for my startup. Because Ruby community is solid so, you will get enough help (on oDesk or eLance ) + cheap hosting + it will be quick to launch app based on Ruby vs Java.

Java hosting is costlier. Simple example - WebLogic, OracleAS or JBoss will need dedicated server ( @100$/month - not powerful server) 

While you can launch your Ruby based app for @10$/month. Once you see traction then you can add more sever etc.

All language/framework are proven to handle high TX but I would like to launch fast to get quick feedback so I can iterate based on user feedback.




## Answer 3463

- posted by: [Wayne M](https://stackexchange.com/users/-1/1455-wayne-m) on 2009-11-11
- score: 3

I'm in the same boat so I have to say first of all that this question is great.  Secondly, it depends on what type of "startup web 2.0 app" you're doing.  There are a ton of great free and commercial solutions out there for Ruby on Rails; for instance if you want a typical subscription-based site, you can buy for $249 a kit that has all of the plumbing taken care of.  Nothing like that exists for any other platform that I'm aware of - if you were to go with .NET MVC, for instance, you would have to write all of the subscription and billing code yourself.

In my case, I'm trying to decide between exactly those two platforms (RoR or ASP.NET MVC).  Some of the things I've considered are:

 * Which I'm more knowledgeable in, since my startup is bootstrapped and I'll be doing all the programming myself
 * Which is the fastest time to market?
 * Which can scale better/quicker with the least cost to me?
 * Which can be set up for the least cost to have a prototype up and working?
 * What are my options for hosting?  Personally I want a "hands off" approach to server configuration since I'm only a half-assed sysadmin and don't want to risk screwing something up by accident.

and finally:

* If my startup fails, what platform will give me the best experience for the future?

Now in my case, I live in an area that is 94% dominated by .NET programming, with about 3% PHP/MySQL and 3% Java.  Virtually nobody here knows or cares about Ruby on Rails.  However, as I'm doing my research between ASP.NET MVC and RoR here's what I've discovered:

* Both platforms are largely similar in their feel.  .NET MVC has much less of the "magic" that Rails has (it's more akin to Python's Django framework than Rails, I think) but all of the power, albeit explicit instead of implicit.
* Rails has more plugins and add-ons available - there are some offerings for .NET MVC (Telerik just released a free set of components, for instance), but the Rails world also moves at lightspeed and the community continually changes what they all do... it's mainly a big game of "follow the leader" where as soon as one prominent Rails developer says "I just found out about X and it's beautiful!" everyone else starts to migrate
* Both platforms have a lot of hosting options.  For the "hands-off" approach I mentioned above, Rails has Heroku and .NET has Windows Azure (although that's still in Beta, I believe?)
* ASP.NET MVC seems like it's a better option **if** you think that you'll eventually want to branch off from web development or expand your application, while Rails is firmly entrenched in web development.
* .NET allows for more software architecture practices than Rails, which tries to keep things "quick and dirty" due to it being "opinionated" software.  This is a blessing and a curse IMHO.

I'm still deciding between the two - the biggest problem I have in deciding is the "plumbing" work.  With Rails, I can spend $249 (that I don't have at the moment) and get the plumbing code taken care of for me already, but it means that I have to wait until I have that money to buy the kit, and even then it might not be entirely what I need.  Also, I repeatedly have issues developing with Rails because I often come to a situation where I know what I want to do, but I'm having trouble fitting it into the constraints of Rails.  With .NET MVC I can start the app the way **I** want it, but all of that yucky plumbing code I need to write myself, instead of focusing on writing my application.

I apologize that this has gotten a bit long-winded, but this question is pretty much one that I was thinking of asking myself :)  I hope my findings help you, and I hope that the answers you receive helps me!  Good luck!


## Answer 868

- posted by: [anthon](https://stackexchange.com/users/-1/238-anthon) on 2009-10-12
- score: 2

I am only a wannabe tech guy, but it was suggested that I go with (and by I, I mean whoever the developers end up being) with the 'stack' with the most incentives to begin with - but, do it properly.

With Sun Startup Essentials and Microsoft Bizspark (only two that come to mind), there are some pretty good inclusions outside of their respective software offerings. These include hosting, advice, support etc.. 

Now the bit I was told is the 'smart' bit is that, like most things, they all have their own proprietary hooks that may make life easier when developing them initially, but can tie you inexplicably to a certaint techology/provider. Apparently the key to not getting stuck is to avoid these until you are mature (as a product/service manufacturer) to decide where you are going to focus your efforts.

Hey they may be wrong - but it seemed to make sense to me... Maybe thats why I am still a wannabe tech guy!


## Answer 31864

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-10-25
- score: 2

**Ruby on Rails**

I understand the premise of "it doesn't matter", and there are some good arguments for it... I just don't agree.

I was a .Net developer that started my own startup around 1 year ago. I decided to switch to Ruby on Rails as a complete novice to it (and to linux and all open source really). I couldn't be happy that I switched, and it is one of the best decisions I made. The key reasons are:

- Development speed is fast with Ruby on Rails, you spend much less time doing plumbing.
- MVC is a great structure that doesn't get as messy as some others as your software gets larger.
- Deployment and hosting is amazingly simple with Heroku, scalability too.
- There is so many good gems out there that take care of big chunks of functionality (authentication, authorisation, file uploads, etc.)
- Great community support
- Cheap hosting (this is a big one, Microsoft licensing is expensive, and gets expensive as you scale, open source technologies have a big advantage here)
- This is a subjective one, but it seems that open source language programmers are more passionate that .Net programmers. I find it easier to find great open source programmers than I do .Net programmers.
- Easy integration with other tools. There are so many good tools to integrate with in a SaaS app (Chargify for subscription billing, New Relic for server monitoring, etc.). There is very good support for Ruby on Rails with these tools, this can save a lot of time.

I don't agree with use the language you know. Learning a new language can be exciting and be a great way to keep you stimulated. It also really isn't that hard to learn a new language, so don't be scared to try.


## Answer 1833

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2009-10-18
- score: 1

<p>I think I would be the only one that would say that this matter. <a href="http://blog.scrum8.com/2009/oct/02/dont-let-your-systems-architecture-fail-you/" rel="nofollow">Don't let your architecture bite you</a>. I would like to say that RoR is a perfect fit for a startup.</p>

<p>Why?</p>

<ol>
<li>It's born from a startup. So it has got great startup mindset in it. No joke.</li>
<li>It's mature. It's been out there for 5 years and has been used by many well know startup.</li>
<li>It's full blown. So you only need to worry about what matters most for your apps.</li>
</ol>

<p>The rest:</p>

<ul>
<li>Java is too expensive. Higher initial investment for hardware, human resources, and too much code to write to do just simple thing. A startup can't afford that.</li>
<li>.NET is the same with Java. Too expensive for initial investment.</li>
<li>PHP is just a language. But many other PHP frameworks are not as good as RoR.</li>
</ul>



## Answer 7543

- posted by: [Abhay Vardhan](https://stackexchange.com/users/-1/2368-abhay-vardhan) on 2010-02-03
- score: 1

My personal recommendations are Ruby on Rails as it is very easy to iterate and experiment with and Google App Engine (python or Java) which provides a good API and hassle free scalability.


## Answer 37409

- posted by: [codejunkie](https://stackexchange.com/users/-1/16219-codejunkie) on 2012-03-21
- score: 1

Here is my answer based on startup i created gkzone.com and real life experience as techie / coder


    J2EE with Postgress   -- too cumbersome and slow for heavy optimisation
    PHP with MySQL        -- perfect as its designed for web 2.0 heck 3.0
    Ruby on Rails and MySQL   -- similiar to PHP but bit less mature and lacks major features PHP has
    PHP with Amazon AWS and SimpleDB -- Amazon AWS too too expensive, stick with simpler solution hosting company+php+mysql+memcache+ if you want noSQL then go for Casandra. 
    Microsoft .Net platform  -- avoid at all cost licensing and upfront and maintenance cost is enormously high! - infact MS have started to offer PHP as it has been beating them in market over ASP.net



## Answer 837

- posted by: [Tony](https://stackexchange.com/users/-1/373-tony) on 2009-10-12
- score: 0

I second the "doesn't matter" point, there _are_ examples of success with all of the technologies. Scalability is in the architecture, not the compiler/interpreter -- if PHP or Ruby runs slightly slower than J2EE, then throw a few more servers into the cluster; AWS makes it trivial.

You should go with the tools that will let you write the best quality of code, with the least effort.

[edit] We've had some amazing productivity with the use of Ruby on Rails (but fumbled with PHP when trying to integrate FOSS projects). Though you could certainly find developers who are passionate about either of the technologies.


## Answer 863

- posted by: [pbreit](https://stackexchange.com/users/-1/239-pbreit) on 2009-10-12
- score: 0

I second "it doesn't matter" and that if you are going to partner with a co-founder, they might make the decision for you. PHP, Perl and Ruby on Rails are all adequate with MySQL.


## Answer 982

- posted by: [user574](https://stackexchange.com/users/-1/574-user574) on 2009-10-12
- score: 0

I have to third the "it doesn't matter" answer. You need to select the one that you know and can develop in. If you are new, then perhaps you need to find some partners to help with the technology. They will have a bias and will want to go a certain direction.

Personally, I am a .Net head and would never choose any open source or Linux related products (just my opinion). Too  many issues installing, configuring and maintaining the products. 

Rick


## Answer 1013

- posted by: [odmarkj](https://stackexchange.com/users/-1/484-odmarkj) on 2009-10-12
- score: 0

As a company, we hire for talent and then fit technology into that. For example, we were a PHP and MYSQL only company for over two years.

We met an individual who had a killer interview and came highly recommended from our chairman. Problem was, he was a Ruby on Rails guy.

In the end, our problem was focusing too much on technology. Luckily we realized our mistake and changed our focus to finding talent and working with their preferred technology.


## Answer 1803

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-18
- score: 0

I think you would want to choose whatever technology that will get your product out quicker.
so I would use RoR or python.

but stay away from J2EE.
J2EE is too heavyweight. Takes too long to develop. Its great for consultants because it means more billable hours but not good for nimble startups.




## Answer 1841

- posted by: [Davewasthere](https://stackexchange.com/users/-1/672-davewasthere) on 2009-10-18
- score: 0

My current recommendation would be to use django and the google app engine for hosting. Either that or Amazon AWS.

(And to put in context, I'm a Microsoft .Net developer)

Main reason I'd consider Python/Django/Google App engine would be that for starters, it's free. It's massively scalable. And Python/Django look incredible easy to pick up.

But in reality, you should be able to develop on almost any platform. Pick the one you'll be most productive in, and use that. If it gets to a point where you're hitting a limitation of the platform, you should be rolling in green that switching shouldn't be a problem.

That said, a lot will depend what you mean by a high transaction site. Some more information wouldn't hurt. 


## Answer 1845

- posted by: [Nathan Kontny](https://stackexchange.com/users/-1/973-nathan-kontny) on 2009-10-18
- score: 0

<p>I'm a bit more on the side of picking something does matter.  First, it's not just picking a language.  You are also probably getting in bed right away with a framework like Django or Rails or Grails or something.  And that framework choice could bite you if it's not going to be around for the long haul.  With Django/Rails that's not likely going to be the case.  But I've seen crazy hyped frameworks in the past die off and leave their developers struggling to port their application to new frameworks.  </p>

<p>Take Keel for Java as an example. I built someone's new business around this thing.  It was an extremely popular Java framework.  Promised a ton of the benefits of something like Rails.  But it's gone now.  The business owners struggled then to find people to work on it.  Even though it was Java and any decent Java developer could work through the thing, the framework definitely added overhead to mastering developing on it. </p>

<p>With our business now, we picked Rails over 4 years ago, and that was a successful pick given it was still pretty immature when we picked it.  So be careful with that choice as well.  </p>

<p>Also back to the pure language argument, <a href="http://www.paulgraham.com/avg.html" rel="nofollow">Paul Graham shares a different perspective than the "it doesn't matter, pick what your comfortable with" argument.</a> </p>



## Answer 2618

- posted by: [Denis Hennessy](https://stackexchange.com/users/-1/311-denis-hennessy) on 2009-10-28
- score: 0

I'm going to buck the trend here and say that the right choice DOES MATTER. The languages, and more importantly the frameworks, you mention all have significant trade-offs that you should properly consider before making a decision. In particular:

 - Ease of getting product launched and ease of iterating once launched
 - Ability to scale if product really takes off
 - Availability of talented developers
 - Existing codebase (may not apply)

I'm assuming you're bringing in a technical partner to help build your app - he should be able to properly evaluate the alternatives w.r.t. your application. Without knowing anything about it, my general advice is:

 - Give Ruby on Rails a try - language is clean and framework enables rapid development.
 - Avoid Java - too heavy.
 - Avoid .NET - the licensing costs will come back to bite you.
 - Avoid PHP - tends to encourage poorly structured code.





## Answer 2630

- posted by: [Duncan Wilcox](https://stackexchange.com/users/-1/869-duncan-wilcox) on 2009-10-28
- score: 0

As a programmer my advice is find a kickass programmer, and let him/her decide.

There are many choices and tradeoffs depending on what you're doing, and each programmer has experience and passion with different technologies, and will be 10x as productive in the environment they prefer.


## Answer 3135

- posted by: [user1220](https://stackexchange.com/users/-1/1220-user1220) on 2009-11-05
- score: 0

*This might not be an answer but might be another question on the same context.*

Being a Microsoft .NET junkie for most of the day (at work) I've been trying to use some open source alternatives for the side projects, aka PHP/CodeIgniter/jQuery/MySQL. The ultimate reason for going with the open source stack is so I can find some cheap web hosts with less commitments (got hurt with **trying** an ASP.NET app - didn't take off - paid the rest of the hosting contract $$$$ for nothing). 

CodeIgniter was not that hard to pick up but being so used to the .NET platform it's kind of not encouraging much to get things done end-to-end with PHP/CodeIgniter. Always running into one thing or the other issues and spending most of the time trying to figure out how to resolve the issue. Would have been with the .NET stack? Things would have been a lot different. Since I know the platform in-and-out (I'll claim that loosely) I would have deployed the app by now and feel confident about it.

My question to you is, **if you are not sure if your idea will take off what platform would you recommend that can leave us with limited $$$ loss in case if the idea doesn't take off?**




## Answer 3183

- posted by: [Jeremy French](https://stackexchange.com/users/-1/1349-jeremy-french) on 2009-11-06
- score: 0

<p>I admit that I have a huge bias in answering something like this, but I would say that you should go with a higher level framework. Something like <a href="http://drupal.org/" rel="nofollow">Drupal</a>. This gives you a lot for free: Content editing, user management, templating engine.  One of the most talented developers I know has spent a lot of time at start ups re inventing the wheel to implement these features over and over again. </p>

<p>It means that you can spend time on focusing on focusing on your business plan than building a web site. </p>

<p>Eventually you may find that you outgrow the technology and that it is holding you back, but by that time you should have built your business and can spend time on building out a bespoke architecture. </p>

<p>I would also note that you should be weary of trying to build a super scalable system right from the off. You can get quite a long way by just throwing hardware at the problem. And you can fix bottlenecks when and where you find them. Whatever technology you choose focus on features and usability, some developers love to (try and) build an amazingly archetectured system when given a green field but they should focus on building the business. Your users won’t care so long as things work. </p>



## Answer 3184

- posted by: [Tim Post](https://stackexchange.com/users/-1/1343-tim-post) on 2009-11-06
- score: 0

This can be done in two steps:

 - Hire programmers with great references and demonstrated skills
 - Use whatever they want to go with

Further elaboration is kind of pointless, in this case :) Sorry for the short answer.


## Answer 3186

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-06
- score: 0

It is important to make a distinguish between the programming language, the framework, development methodology and the people in your team. 

I would say language is least important. Basically the same end result can be archived in any language be it Ruby, PHP, Java or C#. Trying to ask people to pick will only start a flame war, consider them all equal. They can also all scale, in terms of handling volumes of traffic, equally well.

What is more important than language choice is the gains that can be made from selecting a good framework for any given language. For example a popular framework methodology is MVC (Model View Controller). 

Some MVC frameworks include RubyOnRails, CakePHP, Struts (Java), and I believe Microsoft have just released a MVC framework for C#/.NET.

The long term benefits of using an MVC framework which allows for separation of concerns - business logic, querying of data and presentation/User Interface - is essential. Any web developer worth his/her salt will use an MVC (or similar) framework for their respective language. This choice will help prevent your developer and designer stepping on each other toes.  

More important than the framework of choice is the development methodology, you will want to look in to Agile methodology. Agile is a banner for a method of developing an application in incremental steps where you release improvements/features on a regular basis based on feedback. You **deliver the features which hold the most value to your end users first**.

Linked in closely to this are development best practices, is your development team going to be producing documentation, writing tests, using version control, deploying to a staging area?

But most important are the people you choose to hire. It is the people in your team not the technologies that will ultimately help your succeed or otherwise. I would suggest hiring the best, not the least expensive from the beginning, it will be less expensive in the long run and give you a better chance of success. Work together to develop the features which will deliver the most value to your end users with your starting capital. 


## Answer 3921

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-21
- score: 0

I'm going with the answer, "the one you already know."  Mine is the case that my partner already had the ability in Java so that is what we went with.  For us, the product was more important as the platform is already proven.  Only time will tell if we were right.


## Answer 3979

- posted by: [Dave Ambrose](https://stackexchange.com/users/-1/1394-dave-ambrose) on 2009-11-22
- score: 0


We're going through the same technology discussion in my startup and I'm going to cast my vote with "it matters". This is a case where you want to choose your ruts carefully, because you're going to be in them for a while. 

There are three things to consider:

 1. Your business needs; what makes your business unique?
 2. How does a proposed platform (language and supporting software) serve those needs?
 3. How does the culture that's grown up around the platform or programming language serve your business needs?

I've done a lot of work in the finance and insurance industries. Good companies in those fields tend to use Java. Why? The language *and the programming culture surrounding it* tend to emphasize security, reliability and correct execution under all conceivable circumstances. Reliability is paramount in any kind of financial system. In this case, the primary goal is met, and the overhead in labor and hardware is a necessary cost of doing business. 

Our startup is a completely different animal. We don't need security so much as we need the ability to get something on the air quickly, and still have enough richness that we can add new functionality without running out of horsepower in the platform. 

It's a delicate balance between startup costs and headroom. If your company's successful, you'll hit that ceiling. Once you exhaust your platform, you either lose your ability to evolve quickly, or have to swallow the costs of refactoring, or worse yet, reimplementing.

I've seen this technology ceiling in every successful small company I've worked for. That's when they usually go up for sale to a larger company. 


## Answer 7251

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-28
- score: 0

Initial cost for developing in .NET isn't an issue at all, there is MicroSoft BizSpark programme where you get free licences to all their fully-featured softwares for 3 years, after 3 years you wil still have licences to those softwares you downloaded during that period.

For my startup I chose .NET framework because I have 5 years experience developing in it, I like working on it, and I am more productive when working on it. I could have easily used PHP or Java, but I don't enjoy working with those frameworks.


## Answer 8537

- posted by: [rabble](https://stackexchange.com/users/-1/2673-rabble) on 2010-02-25
- score: 0

This is a complicated issue.

For example, if you are doing an application which has a heavy geo / location aspect to it, then Django and Postgis is the only viable option. 

If you're doing something with heavy legacy integration then perhaps Java would make sense because although it's heavy and slow, it integrates well with SOAP legacy systems.

We just had a client switch from django to rails because they felt like the rails community cared more about user experience and the front end of the application.

If you're concerned about getting a broad selection of developers for cheap, go with PHP. 


## Answer 8602

- posted by: [Mike](https://stackexchange.com/users/-1/2696-mike) on 2010-02-26
- score: 0

<p>You can also take a look at the Agile Platform by OutSystems.</p>

<p>You can build, deploy and maintain rich web apps fairly easily. The best part of it is the ease of maintenance and change. </p>

<p>The website www.fly.com (a travel search engine) was built with the platform, and has a huge daily load of visitors and search queries, so I'd say your load and scalability concerns are covered. </p>

<p>You can <a href="http://www.outsystems.com/download" rel="nofollow">download the Agile Platform here</a> for free, and <a href="http://www.outsystems.com/demos" rel="nofollow">see a bunch of demos here</a> </p>



## Answer 8626

- posted by: [David](https://stackexchange.com/users/-1/2684-david) on 2010-02-27
- score: 0

You could consider using Adobe Flex as well. See the discussion on http://stackoverflow.com/questions/2258876/could-facebook-have-been-implemented-in-adobe-flex




## Answer 8627

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2010-02-27
- score: 0

**Framework does matter**

I assume you don't have any expertise on any of this anyway so why choose one randomly? If you are expert or really good in of the options go for it, don't think twice. If you are not my comments:

If it's a classical bunch of CRUD + AJAX stuff and if you can find RoR developers go for it, because it'll be much faster others (assuming developers are experienced in in RoR).

Don't go for PHP, it's dying not that agile unless you got some really really good developers. Lots of things is painful, It's not suitable for unit test, new versions breaking old stuff , there are performance issues, not suitable for big projects etc. Just stay away.

Don't go for J2EE, that's designed for Enterprise rubbish, even for the smallest task you have to spend ages to develop, deploy and test. Also J2EE developers are mostly in this mindset as well, so stay clear.

.NET is not too bad but license cost is high, development is not as agile as RoR, components are expensive, however if you are going to build a big system and need performance then .NET (*ASP.NET MVC not the old way*) is your guy. It's easy to find good developers as well, they are all over the place.








## Answer 12665

- posted by: [Dean Hamton](https://stackexchange.com/users/-1/3661-dean-hamton) on 2010-07-11
- score: 0

**My 2 cents**

I am not a programmer but I based the choice on price per programmer. I found PHP is widely available and not expensive. We selected Google Saas platform and found it was not up to our standards, then switched to Amazon SimpleDB and found many problems problems. So now we have a mix op Amazon AWS servers with MySQL and SimpleDB and S3 as well. 

We work with storing billions or records (analytics tool) so SimpleDB is good for that. But analyzing something became a problem there (as I understood).


## Answer 18255

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-27
- score: 0

I come from a strong .NET background but ended up doing all my side projects in PHP. Call me weirdo! but coupled with a decent MVC framework (like CodeIgniter) I don't see PHP as a messy language as it used to be. In fact I started loving coding in CodeIgniter more and more. For almost all the development issues I have faced PHP and CodeIgniter stood up the challenge and got me going. The best part is the simple deployment overhead, I can almost carry my web apps all around in a thumb drive and get it to working on any machine with a web and database server. It's fitting into my development lifestyle and I'm cool with it. Give PHP/CodeIgniter a try!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
