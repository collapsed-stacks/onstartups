## Buying a low-budget server. What is important ? High traffic?

- posted by: [Martin](https://stackexchange.com/users/-1/15579-martin) on 2012-01-12
- tagged: `startup-costs`, `server`
- score: 4

I need a server that can handle a lot of traffic for my iPhone app. I am just a student, so affording a server in the thousands is rather not an option. How can I handle that ? Can I rent servers ? How much are they usually ? Or should I buy one with low storage and upgrade as the app does better and better ?


## Answer 34751

- posted by: [Paul Cezanne](https://stackexchange.com/users/-1/14795-paul-cezanne) on 2012-01-12
- score: 9

<p>You might want to consider not buying or even renting a server. I'm in a similar position and I've gone with <a href="http://aws.amazon.com/">Amazon Web Services</a>. My monthly bills are right around $50-$60/month. My code isn't tied to them, it can run on any Java EE 6 application server. So far I've been pretty happy.</p>

<p>(I've answered a similar question before and was downvoted. If you want to down vote me here, at least tell me why. Thanks!)</p>



## Answer 34771

- posted by: [Shauna](https://stackexchange.com/users/-1/11273-shauna) on 2012-01-12
- score: 3

The way your question is worded, it seems that you think that a web server is always a physical machine, much like the computer you probably posted this question on. The fact is, quite often, they're not.

A lot of companies, especially startups, as well as individuals, pick up *virtual private servers*. Virtual private servers are fully-functioning servers that the customer has full control over, but they share hardware with other virtual private server instances. If you've ever used VMWare, VirtualBox, or Parallels, you're already familiar with virtualization. Cloud solutions, such as AWS, are very similar.

Both of these solutions provide you with full control to what you want (as long as it's not illegal, of course), and provide you with the same experience that you would have if your server took up the whole machine.

One of the companies I work with uses Rackspace (they have a European sector now), and has a not-quite-bottom spec'd (768MB RAM, 30GB hard drive) server for about $70USD/month. For what you're doing, you can probably get away with their smallest server, or a step up, for a while, which runs around $10-$20USD/month (I do API/web support development for mobile apps, and we have about 8-10 apps running and active with some supporting a few thousand users each).


## Answer 34752

- posted by: [Angelo Neuschitzer](https://stackexchange.com/users/-1/15578-angelo-neuschitzer) on 2012-01-12
- score: 0

Renting a server is not expensive.
I would suggest you rent a vServer, they come as cheap as 5 EUR (although that won't do much good to you) and what you learn from setting up and maintaining one you can still use when upgrading.

I googled 'server mieten österreich' and came up with https://www.internex.at/de/server/root-vserver/root-vserver-vps.php they have offers from 20 EUR up.

Myself I live in Germany and have my Servers at Strato, so thats not the big problem anyway.

If you are not able to administer your server yourself drop me a line, I know some people in Austria who will be willing to do that for you (and won't cost you a fortune if you want to do something commercially).


## Answer 34772

- posted by: [luckytaxi](https://stackexchange.com/users/-1/15584-luckytaxi) on 2012-01-13
- score: 0

I use linode.com for my new app. Works just fine.


## Answer 34774

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-01-13
- score: 0

If you are using PHP as backend platform, you can try to start with https://phpfog.com/pricing
They have a free plan which should help you the first time.

vServers might be a good choice, as already suggested.

I can confirm the already mentioned Strato are good. 
So is 1und1.de
I have also heard http://www.alvotech.de/ is nice, but not tried them myself. 

If you don't need a complete server I can recommend bytecamp.net

It might be good to know how much traffic you are expecting and which backend technology you are using. EC2 has already been mentioned, but there is also Cloudbees, Rackspace and others.


## Answer 34878

- posted by: [Scott](https://stackexchange.com/users/-1/4312-scott) on 2012-01-16
- score: 0

<p>You could also try <a href="http://www.heroku.com/" rel="nofollow">Heroku</a>.  They offer free plans on shared servers.  Then you can pay as you grow.  It's where I deploy my prototypes and test sites.</p>



## Answer 34950

- posted by: [Herr K](https://stackexchange.com/users/-1/3855-herr-k) on 2012-01-18
- score: 0

<p>The most important things when renting servers is, <strong>SERVER MANAGEMENT</strong>.  </p>

<p>I suppose you are new to this kind of things therefor i would recommend you to rent a MANAGED VPS server and NEVER rent an unmanaged server (especially if you have none linux knowledge).  </p>

<p>I would go for something like <a href="http://www.site5.com" rel="nofollow">Site5</a>.<br>
After that i would suggest <a href="http://www.rapidswitch.com" rel="nofollow">RapidSwitch</a>.</p>



## Answer 34957

- posted by: [Sid](https://stackexchange.com/users/-1/13800-sid) on 2012-01-18
- score: 0

Depending on your traffic requirement and need to customize, you could get away with a shared server (Linux/PHP or Windows/ASP.NET). This will typically be under $10/month

If you need more control and need to "own" the entire server, I'd recommend Amazon Web Service's EC2. AWS EC2 allows you to fire up virtual machines in the cloud. There can be in the $40-$100+ range depending on what resources (CPU,memory,bandwidth etc) your Virtual Machines consume. Here, you'd own the virtual machine but you pay to rent the physical machine that runs your virtual machine.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
