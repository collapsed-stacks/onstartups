## Google App Engine vs Amazon Web Services

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- tagged: `web`, `webdev`
- score: 2

If you were a one developer startup, which service would you pick and why? If the goal is to get to market really fast.

Would you go with GAE and build everything from scratch on Python, and one click deploy?
or pick AWS, setup the server and db, use Rails, and do some admin work?




## Answer 15693

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-10-27
- score: 2

**Hi Johnny, and welcome to this site! :-)**

I'm sorry to be a little pushy on your first question here, but your question is better served elsewhere. As it's mostly about software development technology stack, I think you should try Stackoverflow.com -- here we're more talking about startups, i.e. the company building.

That said, you should be prepared for your question to get a mixed reception. It **is hard to discuss technology platforms in the abstract**, one needs to know the constraints of your specific situation. The fact that you're a one man show is not enough -- for a proper answer we would also need to know what your application *does*, what your expected *growth* looks like, and how experienced you are with Ruby, Python, Java etc. Right now you question is a little like "which is better, space shuttles or supertankers?", to which the only reasonable answer is "well, it depends on what you need.".

My personal pet peeve with regards to development platform is **the developers level of prior experience with the platform in question has by far the greatest impact.** In other words, given a choice between AppEngine and AWS, my first question would be how familiar are the developers with Ruby|Python and with MySQL|"NoSQL type" datastores?


## Answer 15782

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-10-29
- score: 2

Neither!!! Amazon and AppEngine, and Azure all fail.  They are usually more expensive than traditional hosting.  

The word cloud has been overly exploited.
If you build a SAS (software as a service), it is now considered software in the cloud. This is a good thing, but just catchy wording such as WEB 2.0. 

The problem with Amazon, Azure, and Appengine is that they are all very expensive.  They pricing gets a little hard to decifer with compute cycles, storage, and bandwith.

Your best bet is to build a decent server or buy one and colocate it.  
In the long run you will save BIG money.  
I use CalPop.com and have had nothing but a great experience with them. 
You can tell the pricing is great by their outdated web site.

To speed up my site, (a benefit the cloud hosting usually provides) i use a CDN for images, javascripts, and css.  The best service i have found for this (best value and great service) is maxCDN.  I literally called these guys at 2am in the morning and got support.

If you are not up to running your own server, look at Rackspace hosting in the cloud.  They offer virtual hosting, but their infrastructure allows your server to scale multiple machines.  Its more expensive than standard colocation, but they take care of all the management.

Chances are once you have a sver, you wont touch it much.
We only do health checks on our servers, adding hardwawre, and more power.
We sometimes throw another disk in the storage array, and backup (we use drobo) but that is it. 

We save a ton of $$ which is better spent on: development, marketing, beer or strippers. 


## Answer 15769

- posted by: [Jim Blake](https://stackexchange.com/users/-1/4397-jim-blake) on 2010-10-29
- score: 0

<p>In general, I have to agree with everything Jesper said.  </p>

<p>I would also point out that Rails hosting options are becoming easier all the time.  <a href="http://heroku.com" rel="nofollow">Heroku</a> offers a service on top of Amazon EC2 that abstracts away the server administration and makes it the easiest way I have found to get going quickly.  </p>



## Answer 15827

- posted by: [phlai](https://stackexchange.com/users/-1/5133-phlai) on 2010-10-30
- score: 0

What's your expertise in your language? Python or Rails? If you are familiar with Python, then go with Python (Django, Pylons, etc...). If Rails, then go with Ruby on Rails. Because if you want to market fast, it is best that you stick with the language that you familiar with.

My 2 cents though



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
