## What is the real price of an Amazon EC2 machine?

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-02-22
- tagged: `hosting`
- score: 26

Every time I have new idea I usually have a to build a small website as a prototype to pitch it. Every time I wonder what hoster to use and it seems that every time I change hoster for various reasons. I have tried Bluehost, MediaTemple,now I'm on servergrove, but there always seem to be something wrong like not enough space, or no root access, or whatever.

The question is around Amazon.. It is not clear to me what the real cost is.. it's all by traffic, usage, etc.. and seems overly complex. Has anyone setup a machine on Amazon, with root access, a descent amount of disk space (roughly 10GB) and used it for building a prototype (meaning very little customer access as you have no customer). How much were you charged in that context? Examples are super welcome.

Thanks


## Answer 21605

- posted by: [Krzysztof Kowalczyk](https://stackexchange.com/users/-1/3945-krzysztof-kowalczyk) on 2011-03-15
- score: 10

Have you considered that EC2 is not the right platform for you?

EC2 prices are public - if you do know exactly how much disk space you need, how much bandwidth you'll use, which EC2 instance you need and for how long, you can calculate to a cent how much that will cost you.

If you don't know that, then we don't know that either so we can't provide any meaningful answer.

Roughly speaking, EC2 prices are similar to what you can get elsewhere e.g. from linode or slicehost. If your needs are met by linode then just get the cheapest $20/month plan and be done with it. At those rates you won't save any meaningful amounts of money with EC2 or anyone else.

EC2 use case is for people who need capability to meet unpredictable (or fluctuating) capacity without making an up front investment to handle peak demand. The complexity of the billing system is a feature in that scenario but it does seem like for your use case it's the opposite of what you want, so just use one of the many other options that provide clear and simple pricing.


## Answer 20706

- posted by: [Travis Cole](https://stackexchange.com/users/-1/8041-travis-cole) on 2011-02-24
- score: 8

Yeah, Amazon's pricing is pretty complicated, but that's the tradeoff you have to make to really have usage based pricing.

Take a look at their calculator's "Free Usage Tier" estimates:

http://calculator.s3.amazonaws.com/calc5.html?key=my-free-website

If you've never been an AWS customer before, they will give you, for free, 12 months of a single Micro instance with a few add-ons. That's 613MB of RAM, 10GB of storage, plus various other things. It's $39.50/month after the first year.

Details are here:
http://aws.amazon.com/free/

Also it's certainly not true that you are locked into Amazon Web Services, if you're using EC2. Amazon's EBS root EC2 instances are really just the same as any other VPS host.




## Answer 20611

- posted by: [Sean](https://stackexchange.com/users/-1/6610-sean) on 2011-02-22
- score: 6

Well for a year, it's free within limits: http://aws.amazon.com/ec2/pricing/

However, once that's up, you're looking at a MINIMUM of ~$60 a month to keep the lights on on a small instance ($0.0825/hr * 24 hours * 30 days = $61.20/month).  Then you have to pay for traffic and storage.

Now you can get a hell of a VPS for that.


## Answer 21610

- posted by: [stoj](https://stackexchange.com/users/-1/6620-stoj) on 2011-03-15
- score: 4

Cloud hosting services really aren't appropriate for testing new sites out. The whole point in using a cloud hosting service is so that you can quickly meet surges in traffic without having to invest in a bunch of hardware and system administrators up front. If you are just running a normal site or a test site you are going to be paying a premium for the possibility of handling a large surge in traffic. 

There are also some added risks to using usage based services. A couple of years back I had a video clip on a landing page hosted on Rackspace (Moso at the time) ~10mb and a competitor stole my landing page and hot linked the video and cost me a few hundred dollars in bandwidth before I realized it and shut it down.


## Answer 20614

- posted by: [Peter L](https://stackexchange.com/users/-1/7131-peter-l) on 2011-02-22
- score: 2

Following on what Sean said, for small-scale purposes, your costs are close to $0.

After that, "it depends."

What are your bandwidth demands?  Your storage demands?  Your load demands?

And finally, your reliability demands?

People's examples with storage-heavy but CPU-light sites won't be relevant to you if you're running a CPU-intensive but low-bandwidth and low-storage application that requires spooling up a lot of machines to do computation work.

In talking to a lot of people over the last few years, EC2 is quite popular as an out-of-the-gate cloud solution, but as you start to push it in various directions, the general consensus is that there are cheaper & more reliable providers out there.

The point at which you outgrow EC2 is something that's rapidly changing over time as Amazon improves, but also as other Cloud providers improve their offerings as well.  Everyone sees the writing on the wall - virtualization has turned hardware into software.



## Answer 21618

- posted by: [Tass Skoudros](https://stackexchange.com/users/-1/8649-tass-skoudros) on 2011-03-15
- score: 2

The real price of Amazon Ec2 is based on your usage of the service. There are a myriad of different ways to cut costs but by far the most clear of all the prices is the EC2 instance itself. 

A rough way to measure the cost of an EC2 instance would be to take the instances (i.e m1.small) per hour cost and multiply it by 24 then take that number and work out the full monthly cost.

If you did this you will realize that EC2 is expensive compared with other services, Ec2 is only useful as a prototyping environment for larger scale projects where you will be using more than 1 server in unison. The main reason for this is you only pay for the service when your servers are running. Something unique to cloud hosting. 

You get the ability to grow from the very beginning and you can tailor your environment so it grows according to actual capacity requirements not that you chose a Large server, and are stuck with a large server. 


Some advantages of Ec2

 - you get root access to your server
 - On Ec2 you only pay for what you use,
   and you do not pay for servers if
   they are stopped.  
 - cost of
   bandwidth and storage is competitive.
 - you pay by the hour, and billed monthly.


As an example we use a m1.small instance for Qa stuff it has minimal traffic and is on for a few hours a day. We pay about $10 / month. If we ran it full time it would cost about $70. 








## Answer 20656

- posted by: [Marcus Shockley](https://stackexchange.com/users/-1/8007-marcus-shockley) on 2011-02-23
- score: 1

Have you looked at Amazon's Micro on-demand instances? Although not very beefy it is intended to fill that gap of try to get from 0-60 and while the app is being built, etc.


## Answer 20678

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-02-24
- score: 0

Its a ripp off compared to hosting your own app on your own server.  Plus its proprietary meaning that you cannot simply just move from amazon to rackspace or others. 

Look to build your app on traditional VM images for windows or linux.  Host them via VPS hosting or buy your own boxes and throw them on there when the break off makes sense. 




## Answer 36580

- posted by: [Darren Cook](https://stackexchange.com/users/-1/14258-darren-cook) on 2012-02-26
- score: 0

I did a real-world comparison of Rackspace and Amazon here: http://darrendev.blogspot.com/2011/11/actual-costs-rackspace-cloud.html   (NB. this was for a 24/7 web spider and data mining script, not using much CPU or memory.)

Hewlett Packard are about to launch a cloud computing platform, using the same system as Rackspace (meaning any scripts you build for one can apply to the other). Amazon is still way out in front in terms of features and geographic coverage though.


## Answer 47744

- posted by: [tanmay](https://stackexchange.com/users/-1/25238-tanmay) on 2013-02-27
- score: 0

have your tried Openshift from redhat.

It does pretty much everything you are asking for except the disk space.

The other free option was cloudfoundry.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
