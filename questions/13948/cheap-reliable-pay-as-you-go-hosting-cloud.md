## cheap/reliable Pay-As-You-Go hosting (cloud?)

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-08
- tagged: `hosting`
- score: 3

I need Pay as you go hosting for a few of my web startups, I don't want to pay and get a dedicated server or VPN and not even use half the resourses, I also don't want to get shared hosting and get suspended for using too much resources!

With pay as you go hosting (cloud?) I only pay for what I use, and of its cloud, I can make as many servers as I want (one for each startup) and only pay for what I use!

Can anyone suggest a few hosting companies that offer this?


## Answer 13951

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-09-08
- score: 1

<p><a href="http://code.google.com/appengine/" rel="nofollow">Google App Engine</a> is your answer.</p>

<p>But your one-eyed focus on saving money is misguided; if the startup idea is good enough to be worth your time, then it should also be worth 50-100 USD per month for hosting. Remember the <a href="http://en.wikipedia.org/wiki/Opportunity_cost" rel="nofollow">opportunity cost</a> of your time spent, i.e. the money you could have earned with a regular job in that same time.</p>

<p>Regarding App Engine, be sure to understand how Google's model works with regards to request-response cycle and background tasks. You are severely limited in what you can do, or how you go about doing it, on Google App Engine. That's one cost you pay for their nice auto-scaling and very low prices.</p>



## Answer 13956

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2010-09-08
- score: 1

It really depends on what you're trying to achieve.
When you say a few of my web startups do you mean different companies that you manage hosting for or one companies that has several different projects?
Here are the options in order of price:

Shared hosting -- cheapest, but you'll have problems if one of your sites uses a lot of resources. Prices start as low as $5/month (Haven't used this in ages, so prices might be even cheaper)
VPN -- You get a dedicated slice of a host, and you can do whatever you want with it. If you find that you're exceeding the resources of the host, you can upgrade, though it involves some down time. Prices start around 
Cloud computing -- I'm familiar with EC2 and gogrid. This is similar to VPNs except that you pay by the hour instead of by the month, and you can deploy and bring down new instances`on the fly. Administration is somewhat more complicated than with a VPN. EC2 prices start at $72/month for a small instance.

My inclination, based on your description, would be to go for a VPN for each startup. That way, if one of them grows, you can just upgrade to the next level VPN.

Slicehost and Linode are two VPN providers that are highly recommended by various people. I've used slicehost and had no issue, though only lightly.



## Answer 13958

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-09-08
- score: 1

I suggest you look at what Rackspace has to offer. They have 3 different cloud based plans:

 - Cloud Servers (Starts at $10.95/m or 1.5¢/hr / No Charge Unless You Use It!)
 - Cloud Sites (Starts at $149/m) 
 - Cloud Files (Starts at 15¢ per GB / No Charge Unless You Use It!) 

I got the above information from their site: https://www.rackspacecloud.com/signup

If what you need is normal web hosting that can scale, then I suggest you get the Cloud Sites solution, it is $149 per month but as Jesper suggested above, if you believe in your idea you should be willing to put some money down to make sure your site (which could be your entire business) is hosted in a reliable server that can scale and that will not be down when your site appears in the front page of Hackernews.

Goos luck!



## Answer 44506

- posted by: [markasaurus](https://stackexchange.com/users/-1/21770-markasaurus) on 2012-11-26
- score: 1

I always found Rackspace to be great for cloud servers. You pay by the hour used and billed monthly. If you go with a basic Linux server, its pennies per hour to operate.


## Answer 14051

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2010-09-13
- score: 0

While you're still at the early stages (and not consuming too many resources) hostgator.com's reseller plans might work for you. (Unlimited domains / 500G bandwidth for $24.95/month). 

They also have "Virtual Private Server" hosting which sounds like it might be what you are looking for. See http://www.hostgator.com/vps-hosting/ With these you can go from $19.95 to $209.95/month depending upon what youu need.

(I haven't used the virtual private server option, but the reseller accounts work well for me in running a variety of semi-independent websites. The reseller account lets you set up separate accounts with administrative privileges for each domain, along with a super-user account which can control the amount of resources used by each domain). 

Check their user forums http://forums.hostgator.com/ for strong/weak points of their service. There's a specific forum dedicated virtual private servers.


## Answer 44454

- posted by: [mojsilo](https://stackexchange.com/users/-1/1826-mojsilo) on 2012-11-24
- score: 0

I went with Amazon EC2 cloud. Here is the pricing page http://aws.amazon.com/ec2/pricing/ and a server instance types page http://aws.amazon.com/ec2/instance-types/

Disclaimer: I don't work for Amazon nor selling Amazon services.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
