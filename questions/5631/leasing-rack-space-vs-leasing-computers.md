## Leasing rack space vs leasing computers

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2009-12-29
- tagged: `hosting`, `lease`, `cost-benefit`
- score: 4

Currently hosting is our second biggest expense (after payroll).  The question of buying hardware or buying your own is probably a common dilemma for SaaS companies.  

At the moment, I am not leasing rack space from the co-lo, just their machines so we can't install our own or customer-supplied hardware.  Given our current hosting requirements and the size of our company, leasing machines makes many things easier on our end.

* Keeping similar hardware and software configuration across all servers (we have seven) simplifies administration (provisioning, backups and patches). 

* Any hardware failure is the responsibility of the hosting provider and they handle it within hours.  This also means we do not have to stock compatible replacement parts for our machines.

* The hosting provider staff is very knowledgeable and periodically assists in troubleshooting issues with system configuration. This option would not be available if we had our own machines.

* If we need a new server, their provisioning time is under an hour.

* I upgrade to new servers every few years so leasing is slightly cheaper than renting co-lo space, and paying for bandwidth.  I also get the tax deduction immediately rather than have to depreciate. 

* Delegating the installation and maintenance to the hosting provider allows us to put servers in several geographically separated locations (we have servers in California, Virginia and Texas).

At some point though the cost to lease does offset most of the benefits.  What are your experiences?  Has anyone switched from leasing to owning (or vice versa)?  




## Answer 5636

- posted by: [Reid Wilson](https://stackexchange.com/users/-1/2038-reid-wilson) on 2009-12-29
- score: 8

<p>We lease some of our servers through <a href="http://www.theplanet.com" rel="nofollow">The Planet</a> (formerly EV1 Servers and before that Rackshack) -- I think The Planet is one of the largest providers of dedicated servers in the U.S. -- perhaps the largest in the world?</p>

<p>I've been a client of theirs for about seven years and am very happy with the service I get. If you watch the sales, they often offer very good deals at prices you keep getting ever after, and if you want them to manage your server(s) they can do that too.</p>

<p>Here's something I learned this year: prices are negotiable. Check out deals online, then talk to a sales person. I've been very impressed with the discounts I ended up getting going that route. I also negotiated a discount on a server I had been using for a very long time (and had probably completely paid for long ago). Again, these aren't "three months and then back to full price" deals, but are for the lifetime of the server.</p>

<p>In the past I've often compared The Planet to <a href="http://www.rackspace.com" rel="nofollow">Rackspace</a> (perhaps the Cadillac of dedicated server providers). Rackspace's "fanatical support" has always impressed me, but their prices have always intimidated me. (But perhaps I erred in never trying to negotiate down on web-published prices!)</p>

<p>Into the future though I see us using Amazon Web Services (aka "The Cloud") more and more, especially server instances through EC2. In addition to cost savings, the flexibility and capability to quickly scale up is very nice. And once Amazon Relational Data Services (RDS) moves out of beta and offers slave redundancy, we'll likely start making the move -- the beauty of RDS is that you can scale a particular instance up and down regarding its "umph". (How's that for a technical term?)</p>

<p>There's a bit of a learning curve getting going with Amazon Web Services but I bet their documentation and online assistance is better now then when I started. And another thing about EC2 is that you can just get "normal" Linux servers that you can set up however you like. Should Amazon stop offering EC2 one day, it would be simple for us to migrate back to The Planet or another ISP.</p>

<p>I've been involved with other companies that co-locate or have their servers in their own facility. At least in the situations I've been a part of, costs are much higher going that route while reliability has suffered. One issue with having servers in your own facility is that the world can't get to you if your local internet connection goes down.</p>



## Answer 5635

- posted by: [Chris Dansie](https://stackexchange.com/users/-1/2053-chris-dansie) on 2009-12-29
- score: 6

For 10+ years we owned the hardware and had to maintain it. Our systems became very large and complicated. In the end, the primary cost (and risk) wasn't the hardware, but the systems administrators to maintain it.

I've since outsourced all hardware to so called "cloud providers" such as Rackspace, GoGrid, Amazon's AWS, etc. Smartest thing I ever did. While it does eliminate the need for some systems administrators, often those skills can be transferred to focusing on OS and application maintenance...not hardware maintenance.

At the end of the day the cost is much less and a deep security analysis will show that the security risk is not any greater. Reliability and redundancy can also improve if done right.



## Answer 5658

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2009-12-30
- score: 2

I think this should be **discussed based on what the business requirements and risks are**; not what the intrinsic differences between colo of own equipment / server lease / cloud computing are.

Very shortly, the intrinsic differences between the 3 models as I see them:

 - **Colo** benefits: Cheapest in the long run, allows for specialized hardware (SSDs, crypot cards, video encoder cards, etc) if this is beneficial to the business. Drawbacks: High initial cost (spare parts), good sysadmins are hard to come by and need managing.

 - **Server lease**: Middle of the road compromise between colo and cloud computing.

 - **Cloud computing** benefits: Shortest time to market, greatest scalability, offers more value-added services for later-stage scaling (load balancing, scalable storage APIs etc), complete utility pricing model. Drawbacks: Most expensive in the long run (assuming you can handle the sysadmin side of colo very cost-effectively); very strong vendor lock in; premature implementation of those nice scalable APIs will cost you on time to market.

What could be some of the **decision points for the business requirements and risks**? That could be a long list, but here are some initial ideas:

 - Can you obtain a 10x cost benefit by using specialized hardware configuration (encoder cards, high-end SSDs, very cheap clusterede SATA disks for mass storage, etc) **--> colo.**

 - Are your capacity forecasts wildly uncertain **--> cloud computing.**

 - Do you realistically expect huge growth rates (10x - 100x per year), and a need for a large server farm soon'ish **--> cloud computing** (colo can have long lead times for acquiring more capacity).

 - Is your business trajectory not clear yet, and you want to retain maximum flexibility over the near to mid term **--> server lease** (or possibly colo, if you have good sysadmins inhouse and a good datacenter near by).


## Answer 5764

- posted by: [MrMartin](https://stackexchange.com/users/-1/2097-mrmartin) on 2009-12-31
- score: 1

I've been using Rackspace's Cloud (formerly Mosso) for the past 4 years.  Originally we used the $100 a month server but found we needed full control of the server(adding Sphinx to the database server was one issue).  The newer Cloud Servers product is absolutely awesome for development and testing as you can clone existing servers and scale their resources up and down as needed.  The lowest cost Linux instance comes in at around $15/mo.  but having tried every shared hosting provider and cloud solution such as GoGrid there's no comparison when it comes to cost savings and ease of use.  It's very inexpensive to try out and it has saved our company a ton of money.  





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
