## Hits per day Exceed Server Capacity Dilemma

- posted by: [Matthew](https://stackexchange.com/users/-1/15130-matthew) on 2011-12-20
- tagged: `budget`, `server`
- score: 0

I have not actually bought the server hardware yet, but I am anticipating that when I do, my budget can only allow hardware enough to support 2000 hits per day on my website.  How should I handle it if the hardware's capacity is exceeded?  Surely, with a new website, I can't afford for a day of downtime...in which case I should buy in anticipation.  But unanticipated growth could be a problem...and I don't necessarily know if I want to buy all that equipment before I absolutely need it.  Any suggestions?  Thanks.


## Answer 33952

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2011-12-20
- score: 6

The first question to ask is why do you want to own your web server? As you probably know, there are many, many web hosting companies that offer extremely competitive pricing.

The next thing to consider is that the computer is only one small part of running a reliable website. For example without a reliable internet connection and power source, your computer will be unable to operate.

Consider also the need for proper backups and a disaster recovery plan (what if you have a fire?). Then there is security, what if someone tries to hack your site? Best practice is to install a high grade firewall between the internet and the server. Do you have multiple internet service providers (ISPs)? What will happen if the ISP has an outage?

When you look into what it takes to run a **reliable** website, you will find that the actual computer hardware is the cheapest part. Unfortunately far to many low budget web hosters cut too many corners and prove unreliable in the long run, select one carefully.

You are quite correct that downtime can cost you dearly both in terms of lost revenue and reputation.


## Answer 34079

- posted by: [umassthrower](https://stackexchange.com/users/-1/14929-umassthrower) on 2011-12-23
- score: 3

That's 43 seconds per request, your math is wrong.  


## Answer 33954

- posted by: [Tom Squires](https://stackexchange.com/users/-1/11392-tom-squires) on 2011-12-20
- score: 2

For your case virtual servers sound perfect. Dont invest in expensive and inflexible plysical hardware yet. Hire out a virtual server then monitor your traffic. When your demand increases you can make a few clicks to expand your capacity or fork out for hardware then. Hopefully the increased demand will pay for the increased capacity.

While your website is still new you can have a cheap small virtual server so you dont pay for resorces your not using.

As a side note, 2000 hits per day seems very low and day seems like a wierd measure. Normally its hits per second that count. Even a very small server should be able to cope with an order of magnitude more requests than your quoting. I would recomend some load tests to measure your requirements.


## Answer 34076

- posted by: [Krzysztof Kowalczyk](https://stackexchange.com/users/-1/3945-krzysztof-kowalczyk) on 2011-12-23
- score: 2

You would have to expand on how you came up with your numbers.

To give you some perspective: I run my blog (http://blog.kowalczyk.info) on App Engine. Today it'll get over 30 thousand hits. Some of those are static pages but some of those are dynamically generated in python. This level of traffic can be ran on App Engine for free (if you take care to optimize the code). In that context, your 2 thousand seem awfully low estimate.

If you're worried about going over free quota on App Engine, you can enable billing and you'll simply be charged based on the usage.

If you choose to run on AWS, you'll have similar setup - a certain capacity for a fixed price and over that you pay for usage, so on days with more traffic you'll pay more than on days with less traffic.


## Answer 34027

- posted by: [frenchie](https://stackexchange.com/users/-1/15155-frenchie) on 2011-12-22
- score: 0

Cloud computing!!!! That way you don't have to buy the hardware or worry about sizing it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
