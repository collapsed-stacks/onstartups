## Software start-ups: do you outsource your network admin?

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2009-10-10
- tagged: `strategy`, `outsourcing`, `recruiting`
- score: 3

For business, I tend to outsource a lot of things that I am more than capable of doing. Take, for example, office cleaning. Okay, I'm a slob, so in reality, it would never get done... but you get my point.

But for the life of me, I can't seem to outsource network administration. We're not big enough to have a full-time network guy, but stuff like setting up servers, IP phones, workstations, etc. tend to fall on myself or a developer.

Is this a good use of our time? Should I just suck it up and retain a network admin company?


## Answer 677

- posted by: [Neil Davidson](https://stackexchange.com/users/-1/210-neil-davidson) on 2009-10-11
- score: 4

Outsource stuff if it:

* just needs to happen
* you don't need to be better at than your competition to succeed
* is standard (ie what you need isn't dramatically different to what anybody else does)
* is likely to work well enough if somebody else does it





## Answer 465

- posted by: [pclark](https://stackexchange.com/users/-1/303-pclark) on 2009-10-10
- score: 1

Depends how many people. If you're under 5 people there is no reason why everything isn't in the cloud. We use this stuff:

Google Apps
Jira
Confluence
GitHub
Dropbox

Active Directory? VPN? Why? 


## Answer 501

- posted by: [Alex Balashov](https://stackexchange.com/users/-1/371-alex-balashov) on 2009-10-10
- score: 1

It really depends on what the core competency and product focus of your startup is.  

We, for example, are a VoIP service delivery platform engineering consultancy hoping to evolve into a software vendor (consulting is a funding strategy).  We work a lot with servers, IP networks, and other operational/system/infrastructure stuff anyway;  it's a fairly logical extension of our knowledge pool to run our own facilities and not spend the cash when we already pay the fixed costs on people with know-how to do that.

If, on the other hand, you are a web-application oriented company without much background in such areas, or not enough background to do it economically, then it might make sense.


## Answer 587

- posted by: [warp](https://stackexchange.com/users/-1/201-warp) on 2009-10-10
- score: 1

I used to work part-time as a system/network administrator when I was in college.  Have you considered looking for students who could work part-time for you?  (It's fairly common for students here in the Netherlands to have part-time jobs to help pay for a decent education, no Idea how common this is in your area).


## Answer 463

- posted by: [DThrasher](https://stackexchange.com/users/-1/326-dthrasher) on 2009-10-10
- score: 0

We face the same problem in our two-person startup. It's a terrible waste of time to do our own network administration, but we haven't found a good way to outsource it.

The best we've been able to do is use Google Apps for email and calendar sharing, rather than run our own Microsoft Exchange servers. But that still leaves us doing Active Directory administration and VPN services ourselves.


## Answer 467

- posted by: [Micah](https://stackexchange.com/users/-1/284-micah) on 2009-10-10
- score: 0

<p>Absolutely outsource this.  If you look a little, you should be able to find a hosting company that will do much of the server sysadmin stuff for you.</p>

<p>In my case, we're a Ruby on Rails only shop, and we found that BlueBox Group handles quite a bit of the server setup (Apache settings, iptables, installing packages, general stuff).  It saves us a ton of time.  We can usually stumble our way through it, but it's so much easier to just submit a support ticket.</p>

<p>I <a href="http://blog.aisleten.com/2009/06/08/ruby-on-rails-hosting-with-blue-box-group/" rel="nofollow">wrote a review</a> of BlueBox specifically.  However, I'm sure there are other such hosts for other platforms/languages.</p>



## Answer 499

- posted by: [Michael Trafton](https://stackexchange.com/users/-1/19-michael-trafton) on 2009-10-10
- score: 0

At Blue Fish, we are a software development company, and we do outsource our network admin. Our original network was a mish-mash of windows servers that we built ourselves, and they never had the right security patches or service packs. We started out maintaining these servers ourselves (developers did it whenever they got around to it). Eventually, we hired a full-time IT guy, but when he left the company we hired a local IT services firm to do it. The difference was night and day. Now we have a state of the art network powered by linux servers and VMWare - we can snapshot our development environments with each software release.  The price of the local IT company is actually less than an in-house IT guy, and the quality is much better.


## Answer 534

- posted by: [Denis Hennessy](https://stackexchange.com/users/-1/311-denis-hennessy) on 2009-10-10
- score: 0

The important question is not whether you should pay an external services company to manage your network versus do the same work yourself.  The question is: if you're a startup, why are you making decisions on infrastructure which requires that much work to maintain?

My recommendation: First, use as many cloud services as you can:

 - Google Apps for email and document sharing (ignore the paid plan - it's free)
 - Dropbox (getdropbox.com) for general file sharing (~ $10/month)
 - Google Voice or Skype for telephony (~$10-$50/month depending on volume)

Second: Don't buy anything that requires management (in particular, don't run any servers). If you want shared printers, pick a network attached printer with no security. If you want shared files in an office, buy a nas unit like the netgear readynas. Buy any consumer access point and network switch. If anything fails, just bin it and buy another.

Third: Use only Mac laptops. Windows computers might cost a bit less initially but they definitely require on-going maintenance. Just say no.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
