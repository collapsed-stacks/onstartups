## Hosting for web app

- posted by: [Francisc](https://stackexchange.com/users/-1/12502-francisc) on 2011-08-22
- tagged: `hosting`
- score: 1

Can you recommend a hosting company that is both affordable and very good in order for my startup to have a good always-online image? It's nothing complicated that requires a dedicated server or at least not yet.

Hope this isn't the wrong place for this.

Thank you.


## Answer 29146

- posted by: [kurt.heinrich](https://stackexchange.com/users/-1/4659-kurt-heinrich) on 2011-08-22
- score: 2

Check out [Heroku](http://heroku.com)


## Answer 29196

- posted by: [danmaz74](https://stackexchange.com/users/-1/12083-danmaz74) on 2011-08-23
- score: 1

<p>If the most important thing for you is uptime but you still want to stay on the cheap, my suggestion is to use a node balancer from <a href="http://www.rackspace.com/cloud/cloud_hosting_products/loadbalancers/" rel="nofollow">rackspace</a> and then two (or more) different servers from different cheap providers for your nodes. </p>

<p>This is a good way to get the best uptime for your money, if you can replicate your website or app on more servers.</p>



## Answer 29199

- posted by: [B-Money](https://stackexchange.com/users/-1/12049-b-money) on 2011-08-24
- score: 1

<p>You want a VPS hosting solution.  Something cheap enough to begin with, but that you can scale to Enterprise level in case things go well.  All that without having to move your site to some other location etc.  Check out <a href="http://www.dreamhost.com/r.cgi?25395" rel="nofollow">Dreamhost</a>  / TopNav / Servers --->  Virtual Private Servers</p>



## Answer 29209

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-08-24
- score: 1

Amazon Webservices currently offer one year for free.
http://aws.amazon.com/de/free/

If you don't need the power, I like www.1and1.com very much. 


## Answer 29228

- posted by: [Craig Saboe](https://stackexchange.com/users/-1/12715-craig-saboe) on 2011-08-24
- score: 1

You're going to get a lot of detailed suggestions but I think what you need is something a little higher-level. Like danmaz74 said, uptime is a big factor in figuring out what you need. How critical is your site to your customers? Social networking, while you don't want failures all the time, is not something someone will reject on the basis of one or two 404s or something. You're going to pay for really reliable service, so be really realistic on this. 

Second, what is your site built on? That makes a big difference too. Rails can use Heroku, but they've had a few outages recently due to those Amazon outages recently. There's some pretty good shared hosting providers that will give you pretty high uptime, but you'll hit a pretty solid wall at some point as far as site performance goes. A VPS or something like a Linode box works, but only for Linux-based hosting. 

This decision is really best made by your developer, if that's not you. Otherwise, if you're the developer but not real experienced at this, you're going to have a hard time splitting time between your product and figuring out how to use EC2, Heroku, or Linode - don't prematurely optimize, just get some shared hosting by a decent host and go from there. Your site probably won't jump from 5 to 20,000 visitors a day, so you can scale slowly (and keep your sanity).

If you're still not sure, provide more details and we can help you figure out where you can host and how much in resources you really need to get started.  Hope this helps!


## Answer 29232

- posted by: [Denivic](https://stackexchange.com/users/-1/12387-denivic) on 2011-08-24
- score: 1

I personally use www.hostgator.com very affordable. 


## Answer 29256

- posted by: [Tom](https://stackexchange.com/users/-1/12953-tom) on 2011-08-25
- score: 1

If you know your way around Linux, for cheap and cheerful you can't go wrong with http://prgmr.com - I use them for a few projects, and so far 1GB at $20/month has been working very nicely indeed.


## Answer 29273

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2011-08-26
- score: 1

<p>I am currently using Rackspace's <a href="http://www.rackspace.com/cloud/cloud_hosting_products/servers/" rel="nofollow">Cloud server</a> solution and what I paid every month is less than what I spent on coffee for a month. The great advantage of using this cloud solution is that I can add more power, space and memory at any time without any downtime. It is worth a look!</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
