## Making money out of a free and open-source application

- posted by: [Dario Solera](https://stackexchange.com/users/-1/1539-dario-solera) on 2010-04-05
- tagged: `business-model`, `open-source`
- score: 9

I've been working on a [free and open-source wiki][1] application since 2006 (that's 4 years!), and now my startup has taken over the development. Well, at least "officially".

We make several thousands downloads a month, and the application itself is quite popular in the the Microsoft world. Before doing this startup thing (which is focused on other stuff actually), I used my own free time (and that of one of the co-founders) to keep working on the project, mostly for fun. Today that same "free time" has become startup time, thus development has basically grind to a halt. We're only able to push some bugfixes a very minor updates.

Now, to somewhat fund further development, we sell commercial licenses to those who don't want or cannot work with GPL-licensed code. This generates some revenue, but it's not enough big money to allow more work to be done on the project. Moreover, it's becoming clear that to further expand the user base we have to add some big new features that require a lot of man-hours, which we don't have at this moment.

We don't want to change the application to a fully-commercial product, but rather keep this dual-licensing model. Also, we have tried to bring external contributors on board, but it's a very time-consuming task that brings very little value (basically, we spent lots of time coordinating things and getting very few work done in the end).

What would you suggest for this kind of situation? How could we make some money out of this application? I see that the wiki applications market is somewhat crowded, any idea to stand out?


  [1]: http://www.screwturn.eu


## Answer 10874

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-05
- score: 5

That's a good question, as in, it's hard to come up with great answers. I don't mean to deflate your enthusiasm, but keep the below in mind as you develop your strategy:

 - In general, the wiki market is quite crowded, both as self-hosted and hosted solutions.
 - Your wiki started as open source, i.e. at a price of zero. This 'anchors' the users expectations for price, meaning that it's hard to convince end users to pay for your services, as your pricing will emotionally seem expensive compared to zero.
 - IMO wikis are often being integrated into suites, or more comprehensive solutions, such as Atlassian's Studio package. I'm not clear on how many people want a stand-alone wiki, and how many want a wiki as a component of a larger solution, but I imagine the trend is towards more integrated solutions.
 - Some of those many monthly downloads are from people who are just kicking the tires, just looking at the application out of curiosity and without intention of using it / paying for it.

As JimBlizzard says, 3 typical breadwinners are support, hosting and consulting. However, some FOSS projects have found themselves unable to make enough money from these 3, and have toned down or removed the FOSS offering altogether. Perhaps this choice is available to you, perhaps not, it will depend on how many 3rd party contributions you have in your codebase, and who owns the copyright on these contributions.

**Some ideas:**

 1. A support subscription. A yearly subscription, perhaps charged monthly, that gives access to an extranet with downloads, proactive notification of security issues, guaranteed turnaround time on individual support requests, priority on bugfixing, etc.

 2. A partnership with a preferred webhost, who offers turn-key hosting of the wiki, and kicks a monthly fee for each customer back to the project. (Nota bene, a wiki would often be seen as a confidential, inside-the-firewall thing. Data confidentiality must be maintained, and there may not be that many customers for this.)

 3. Add-on modules. Offering the basic wiki for free, but charging money for modules that have high value for (larger) companies. One example could be an Active Directory user integration plugin.

 4. Licensing. Licensing your wiki engine to other (application suite) developers for inclusion into their applications.


## Answer 9903

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-04-06
- score: 1

Dario - I nearly used your application, but I was taken in by all the buzz around Atlassian's Confluence, which is kinda weird as I'm a .NET guy.  As this probably isn't particularly of general interest, drop me an email (see my profile) and I'll try and give you some specific feedback.


## Answer 9878

- posted by: [Jim Blizard](https://stackexchange.com/users/-1/1309-jim-blizard) on 2010-04-05
- score: 0

Generally, money is made from FOSS through support, hosting and consulting. Being the primary developer of the software you are well positioned to do all 3 of these.




## Answer 9920

- posted by: [Rahul](https://stackexchange.com/users/-1/2109-rahul) on 2010-04-07
- score: 0

In addition to support and consulting, an option would be to create a hosted wiki platform where users can create/setup wikis on demand and you charge them subscription fee for it. Before you implement it, I would recommend talking to end users and see if there is a demand for it and how much they are willing to pay.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
