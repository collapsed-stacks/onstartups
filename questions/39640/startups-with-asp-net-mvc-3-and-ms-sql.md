## Startups with ASP.Net MVC 3 and MS SQL

- posted by: [user636525](https://stackexchange.com/users/-1/18232-user636525) on 2012-06-03
- tagged: `launch`, `startup-costs`, `microsoft`
- score: 7

We were thinking of starting a Web Startup using the technologies C#,Asp.Net MVC 3 and Sqlserver. We have heard a lot of talk about "cost" when it comes to using Microsoft technologies for a startup and have read many blogs trying to discourage from using MS techhnologies for a startup. All the alternate routes suggests Ruby on Rails, Python ,PHP etc.But, Me and my team's expertize are in C# ,Asp.net and MS SQL.


But since we now have Amazon Ec2 ,Azure,Appharbor etc, do we still need to worry about the cost to begin a web startup using Asp.Net MVC and MS SQL? We are even willing to consider MYSQL or MongoDB instead of MS SQL if that can help us reduce the cost.


## Answer 39641

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2012-06-03
- score: 4

<p>If your expertise is with the MS stack then go with that.  It makes no sense to try to learn a new set of tools and platforms when trying to execute a new business - there are enough things to keep you busy.</p>

<p>Look into the <a href="http://www.microsoft.com/bizspark/" rel="nofollow">Bizspark program</a> - it essentially allows you to use the MS platform for "free" the first 3 years.</p>

<p>The "cost" of the platform/technology stack is not just the licensing fees - it includes the training, learning, maintenance and the ability to hire people who know/learn the technologies.</p>

<p>If you become successful enough to have to pay the licensing costs then you can afford them.</p>



## Answer 39643

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2012-06-03
- score: 3

> We have heard a lot of talk about "cost" when it comes to using Microsoft technologies for a 
> startup

There are a TON of idiots on this planet, and most people rambling about the cost fall into at least the category of people being ignorant (per the definition of the word - "lacking knowledge or training") torawrds the cost.

Point being, the costs are not really relevant in the larger picture. Let's leave out MS's own startup program (all you need for 3 years, the software stays yours afterwards and you pay 1000 USD or so AFTER 3 years).

SPLA means monthly payments, a Web edition Windows + a Web edition SQL Server are extremely low priced. If you move up the food chain, because you NEED it (i.e. you have more than a couple of sockets) then unless you are an idiot programmer, that is a LOT of processing power. I remember serving 400.000 VISITORS in an hour on a dual pentium with SQL Server; today with proper programming the limit is VERY high. And that is if you cannot use the free SQL Server, which already goes QUITE high.

Now, I am not saying it is free, but compare it to the running costs in general, and if it makes a significant difference, you have a problem. I am just renting a machine in Chicago - 4 cores, 16gb memory, 120gb SSD. Cost per month is in excess of 160 USD. Add Windows Standard (cannot use Web Edition as the apps there would not qualify per Web edition rules - this is an internal machine) is 20 or so USD per month. That is 12% of the server costs, including all updates (I rent monthly). Add some more for system control (SCOM). We talk of 30 USD totally, or so. 20% of server costs.

Now, here is the trick: The machine is the backbone of my business. It will, in half a year, get a mirror etc. I have 2 people working full time just to permanently develop software for it. The machine operations causes me external costs of about 300 USD per day. I pay 800 USD per month for the data on it. The 40 USD more for Windows DOES NOT SHOW UP. Lost in rounding.

Now, web apps are cheaper, but still. Given the cost for people, support etc. - if it makes a hugh difference you have a problem somewhere else.

Most people advising against Windows are either:

* Die hard Linux (Windows is EVIL - regardless how senseless)

* Cent-wise and pound-foolish - saving a cent to waste a pound. Can be because they lack the cent.

* Ignorant to what the real costs are. Windows is SO expensive up front - where the up front costs are ZERO if you are an SPLA, and you better be one because otherwise hosting may be flat illegal (not covered by normal licensing). And SPLA is cheaper anyway.

* Not specialized in Windows. If you know Ruby, but not MVC, then heck, that is the better way to go - after all, the OS costs are a lot less than the development costs.

Everyone else will tell you that yes, Windows costs money, but not in a level that will make a difference for your startup. It may even be better - I am not sure how good the Ruby tools are with stuff like proper profilers for memory and CPU utilization. It may well be those people just need large machines because they cannot write efficient code, lacking proper ways to find out where the code is slow ;)

So, here is your cost:

* SQL Server = 0 for Express Edition; check SPLA pricing for Web edition if you MUST have that. 10gb per database is quite a lot unless you store text or binary data or high resolution financial data ;)

* Windows Web Edition is - well....

I would be a lot more concerned about stuff like Amazon EC2 - the costs of that for anything but a trivial install are ridiculous. Talk cent-wise and pound-foolish... saving some small money for Windows, but wasting a lot for EC2.

Unless you have special needs, I would always start with my own servers. The moment you need more than a trivial amount of power... EC2 comes with a cost that is extreme. The moment you have some data, the costs are extreme. Cloud is a way to sell you virtual machines for a high price by the hour, instead by the month.

Go to a "real" VPS provider or rent a physical server. Compare the per monthly price with the per month price on Amazon and you will be shocked.


## Answer 39642

- posted by: [QuaffAPint](https://stackexchange.com/users/-1/13402-quaffapint) on 2012-06-03
- score: 1

I'm working on one with asp.net and originally sql server.  I have since moved to MongoDB (better fit for my needs, and better price :)).  I plan on going with appharbor when I'm ready.  In the end it may be a wee bit more, but I prefer working in .net, so why not use it.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
