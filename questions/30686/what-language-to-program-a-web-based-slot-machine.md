## What language to program a web based slot machine

- posted by: [Benny](https://stackexchange.com/users/-1/13536-benny) on 2011-09-26
- tagged: `development`
- score: 1

I'm wanting to create a web site that will have a slot machine game on it. I want to have a facebook app as well as apps for mobile (iphone/android). 

I want to have prizes and a progressive jackpot on the site as well, so they would all need to work together. I also want it to be highly scalable so hopefully one day it could handle up to 50 million users.

I'm not sure what language is the best for me to write this in. Is there someone that has done something like this that can offer me some advice? It would be greatly appreciated.



## Answer 30693

- posted by: [Mihaly Borbely](https://stackexchange.com/users/-1/13257-mihaly-borbely) on 2011-09-26
- score: 1

Choose the language you are most familiar with. Forget scalability. I know it sounds weird, but the success of your app will depend on completely different things.

What you need is not the most elegant code architecture or the most scalable app. You need a service that serves existing needs. This is harder to make than you imagine. Concentrate on that. Worry about scaling when you need to. Be happy if you reach that point. Most people don't.

http://gettingreal.37signals.com/ch04_Scale_Later.php


## Answer 30697

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-09-26
- score: 0

**Ruby on Rails**

Amazing web framework. Simple, elegant, code and there are cloud hosting platforms like Heroku.com and Engineyard.com that will make it easier to 'scale.'

Usually use PostgreSQL or mySQL for database.

:Pretty much all I code new projects in.

**PHP**

The most popular server side website technology. Facebook uses it, among others. mySQL or PostgreSQL as the database. You can use Symfony or cakePHP frameworks to speed along some things if needed.

**ASP .NET, Java, Python PERL**

There are lots of options but I RoR & PHP are great.

But Mihaly is right, worry about 'scaling' when you need to worry about scaling. Nice to look ahead but, its really not a concern for 99.9999% of websites ;)


## Answer 30698

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-09-27
- score: 0

There are a few opinions around "ignore scaling" as a concern, I would like to put a case that is a little different.

While I agree most techies, including myself, get all caught up in performance concerns, most of which turn out to be completely useless, there is still several good cases for still including performance as ONE OF your key design metrics.

- If your hosting "in the cloud" then compute time is a cost factor, the more effecient you are the cheaper your app will be to run. -  again to start with this will be only a few dollars difference per month so the ROI means don't spend too long ... 
- If your not in the cloud, then how many users per new machine? 100 VS 25000 is a big scale difference when it comes to buying computers.
- Very ineffecicent database designs can be very costly to refactor, investing a extra few hours going through alternatives can pay off as your database grows through its first 1000, 10000, and million records ... 
- Highly coupled systems, a hallmark of "dive in somewhere and start coding from beginners" makes it very hard to refactor your code, where possible design the components in isolation so they can be tuned later  
- Spend a little bit of time to instrument your system. If you can get timing and volume data from components of your system then you stand a chance of being able to isolate the issues as they arise ... a magic black box is impossible.

Then balancer is, its better to get something running today than to have the ultimate performance based system. 

My advice would be have performance and good seperation of concerns design in the list but don't obsess about it. If you isolate components of the system you should be in good shape.

**As for "which langauge" to use**? 

It doesn't matter all that much, a well designed system in a slow langauge can be far better than a slapped together system written in C or assembler ... plus you stand a chance of finishing it.

I use .NET and SQL Server because I know them backwards, know what the rules are and when to break them, SQL Server I can normally tune to perfection ... In comparison JAVA, RoR, MySQL, Oracle etc I don't know much about, they probably can do the job just fine too. 

I know the overall design pricipals that would probably keep me on track with any OO langauge but I know I can make my tooling hammer when the time comes ... and in Australia I can hire a LOT of developers capable of doing the same ... **People, the true scale concern** over raw instructions per second if you really grow.

**Your "50 Million users" goal**

This is a nice goal to have but really you need to ask

 - How will I get my first 10 users? then 100? then 1000? 
 - It may go viral after that, if it doesn't how are you going to scale? Advertising?
 - How are you going to make money from it? Its going to cost you something to run, especially if you get 50 million users.
 - What is it going to cost you to host and run the app for 1 person? (then for 10000 people, then for a million people)
 - How many people would be playing it at any one time? 
 - What does your storage structure look like? When you put 10000 people in it all playing the game 20 minutes per day ... what does your growth pattern look like? 
 - When do you hit the limit on a 10GB database? (Never on an over normilised database, 2 months on a big "flat file holding XML")

**To summerise**:

- Software scaling should be a consideration, but only one of many. Design for it early on then wait till issues show before tuning.
- People are harder to scale than software. If your successful, you will need others, maybe business people, maybe developers, maybe support ... Is the pool of available talent in your area going to limit you?
- Business model will impact your ability scale more than software. No cashflow is end game, too many people turned away by prices or annoying ads leads to no cashflow. This bit is tricky, for your app don't change the general user, either freemium OR advanced leader boards OR targeted advertising seem to be obvious choices.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
