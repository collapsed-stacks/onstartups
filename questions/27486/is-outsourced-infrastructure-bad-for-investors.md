## Is outsourced infrastructure bad for investors?

- posted by: [VP.](https://stackexchange.com/users/-1/11950-vp) on 2011-07-13
- tagged: `outsourcing`, `infrastructure`
- score: 7

I did work for more than 6 startups. I never saw it. But I heard from a friend that is working for a network appliance startup, that his CEO, wants to keep the whole infrastructure in-house, because it looks amateur in the investor's eyes, if they use external services like business google mail, github private repos and etc. For me it makes no sense at all, since myself, as investor, I would look for a company that will spend my money in their core-business and not keep 2 admins, multiple servers, having problem with backup script that doesn't work and so on. 

Anybody here agrees that outsourced infrastructure looks amateur? 

Any reference showing that it's a huge BS?


## Answer 27498

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2011-07-13
- score: 10

In my opinion it would look even more amateur for investors if a startup **didnt** outsource large parts of its IT infrastructure to someone else. Startups need to focus on their business offering, build their applications, and not worry about server racks for exchange or LAMP blades. 

From experience, my wife works for a 3 year old startup that raised 10's of millions of dollars already from investors and it on the way to being bought. All of their infrastructures are outsources, down to the exchange server ,file servers and application servers. They wrote the code, but it's deployed and managed on someone else's farm.

I believe it's the only way to prepare your business for real growth and scalability and frees your time to work on things that matter.


## Answer 27497

- posted by: [vartec](https://stackexchange.com/users/-1/10635-vartec) on 2011-07-13
- score: 3

<p>Not at all. There are many successful startups running using IaaS or SaaS. And even already not startups, like Netflix with $2.2 billion revenue, and they're using Amazon Web Services. 
You can read why AWS on Netflix' tech blog post: <a href="http://techblog.netflix.com/2010/12/four-reasons-we-choose-amazons-cloud-as.html" rel="nofollow">"Four Reasons We Choose Amazon’s Cloud as Our Computing Platform"</a> and in presentation <a href="http://techblog.netflix.com/2011/03/cloud-connect-keynote-complexity-and.html" rel="nofollow">"Netflix In The Clouds"</a>. </p>

<p>Using free GMail accounts for company, that indeed wouldn't be very professional. But if you're using <a href="http://www.google.com/apps/intl/en/business/" rel="nofollow">Google Apps for Business</a>, it would be ridiculous to call it unprofessional. I would say similar logic applies to <a href="http://www.atlassian.com/hosted/studio/" rel="nofollow">JIRA Studio</a>, of course hosting it yourself gives you more control, but it's a professional SaaS used by important players. </p>



## Answer 27517

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2011-07-14
- score: 3

For what it's worth, I started off building out a level of infrastructure for my business but am slowing dismantling it and moving to the cloud/private hosted services.  Even with stuff in the cloud, you're going to need admins if you're running a decent scale business, but it makes no sense to me to have a bunch of people running internal infrastructure for a < 5-10 man shop.  The quality of hosted tools is excellent in any case.

I would have a more fundamental question if I were an investor - do I want my investment dollars going into a firm that wants to waste a bunch of money on non-core activities and facilities...?

(I should point out that some level of internal infrastructure is inevitable - for example, if you are doing embedded development then you'll need testbeds, or if you're doing some sort of enterprise deployed software that is highly performance critical, you'll need a dedicated 'perf lab', but I would try to make zero servers the goal).


## Answer 27528

- posted by: [alphadogg](https://stackexchange.com/users/-1/3197-alphadogg) on 2011-07-14
- score: 0

I don't think it LOOKS amateur.

But, I also don't think people fully grasp what they give up when they outsource. Don't get me wrong, partially or fully outsourcing your infrastructure is not inherently wrong.

Basically, outsourcing is about removing the number of hands you control over your infrastructure, and to some degree, your business model (some online apps constrain you into their way of working). Yes, less hands means less direct expense, and that is the limit of the ability to think of some. Because they don't see the indirect expense of managing the managers, or the bigger potential expense that is taken on as risk.

I had a buddy have his data center go bankrupt and close shop, which not only took him offline, but also made him lose access to his colo'ed boxes for days. (BTW, his backup server was also in the colo. Ugh.) I have seen downtimes on virutal hosters cause another to almost go bankrupt for being down two days, which was a critical length of time to his business. I've seen a third company not be able to receive email from their 800 vendor contacts because their email provider implemented an aggressive spam policy that they did not want to roll back. They survived, but their reputation was dinged. Myself, in an older effort, I had used a backup service for keeping offsite backups of all my company servers. What didn't register was that the center was in New Orleans. Yep, Hurricane Katrina took care of that.

Amazon virtual servers (and like) are not cheap at all anymore, and severely underperform dollar-for-dollar. For the few hundreds a month you pay Amazon per server, you could get a colo box, fat bandwidth and get a sysadmin to help with the setup and occasional maintenance issue. You get to keep your data and your destiny.

OTOH, a law office I know waited two days for technicians to swap a motherboard on their in-house server. Yes, horrors exist on either side. That is why my strategy is to always use both redundantly.

What would look amateur (to me, as an investor) is someone who doesn't understand the pros and cons of outsourcing and has one-sided opinion of it either way.


## Answer 27489

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-07-13
- score: -2

Yes.

Problem is that:

* You may have legal problems. What exactly is the contract you ahve with gfoogle? Privacy laws? desaster recoveryp lans?
* Dont get into Githu´b. Yo do software development, that IS your asset, and you put it on a public service on the internet? NICE TRY ;)
* Backup "script" is amateurisch, to. Use backup software.

A decent small startup setup could be:

* 2 servers based on micro atc (16gb each)
* Virtualiaztion on top as needed
* A virtual server platform in a data center if needed.
* Backup device as needed. Tape still rules.

Finished.

That is quite as decent as it gets. I run something like that, although this is a little biger on the prioduction side, but my infrastructure is basically smoething like that.

I personalyl woudl also be careful with any company thinking gmail is viable. They are note evena ble to enforce the privacy laws I am obliged to follow as eu citizen.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
