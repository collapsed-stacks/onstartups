## I'm naive, technically savy, but I can't write a line of code so I just hired a coder to build me a web application

- posted by: [Alex](https://stackexchange.com/users/-1/4951-alex) on 2010-10-22
- tagged: `development`, `hosting`
- score: 1

I'm naive, technically savy, but I can't write a line of code so I just hired a coder to build me a web application.... anyways, I have a few questions about what happens next?!

I have this great idea (its a secret for now ;) and that's why I went on vworker.com to have someone make it. I consider myself an entrepreneur (whatever that means) and predicatbly I'm looking to the future of my site/webapp. Well, let me wallow in fantasy land and ask a few questions.


Scaling- What do all of these bloggers mean when they say you need to prepare for when TechCrunch writes about you and your site goes down? http://www.webhostingpad.com/ says that for $2.00 a month I get unlimited bandwidth? So inst it impossible to go down? Whats the best service out there so this doesnt happen? I want my site to be fast, and besides the fact it needs to be well written, it needs to be hosted with a good service right? 

Amazon Web Services says that you get one year of free service. (http://aws.amazon.com/free/?tag=gmgamzn-20) Netflix just moved to it because its reliable (http://highscalability.com/) - WHAT IS ALL OF THIS?! (lol) thanks....







## Answer 15479

- posted by: [Dan Dyer](https://stackexchange.com/users/-1/4221-dan-dyer) on 2010-10-22
- score: 6

> Scaling- What do all of these bloggers
> mean when they say you need to prepare
> for when TechCrunch writes about you
> and your site goes down?
> http://www.webhostingpad.com/ says
> that for $2.00 a month I get unlimited
> bandwidth?

"Unlimited bandwidth" pretty much never means "unlimited" bandwidth, especially for $2 a month.  I couldn't find the small print on that site but there was an asterisk next to "Unlimited Bandwidth".

> So inst it impossible to go down?

Bandwidth is not the only consideration.  Even if you can get data in and out faster than you'll ever need, you might not be able to process it quickly enough with a single server (really big sites can use hundreds or thousands of servers).  This depends to a large extent on how much work your software does for each request.

If the server gets saturated with requests, subsequent visitors will not get a response.  The user's browser will remain blank or they will get an error message.

Also, with a single server you have single point of failure.  If there is a power failure or hardware failure your site will go down.  You have to decide whether you want to pay extra for redundancy to protect against these problems or accept occasional downtime.


## Answer 15480

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-10-22
- score: 1

First, there is no such thing as **unlimited bandwidth**. That is a marketing ploy a number of web hosting services use. These web hosting services have to **pay** for every bit of bandwith they use. Do you think they will then pass that on to you for free?

Second, you probably don't understand what a shared server is. Your web site and a number of others are all running on the same computer. The computer switches between web sites pretty quickly. This doesn't matter when you have little traffic. But if your traffic suddenly gets large there aren't enough CPU cycles to serve your web pages up to viewers.




## Answer 17171

- posted by: [Michael B](https://stackexchange.com/users/-1/5665-michael-b) on 2010-11-29
- score: 1

I don't mean to shoot you down but if you have never written a line of code I doubt any of these concrete answers will be very meaningful to you. Your question is similar to asking 'what is string theory' and expecting to understand it with a one paragraph answer. I would suggest hiring a consultant. However, consultants are extremely expensive and if you have no knowledge of programming or sysadmin you will have no way of knowing if what the consultant is telling you has any worth.

Making a scalable web site is a huge technical challenge - one that requires deep programming knowledge and deep sysadmin knowledge. This is particularly challenging because it is very hard to find some one that is an expert in both areas (sysadmins are usually not professional programmers and programmers are usually not professional sysadmins). I would say that once a web site becomes successful and profitable, most of the effort goes into keeping it afloat rather than adding new features.

All this being said I wouldn't really worry about it this because your website has about a 0.1% chance of being successful enough to have to worry about these issues - no matter how great your idea actually is. I'm not saying you shouldn't try - just make sure you realise the actual statistics of web sites that get more than 10 frequent users. 

I guess scalability is a kind of catch 22: it's a waste of time thinking about it because you will probably never need to worry about it, but if you do find yourself needing to worry about it you are probably screwed. 


## Answer 15478

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-10-22
- score: 0

Alex, the $2.00 per month is for a shared hosting enviornment.  Your site along with thousands more sits on the same server.  WHen that server has a big load, it crashes and goes down all the sites until it restarts.

If you use dedicated hosting (colocation or virtual colocation) you can get more guarantees on bandwidth.

Cloud hosting with Azure, Rackspace Cloud (My Favorite) and amazon gives your site the ability to grow in the cloud.  What it essentaially means that if your site stored 100tb of data, then you can have that span across several servers.  If you get tons of bandwidth your infrastructure can handle it.

As you can guess they go from least expensive to most.  
what i would look for is a hosting partner that can do all three, Have had nothing but great experience with Rackspace.com, i use them for Exchange hosting also.




## Answer 15485

- posted by: [Jasdeep Singh](https://stackexchange.com/users/-1/4955-jasdeep-singh) on 2010-10-23
- score: 0

At $2 a month, never expect Unlimited Hosting. If you think your idea is really great and it will self propagate i would suggest you invest in Cloud Hosting. rackspace cloud would be the best bet here.. Their services are scalable, so start out with a very basic plan and configuration and then expand or scale as you need...


## Answer 15573

- posted by: [Paul](https://stackexchange.com/users/-1/5003-paul) on 2010-10-26
- score: 0

<p>There's a lot of factors that deal with scalability of a site. Some are covered already, but basically what it comes down to is what is the bottleneck in your system. You won't know that today, most likely, but as other posters have said, bandwidth is but one of them.  Generally, you talk about performance and reliability.</p>

<p>when you talk performance, you talk about bottlenecks in an application, and you're talking about the bandwidth (traffic in and out of the server), but also CPU utilization, memory utilization, disk utilization, as well as I/O load (i.e. if you have to write to a disk faster than it can do so, bad things can happen).</p>

<p>When you talk about reliability, performance has an impact (the more heavily stress parts are, the more likely they are to fail) but you're also talking about more load-agnostic things like mean time between failure of parts, potential for outage due to environmental conditions and so on.</p>

<p>A really great book on the subject, that's accessible to non-coders, is <a href="http://rads.stackoverflow.com/amzn/click/0596102356" rel="nofollow">Building Scalable Websites</a>.</p>

<p>As a startup, though, I think the concerns you're talking about are as common as they are overblown.  No offense to you personally, but the chances of your site having that problem are low enough that you probably shouldn't spend too much money trying to solve it at this stage on the hardware, and spend more time making sure your coder is writing the app in a way that makes it easy to scale (e.g. proper separation of the tiers, etc).  Depending on what kind of contract you have with him, you may want to consider hiring an outside oversight if you can't evaluate his code yourself. </p>

<p>There are no one-click solutions to scalability issues, unfortunately.  AWS does some really great things, as does Google App Engine, as does MS Azure, but none of them make it completely seamless &amp; painless (yet), and all of them are going to be more expensive than your current solution.  A low-cost alternative, if your coder knows Ruby on Rails, is <a href="http://heroku.com/" rel="nofollow">Heroku</a>, which is about as close as I've seen yet to being the seamless solution to scalability, though it's not entirely without warts either.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
