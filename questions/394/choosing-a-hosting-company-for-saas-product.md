## Choosing a Hosting Company for SaaS Product

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-10
- tagged: `hosting`
- score: 5

I am building a SaaS product and am evaluating hosting providers. Currently I have three subscription paid websites hosted at GoDaddy. My new application will be quite a bit beefier than the existing ones. Although I’m happy with GoDaddy I am open to other suggestions. I don’t intend to bring hosting in-house anytime in the near future (or probably ever).

My biggest concerns are:

- Ability to easily restore database when things go wrong
- Start small and expand as client-base increases
- Responsive support

The SaaS is product is PHP & MySQL based. 

Any suggestions?


## Answer 408

- posted by: [Yoav Shapira](https://stackexchange.com/users/-1/310-yoav-shapira) on 2009-10-10
- score: 2

I'd give Amazon Elastic Cloud (EC2) a shot.  You can start with one box for pennies a month, and grow as you need.  The services are easy to use and set up.  Billing and such is trivial.  You don't need any contracts.  There's no support, however.  It's all on you.

If you do want a more traditional hosted offering, Contegix is awesome: http://www.contegix.com/.  Their support is excellent, their prices good.


## Answer 549

- posted by: [Peldi Guilizzoni](https://stackexchange.com/users/-1/215-peldi-guilizzoni) on 2009-10-10
- score: 2

I am very happy with Slicehost. Their support is top-notch, backups are a breeze to recover, you get root access etc.

The best part though is their help site: http://articles.slicehost.com - the PickledOnion articles are made of awesome, he makes even the driest topics accessible and fun. Makes you feel smart! :)


## Answer 410

- posted by: [Mark Beadles](https://stackexchange.com/users/-1/296-mark-beadles) on 2009-10-10
- score: 1

You need to first figure out what your hosting requirements and future projections are.

 - How many concurrent users do you need to serve (as **blekkzor** said)? Now and projected?
 - How many requests does each user make during a session?
 - How much server and database processing do you expect per session? 
 - Are your users local? National? International? If international, what regions?
 - Do you anticipate the need for specialized web performance and caching?
 - Are you going to be streaming audio? Video?

Unless your application requires very specialized hosting, which is doesn't sound like, nowadays there is really *no* reason to think about doing your own hosting. 

Once you have your set of requirements, just shop around. Web hosting has become commoditized, so you should be able to easily compare vendors apples-to-apples.

**One bit of advice that I've found useful is to strike up a relationship with a web hosting provider local to you. Most metro areas have a selection of reputable providers with decent hosting packages. You're likely to get much better service if you've met the people who are providing your services than if you're just an account number at GoDaddy, and you may also find synergies.**

Best of luck.


## Answer 430

- posted by: [Ade Olonoh](https://stackexchange.com/users/-1/317-ade-olonoh) on 2009-10-10
- score: 1

Generally speaking, you need something a lot more robust and reliable than shared hosting for a good SaaS product.  For not *that* much more you'll get a huge performance boost, and you're not susceptible to the load that other customers put on the server.

In addition to S3, check out cloud providers like rackspacecloud.com, joyent.com, slicehost.com and bluelock.com.

I'd also highly suggest looking at a dedicated server.  If you don't have sys admin resources, there are plenty of good managed hosting options.  Check out rackspace.com and peer1.com where an entry-level managed server is going to cost at least $200/mo.



## Answer 611

- posted by: [tequilatango](https://stackexchange.com/users/-1/219-tequilatango) on 2009-10-11
- score: 1

<p>I investigated <a href="http://dirtyaura.org/blog/2009/09/22/programmer-friendly-virtual-private-server-hosts/" rel="nofollow">three VPS hosts</a> a couple of weeks ago. I ended up choosing Slicehost, but Linode and prgmr.com seem to be fine choices too, if you want start small and expand from there. All of them seem to have a good responsive support.</p>



## Answer 398

- posted by: [blekkzor](https://stackexchange.com/users/-1/281-blekkzor) on 2009-10-10
- score: 0

More information could be useful, though you should stay away from any unlimited offers or 5TB bandwidth for 10$.

How many users do you expect concurrently on your website? Are the web pages very sql intensive?


## Answer 411

- posted by: [pclark](https://stackexchange.com/users/-1/303-pclark) on 2009-10-10
- score: 0

We've found Linode to rock. Don't confuse yourself into thinking "enterprise software" requires different hosting than everyone else. 


## Answer 423

- posted by: [danpickett](https://stackexchange.com/users/-1/13-danpickett) on 2009-10-10
- score: 0

I use Linode and I've heard good things about http://prgmr.com/xen/ (inexpensive).

EC2 has a barrier to entry that's significant - there's a lot of infrastructure to set up and and the initial costs are pretty hefty.


## Answer 428

- posted by: [Corey Maass](https://stackexchange.com/users/-1/325-corey-maass) on 2009-10-10
- score: 0

I can't recommend Wiredtree.com high enough. Their support is so good I've sent them cupcakes. I'm not kidding.


## Answer 443

- posted by: [Brian Armstrong](https://stackexchange.com/users/-1/332-brian-armstrong) on 2009-10-10
- score: 0

<p>I like the idea of cloud computing (Amazon EC2) but there are cheaper options for a startup I think.</p>

<p>I prefer to start with a VPS.</p>

<p>I've had great success with SliceHost.com on several startups (heard good things about linode.com too, slightly less expensive).  You can start this way for about $20 per month.</p>

<p>For the ultimate bootstrapper: if you are doing a ruby on rails app, my favorite is Heroku.com to get up and running for FREE!  Yes, rails hosting for free (one rails instance works fine for low traffic).  I use this if I just want to throw up an idea.  I launched <a href="http://BuyersVote.com" rel="nofollow">http://BuyersVote.com</a> this way for a total startup cost of $7.95 (the domain name).</p>



## Answer 464

- posted by: [JeremiahLee](https://stackexchange.com/users/-1/352-jeremiahlee) on 2009-10-10
- score: 0

Joyent has served me well, but I'm considering Rackspace Cloud (Mosso) for future projects because it's cheaper and has better free support.


## Answer 559

- posted by: [user287](https://stackexchange.com/users/-1/287-user287) on 2009-10-10
- score: 0

see http://news.ycombinator.com/item?id=109632


## Answer 601

- posted by: [anthon](https://stackexchange.com/users/-1/238-anthon) on 2009-10-11
- score: 0

I am not sure what your developing in/for but Microsoft's Bizspark offering has deals with various hosting partners. See http://www.microsoftstartupzone.com/BizSpark/Pages/What_Do_I_Get.aspx for details.

Sun's Startup Essentials has a similar offering from memory.


## Answer 613

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-11
- score: 0

<p>Check out <a href="http://microsoft.com/azure" rel="nofollow">Microsoft Azure</a>. </p>

<p>Azure lacks many of the shortfall that Amazon EC2 and Google offer. Azure will also host apps written in Java, Ruby, Python, Lamp, or whatever.</p>



## Answer 679

- posted by: [hadi](https://stackexchange.com/users/-1/450-hadi) on 2009-10-11
- score: 0

I find having my own server a lot better than the cloud platform. You could start off by having a VPS which you can get for around $30 & eventually migrate to a Full Dedicated Server.

My experiences have been good with (google up for them I'm unable to post links) -

LiquidWeb  <br/>
ResellerZoom

You're running a SaaS based paid product for customers where you would want higher control on the performance & behavior of the server, my thumbs go up for vps / dedicated server with managed hosting (if you don't have server admin)


## Answer 680

- posted by: [MartinHN](https://stackexchange.com/users/-1/259-martinhn) on 2009-10-11
- score: 0

I'd go with someone like Rackspace. They've got datacenters in both US an Europe. It's managed hosting. When things go wrong, they're there to make things good. Whether that being restoring a database, server, disk whatever.


## Answer 32141

- posted by: [Nilesh](https://stackexchange.com/users/-1/6985-nilesh) on 2011-11-01
- score: 0

I would add servint to the list as well. It starts at $50 but it provides better console for management. I am looking at linode but looks like too much to handle for a newbie. If you cannot handle all the admin,security stuff then hire someone or go with a managed service like servint.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
