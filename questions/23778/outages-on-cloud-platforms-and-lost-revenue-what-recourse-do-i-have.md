## Outages on cloud platforms and lost revenue - what recourse do I have?

- posted by: [Korneel Bouman](https://stackexchange.com/users/-1/9872-korneel-bouman) on 2011-04-21
- tagged: `cloud`
- score: 9

Inspired by today's EC2 outage, if I build a webapp on a cloud service, and they have an outage which affects my business, is there anyway I can hold them responsible for lost revenue? Or should I see that as a cost of doing business to be outweighed (hopefully) by the benefits cloud computing offer in terms of flexibility, scalability, etc?



## Answer 23779

- posted by: [Alex Miller](https://stackexchange.com/users/-1/8839-alex-miller) on 2011-04-21
- score: 7

The short answer here is no.  When signing up for these services the agreement you sign will almost certainly contain a clause as part of the SLA (service level agreement) that their financial liability can't extend beyond the amount you paid for the service while it was down.  That is, if you pay $31/month for a service and it is down for a full day, you are entitled to $1 at best.

In terms of whether it is worth the trade off or not?  You have to ask yourself and think about whether you would be able to maintain better uptime for your services at the same or lesser cost than the cloud provider you are using.  Also, if you have a service that has large changes in demand over time (needing to triple resources for a 24 hour period for instance), would running it yourself give you that flexibility?  Ultimately cloud computing can be a helpful tool when you're starting off or rapidly scaling up, but once you have grown your service, have predictable traffic levels and have a competent SysAdmin, you'll probably want to bring your servers in house.


## Answer 23785

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2011-04-21
- score: 3

<p>I wouldn't look at it that way. Select the provider with the best uptime record, don't think of it in terms of getting money back afterwards, it'll never cover the true cost.</p>

<p>As an aside, I used Amazon US East and Eu and the quality of the EU service is great, US East has been variable over the several months I've monitored them. So I put my critical system on EU, despite the extra cost.</p>

<p>If you've already provisioned on a weaker region, it is possible to move snapshots across region, though not trivial. Also, providers like <a href="http://Ylastic.com" rel="nofollow">Ylastic</a> do in their GUI for you.</p>

<p>You could keep doing this if one region then became the highest quality, maybe averaging over the last 6-12 months.</p>



## Answer 23783

- posted by: [Yuri Gadow](https://stackexchange.com/users/-1/5083-yuri-gadow) on 2011-04-21
- score: 2

As @Alex indicates, it depends entirely on the agreement negotiated (or not for us small fries) between you and them, as with any provider of services to your company, be they a telco, cloud provider, SaaS vendor, etc.

If you're a bit larger, or have a good relationship with a provider, significant problems can be escalated resulting in what essentially amounts to light professional services on their part, e.g., helping you use their service in better way to prevent a recurrence (I've seen this with Amazon and Rackspace, though the former was more traditional in terms of requiring CxO's be involved first and not helping until the politics/press got sticky.)

But, if, as it appears at the moment, the outage is truly contained to an availability zone(s), Amazon's response will probably be a polite reminder to those who actually got taken down by it that this "cloud" is mostly a very fancy VPS system and HA is still our (the customers) responsibility to understand and manage.


## Answer 23802

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-04-21
- score: 2

"We'll be back shortly, we hope. Sorry, it sucks for us too," a note on Quora’s website explained, according to CNET. "We'd point fingers, but we wouldn't be where we are today without EC2."

I agree with that sentiment. The Amazon outage affected us at contentcrooner.com too. But even so, we have had physical servers fail in the past too. Downtime has been very, very low on our cloud servers. Just on that point it has been better than physical servers. Even with this outage it is still an easy choice to stay in the cloud.

You are 19 times more likely to die is a car crash than a plane crash, but what gets the press? It's the same thing here. So don't drive when you can fly, use cloud servers rather than physical servers.


## Answer 23788

- posted by: [Igorek](https://stackexchange.com/users/-1/4395-igorek) on 2011-04-21
- score: 0

Windows Azure cloud's SLA is around loss of revenue.  If you were on Azure, you'd (theoretically) be able to receive lost revenue from Microsoft in a similar situation.

But frankly speaking, cloud providers are pretty damn good about uptime.  I can guarantee that vast vast majority of other providers would do no better and likely a lot of worse than the big boys, when it comes to uptime


## Answer 23823

- posted by: [John Corby](https://stackexchange.com/users/-1/9891-john-corby) on 2011-04-22
- score: 0

It all comes down to what cloud you choose - all clouds are not the same. Amazon cater for the mass market, low budget lot and thus you wouldn't expect them to offer the kind of SLA that a mission critical site might want. The flip side of this is the top end cloud providers which would offer you a service guarantee, but are going to cost you a fair bit more. In particular I'd suggest looking at one of the VMware hosting providers such as StratoGen, as it is a very mature technology with very little if any downtime. 



## Answer 23841

- posted by: [Nick ](https://stackexchange.com/users/-1/1502-nick) on 2011-04-22
- score: 0

I really wonder if these are a fluke or will continue. We just started building our app and it's 100% up on AWS and EC2. News like this makes me nervous, but I still think it will be easier to manage than actually having to manage a bunch of servers and have to build capacity for peak instead of building for the norm and having the ability to quickly scale to the peak with new instances. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
