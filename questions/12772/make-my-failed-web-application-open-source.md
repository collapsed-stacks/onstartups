## Make my failed Web application open source?

- posted by: [Dennis](https://stackexchange.com/users/-1/3808-dennis) on 2010-07-14
- tagged: `open-source`, `webapp`, `development`
- score: 8

I've outsourced the creation of Web Spy Pro (www.webspypro.com) last year.
It's a Webanalytics software that record/play the visitor mouse movements, so you can see exactly what visitors are doing on your site instead of guessing.
And with that gathered data it also generates advanced heatmaps.

Problem: The developer stopped working after 75% and new developers didn't understand the code.

So after spending $10k I'm done with it.
But I also feel it's a little bit sad to just throw it away...

Is there a way I can make it OpenSource so people can contribute to the software and eventually when it's running as it should, sell it?


## Answer 12818

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-16
- score: 11

Good answers in the thread already. I just want to add one element: If you just 'throw it over the wall' and into the realm of open source, then it will almost 100% certainly fail completely as an open source project. Open-sourcing and then running away is the same as killing the project outright.

There are way more open source projects than there are volunteers. If you don't trust me on this, then go have a look at Sourceforge and Google Code notice the projects that have not had updates for 2-3 years.

For projects to succeed, they need careful stewardship, a friendly community to attract developers, and some 'hotness' in technology or elsewhere that can motivate and inspire developers.

> a way I can make it OpenSource so people can contribute to the software and eventually when it's running as it should, sell it?

Yes, dual-licensing, as Steve Wilkinson pointed out. But this requires you to obtain the copyright (ownership) for all open source contributions via a contributor agreement. That raises the bar, and makes it harder to attract developers.

And additionally, if you open source just to 'feed' off the open source energy and then sell for profit, then expect your reputation to be permanently damaged. The open source community has its own set of values, and they're not always in internal agreement on them, but if they become united against an 'outsider' they can hit hard...


## Answer 12816

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-07-16
- score: 6

<p>I wouldn't completely agree that open-sourcing stops you generating product revenue, as you could <strong>dual-license</strong> your product - say GPL and commercial, that way people can get to it who might never had paid for it anyway, but for firms that need to buy a formally supported product there is always the commercial offering.  See <strong><a href="http://monty-says.blogspot.com/2009/08/thoughts-about-dual-licensing-open.html" rel="nofollow">this article by Michael Widenius, founder of MySQL</a></strong>, for example, for some thoughts on the subject.  I would also argue that you can still maintain control, as long as you don't have a do-pretty-much-what-you-like licence (such as MIT or BSD).</p>

<p>In terms of hoping that you get people to contribute freely and then sell, I don't think that is a viable model - contributors in the open-source world often contribute for altruistic reasons and knowing that your goal was to make money rather than provide a public resource is likely to hamper contributions.  (It also doesn't seem morally right to take people's contributions and generate income without giving something back.)</p>

<p>A more viable model involving open-source is to release the source so people can build add-ons - developers often do this to solve their own problems, and are also often happy to put the source out there.  One thing to be careful of generally is that you have in place a sensible contributor licence, especially if you let people contribute to the core.</p>

<p>Good luck with the project.</p>



## Answer 12779

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2010-07-14
- score: 2

If you Open Source the project, you won't be able to sell it. After all, any potential buyer could just download the source. Once it enters the public domain, it's basically out there for anyone.


## Answer 12784

- posted by: [Susan Jones](https://stackexchange.com/users/-1/2737-susan-jones) on 2010-07-15
- score: 2

Is it possible that your new developers are not competent?

Do you really want to throw it away or are you just having one of those moments?

If you go back to your original purpose for starting this project, is there another way you can achieve it?


## Answer 12799

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-07-15
- score: 2

Don't open source it unless you want to do more consulting than selling software. Too much of your time, energy and money have been put into it.

You certainly aren't dealing with typical web development stuff. Not only do you need a good developer, but one that will stick around. Unless your problems are major bugs or performance issues, hold off on development and spend the time selling this thing. 

Working on a complex project will attract developers, but if the project can be profitable for them, it will be much easier.

I wish you luck on this. After reading on usability tests, this could be the next best thing to looking over a user's shoulder.



## Answer 12802

- posted by: [Jeff Epstein](https://stackexchange.com/users/-1/3666-jeff-epstein) on 2010-07-15
- score: 2

Dennis,

If you really want to keep the software private and are worried about the expense or commitment of a programmer I would suggest that you attempt to find a programmer who will take equity in the project to work on it.

This way:

 - The programmer has a significant incentive to 'dive in'
 - You do not have to pay anymore $$
 - If it does not work, then go with the open source

Seems like a situation where you can't lose, especially if you are considering open source already...

Good Luck!


## Answer 12804

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-15
- score: 0

Im interested in working with you to finish this interesting concept.
Lets touch base.
my address is adrianadrineda at gmail


## Answer 12813

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-16
- score: 0

Dennis,
I too have had a project that was abandoned. In fact, I have the product, and actually sold a few licenses. But my 'marketing & sales' partner didn't deliver. So after 3 years, i've actually decided to re write the code. I gave my developer a % in the software, and am currently looking for marketing/sales to come on board. The target market is over 50 million users. I would not suggest you open source it, as you would then lose control over it.
just my 2 cents.


## Answer 15510

- posted by: [Lena Schimmel](https://stackexchange.com/users/-1/4970-lena-schimmel) on 2010-10-24
- score: 0

I think making it open source is a good idea. The only downside is the risk of someone taking it away and making money with it, eating you cake. So what would the potential user have to do to use your software free of charge? This depends on some technical details, which I can only guess, so I outline two scenarios:

 - If, for example, he only has to download a single PHP file, put it onto his server and everything is working, well, then he will do exactly this and has no incentive to pay anything.

 - But if, on the other hand, there are multiple parts of that software, maybe in different languages, using a complicated database setup, with diverse hard-to-fulfill dependencies, etc... That is: It would be possible to take the source and set up everything, but it would be hard. This is where your business comes in. You provide the back end and all infrastructure on your server, so the user only needs to do a little work to get it working. The user pays for the service, not for the software.

In the second case, (nearly) no end user would want to go through all the hassle to setup the back end on his own. But there would be the risk of someone else taking your software and creating the same hosting service that you build up. To prevent this, you could take some of your back end code (if possible, those parts that are already working fine) and leave those closed source.

Maybe some of my assumptions don't really fit your case, but I thought I'd just share my ideas anyway.


## Answer 15559

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-25
- score: 0

Could you enter into a partnership agreement with a development company whereby you supply the intellectual property and they provide the coding. sales and marketing can then be a joint effort.




## Answer 39575

- posted by: [Matthew Galloway](https://stackexchange.com/users/-1/15145-matthew-galloway) on 2012-06-01
- score: 0

I'm probably answering this way too late, but for others reading:

I'd follow this path:

0) try everything reasonable to see if you can bring it back from the dead...
1) try to sell it
2) IF you can't sell it OR the price offered is very low (depends on the person and the project, but say a few hundred or thousands) then release it as open source instead
3) pimp it out and promote the fact it is available as open source (back it up with a proper community website, with a forum etc for the community to help each other. If you can put one of these together yourself for free then get it touch and I'll make one for free just for the sake of encouraging open source!), hopefully then you'll reap positive karma/attention/networking which will help you for the future :-)

Additionally something nearly everybody seems to be overlooking is there is a LOT of different open source licenses.

Some of them are quite different to each other, giving the person who released to open source varying amounts of "control" over it (or not).

So seriously recommend researching and asking for advice on what open source license first so you know your options :-)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
