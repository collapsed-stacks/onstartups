## Initial funding for Server cost

- posted by: [user892134](https://stackexchange.com/users/-1/15962-user892134) on 2012-01-25
- tagged: `website`, `business`
- score: 0

I'm nearing completion of my website.  I need advice on how i would go about server costs?  I haven't got the type of money to pay for a good dedicated/VPS server for high traffic.  Should i go about getting funding first from an angel investor before putting the website live?  If the investor wants to see traffic to see if their investment is secure and can be paid back... then what?  This is my first web startup and i'm more familiar with coding/graphic design as opposed to the business side. 

Any advice appreciated.  Any websites with investors for web startups?


## Answer 35229

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2012-01-25
- score: 7

> I haven't got the type of money to pay for a good dedicated/VPS server for high traffic.

Take a job at McDonalds serving  burgers. One evening a week should be enough to pay for a decent virtual server for the month.

Seriously.

The prices are low. I can get a dedicated Phenom II with 16gb memory, windows standard and a LOT of bandwidth for 150 USD per month in chicago (which incidentally is ap lace people pay a premium for the obvious reasons that low latency to a large financial hub is interesting for those using it).

I can get a decent virtual machine for peanuts these days.

If you dont have like 500 USD to put in totally to see whether it goes off, maybe taking an evening job and saving some money is not a bad idea. I would, as in vestor, steer clear from anyone not having this kind of invetment willing to do himself.


## Answer 35243

- posted by: [mhoran_psprep](https://stackexchange.com/users/-1/15626-mhoran-psprep) on 2012-01-25
- score: 4

<p>The are services like <a href="http://aws.amazon.com/" rel="nofollow">Amazon Web Services</a> that will let you start small and grow. If you have the skills to run your own server, you can be ready to go in a few hours. The cost range from free to hundreds of dollars a month. There is no long term contract required. </p>



## Answer 35376

- posted by: [Priyeshj](https://stackexchange.com/users/-1/9078-priyeshj) on 2012-01-27
- score: 1

<p>So you almost have a finished product, and don't have the money, nor the business expertise to go all out. First thing you need to do is analyze your own situation from business side. </p>

<p>Are you serious about turning this app into a business with revenue? If so, do you have a revenue generation model in the app? if so, you should approach target audience personally and based on the interest generated, use whatever means necessary to sell the product and generate income to sustain your servers. You might find this <a href="http://paulgraham.com/startupfunding.html" rel="nofollow">post by paul graham</a> or <a href="http://www.inc.com/guides/finance/20797.html" rel="nofollow">this inc post</a>, or this useful.</p>

<p>If your application involves certain amount of crowd sourcing, then you should definitely think long term, and get a business buddy of yours to join in to assist with the business building, or vc funding. Or otherwise, depending on your location, there are usually <a href="http://meetup.com" rel="nofollow">meetups</a> related to startups you can attend in any given area, and get certain business folks interested in your idea for little performance based equity, or whatever setup you might see best. </p>

<p>Meeting the right people, and knowing what you want, can get you much further than google's app engine, Heroku, Microsoft Cloud, or Amazon Cloud services can. But, in case you would like to go solo on this, you might wanna read up on business stuff on places under <a href="http://www.ceoexpress.com/default.asp" rel="nofollow">ceoexpress</a> and the likes.</p>



## Answer 35307

- posted by: [Chris Lively](https://stackexchange.com/users/-1/1306-chris-lively) on 2012-01-26
- score: 0

Amazon has a couple of free options both in the linux and windows world.  Investigate those as your starting point.

If you have something that might need to actually scale, Amazon or a similar provider is the best way to go.

The trick is to make sure you are making the money to cover your costs if you need to go beyond their free offerings.

Regardless, this is a MUCH cheaper route to go than other hosting options.


## Answer 35310

- posted by: [Muthu](https://stackexchange.com/users/-1/13073-muthu) on 2012-01-26
- score: 0

You will need a dedicated or VPS server only in cases like the following.

 - You have some special service/executable program running on the server
 - Your load of website is too high
 - Your database/website is configuration is not available in shared hosting easily

Otherwise if your application is built on a standard website platform like php/mysql/postgres or asp .net/sql server, then you can go for shared hosting to start with. When the traffic grows, you can choose to move to better plans.

If you need some cheaper and good configuration windows servers, try looking at softsys hosting or vpsfarm. I prefer softsys.

For linux I would prefer Amazon or Rackspace.

If you have a specific requirement of a clearly dedicated ip (which should not change frequently), then amazon ec2 with reserved elastic ip would be the best option.


## Answer 35414

- posted by: [jarjar](https://stackexchange.com/users/-1/16052-jarjar) on 2012-01-29
- score: 0

This is a little off-topic, but I'd like to add that I went with MacMiniColo.net after having a spare MacMini laying around that wasn't being used.  Their cheapest plan at $35 a month is amazingly great for the quality of the connection and service I am receiving through them.

For a small website, that should give you plenty of room for growth and at the cost of a nice dinner once a month, you can't go wrong.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
