## How to know if I will need a dedicated server?

- posted by: [sk24iam](https://stackexchange.com/users/-1/4660-sk24iam) on 2010-11-05
- tagged: `business`, `hosting`
- score: 5

I am currently building my business on a shared hosting account with a reliable host(hostgator).  When my site goes live, what should I look for that would be an indication that I should switch to a dedicated server.  This is all assuming that I have success with my business and accumulate steady traffic in the future.  


## Answer 16119

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-11-05
- score: 7

I would never put anything more than a small brochure site on shared hosting.  Even if shared hosting would work for your initial load, it does *NOT* scale well. In non-geek-speak: end up on the front page of Digg, watch site fall off the internet and customers see that you are GONE, lose hours if not days while you migrate to a more robust solution.

What *could* have been the event that rocketed your company forward, on shared hosting turns into your death knell.  You've lost the trust of your potential users.

On the other hand, while there are situations in which a startup can benefit from dedicated hosting, they are few and far between and always involve a startup that requires an in-house tech (if not technical founders) who could have answered this question already (so we'll assume that none of those cases are you).

What you should look for is a good VPS (Virtual Private Server) provider.  A VPS gives you all the benefits of a dedicated server: your own reserved CPU cycles, RAM, storage, and I/O, without the need to ever run down to the datacenter and swap out hardware for upgrades (or wait for someone else to do it).  Multiple VPSes run on the same beefy multiprocessor machine at the datacenter, and if your needs spike, you can buy more RAM, storage, I/O, or CPU with a click or two.  There are other advantages to VPSes in terms of manageability as well, but I won't go into them all here.

My preference is for an unmanaged VPS (one on which you have a server upon which you install your OS of choice and any other software you need).  The provider I use is [Linode](http://linode.com) -- they are extremely reliable, fairly priced, and have outstanding service.  (No affiliation, just a very happy customer.)

However, if you lack an in-house tech with server administration experience, you may want to consider a managed VPS (you still get dedicated resources, but your hosting company maintains the server's OS and basics like Apache, PHP, MySQL, email server, etc.).  I have a client or two who use [Media Temple](http://mediatemple.net).  They do managed VPSes very well.  So, while I'm not fond of the inflexibilities that come with a managed service, if I weren't a competent server administrator and no one at my company were, I would consider using them.

**In summary:** with a low-end VPS coming in at about $20/month, there is NO reason not to abandon shared hosting as early in the process as possible, and get onto a good VPS.


## Answer 16115

- posted by: [Janis Peisenieks](https://stackexchange.com/users/-1/5241-janis-peisenieks) on 2010-11-05
- score: 2

These are my suggestions:

 1. Usually every shared hosting has a statistics page. They should have some statistics about how your site is using the available resources. If they are nearly used up - switch.
 2. If your project gets big enough to worry about sending and receiving lots of e-mails, you should think about this. The problem with shared hostings is that more than 1 sites have the same IP. I have had a case, where I couldn't send or receive any e-mails to my server, because someone else on this server had sent out spam earlier. You can battle this, but only to some extent.
 3. Looking at the frequent visitors, or the max online visitors at a time, I would use available RAM as a measurement. I would divide RAM/10 and get the approx number of users the site could take. But this is VERY approximate and could be ***far*** less, if your site does anything other, than server content.
 4. Look for snags in load time. If your site is the only one loading slowly, or doesn't load at all sometimes, its time to switch.

I would personally move to a dedicated server once my average concurrent visitor count reaches 200. This is about the number, that a shared hosting can take.

EDIT:

In light of your previous statement, I would actually consider using cloud hosting for the project, if it's usage could spike rapidly. When in the cloud you don't have to worry about user using too much of the servers resources and crashing it. Rather you just pay the price for the extra compute time and that is it. I would recomend http://www.rackspacecloud.com/ , which is a GREAT service!


## Answer 16191

- posted by: [Jeremy](https://stackexchange.com/users/-1/5184-jeremy) on 2010-11-08
- score: 1

I'd stay on a shared host to start with but get ready to handle an avalanche of new volume by prepping some Amazon EC2 instances and leaving them turned off until you need them. You'd need to couple this with some plan for how to divert traffic there quickly, such as a frame redirect.


## Answer 16123

- posted by: [Gattster](https://stackexchange.com/users/-1/5250-gattster) on 2010-11-05
- score: -1

I would recommend getting a dedicated server from the start. You can get a micro instance of a webserver from Amazon EC2 for < $20 per month. There are other choices besides Amazon, but I haven't priced them. Rackspace is one other option.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
