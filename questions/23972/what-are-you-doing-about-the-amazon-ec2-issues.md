## What are you doing about the Amazon EC2 issues?

- posted by: [Jorge Guzman](https://stackexchange.com/users/-1/9525-jorge-guzman) on 2011-04-25
- tagged: `saas`, `infrastructure`, `server`
- score: 2

Amazon has been having a lot of issues on EC2 through this weekend and I am sure many other startups got burned by them. What are you guys doing about it? Do you consider Amazon equally reliable now or do you have any plans to partially more off of this service?

How else do you plan to mitigate the risk?


## Answer 23987

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2011-04-25
- score: 4

Having had to build server rooms and worry about uptime before and considering I had to dump hundreds of thousands $ to build and maintain darn things. I've had 2 disks fail in RAID5, power cables and fiber cut by stupid utility crews, main AC and the redundant one fail the same day, UPS batteries overcharged and almost catch on fire... etc. etc. etc. Not including stupid things like network admin shutting down wrong server for maintenance.

I will take cloud ANY day! Amount of effort and resources it takes to maintain an uptime equal to Amazon or Rackspace cloud (or Google Apps) is virtually unattainable for startups, until you are willing to write checks with many zeroes before the period and hire 24X7X365 staff.

We should be honest with ourselves - we have same level of expectations we are spending $1000 per month without up-front capital costs as what would be more fit for heavily front-loaded 10X+ in cost.


## Answer 23977

- posted by: [AlanBarber](https://stackexchange.com/users/-1/8933-alanbarber) on 2011-04-25
- score: 2

Amazon had issues in 1 of their 5 datacenters and it was the first time in a very long time for them to have any issues.

They still have one of the best availability records even with this outage.

The particulars of this outage are still being discovered and reported on but it seems to boil down to some sort of network failure caused one of the 4 zones in the virgina data center to start a massive remirroring of the ESB (elastic storage block) services. Which as a result saturated their management systems that control the cloud in the datacenter.

While it's terrible for all those that suffered from it many companies like netflix (that runs inside amazon) didn't go down at all because they planned for such situations by spreading loads across multiple zones in multiple datacenters.

I think most will not move off of amazon just becuase of one outage but instead will learn to better understand and use the cloud in such a way that issues in one area will not bring them down in the future.




## Answer 23976

- posted by: [Gino Cerro](https://stackexchange.com/users/-1/9971-gino-cerro) on 2011-04-25
- score: 1

Jorge,

We were in the process of moving from our traditional hosting provider to EC2 when the Big Downtime happened.  At first, we had mixed feelings about the situation but then, we continued our work toward Amazon's cloud service for the following reasons:

 1. From its beginning, EC2 has a proven track record
 2. Amazon's AWS has the most complete offer of services
 3. Last week events will force Amazon to make EC2 even better

At the moment, we are still testing the environment but we are confident that it will fill our long-term needs.

Regards.


## Answer 23978

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2011-04-25
- score: 1

Unfortunate hiccup. Amazon is still one of the great providers out there. If it can happen to them, it can happen to anyone. If your product is good, your clients will forgive you for that hiccup.


## Answer 23980

- posted by: [Nick ](https://stackexchange.com/users/-1/1502-nick) on 2011-04-25
- score: 0

Shouldn't individuals though not need to worry about load distributing across datacenters? That's' half of the appeal of the cloud. Not having to worry about that (like Netflix). Cloud = outsourcing server team. (in some ways)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
