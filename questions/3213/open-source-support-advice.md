## Open Source Support Advice

- posted by: [user1362](https://stackexchange.com/users/-1/1362-user1362) on 2009-11-06
- tagged: `ideas`
- score: 3

I need your advice. Our startup plan is to give support to high quality open source softwares like xen, postgresql,drupal, hadoop, nagios etc. What do you think how must be the process from beginning to end? We will give online facility for customers to rate freelancers. Customers will request support from our website and according to their location we will assign the most suitable freelancer. We also need to find professionals freelancers to support these products. We will choose freelancer by interviewing (we will ask their previous projects and a showcase etc.). What are the main points for choosing the best freelancers. Lets assume you are the one of the professionals that we want to work with. How must be the revenue share? Are there anybody have prior experience before this kind of work?


## Answer 3253

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2009-11-07
- score: 5

I'd find out first is there is a good market for this...  Are people willing to pay for it?  In my experience (and other people might have very different experiences, so please share), non-tech companies that do not have in-house staff (ie, are relatively small) and go for open source technologies are looking to save money and nothing else.

Would they use your service?  If they do, you are onto huge money, there are many companies like this.  Do very good market research on this...

You might also not want to shut yourself out of other markets:

- Why just pursue open source technologies?  Wouldn't the same company that has a need for a postgres admin to set up a backup schedule also need it for their SQL Server?  What about a similar company that just happens to use old Windows servers?

- Why just do support?  There is a question right now about someone needing a clearinghouse for old hardware, you might want to look into that...

In my view, outsourced big projects (1 day long and over) are dominated by the guru.com and the like.  If you attack stuff that is shorter (ie, "I need an admin to upgrade my server to Apache 2.4") then you are filling a very big, not so visible need.

Now, I'd say you have to look at the bigger picture.  These potential clients are not looking for fragmented stuff.  Yes, they will have an urgent need when they go to you the first time perhaps, but what they really need is hand holding.  So look into these things as well (See if you can do them and see if there is a market):

- Regular maintenance plans (5 hours admin time per month for $X dollars)

- Guaranteed emergency response in X minutes if they pay $Y per month

- Fixed price for services (Pay $X per month and you get a guaranteed Y hours of your choice of services [examples: Linux sys admin, windows sys admin, mysql admin time, etc...])

The point is that customers seldom have just one need.  They have many needs.  It would be a good idea to be a middleman in all of them.

A couple notes to make:

- It is not a bad thing to be a middleman.  It is a bad thing to not add value.  If you can do what you propose and you can do it well (ie, save your clients the headache of managing all of this themselves), then you have added value, and you should be rewarded for it.

- I realize you do not want to employ people.  The previous points I made I think you can work them out with the contractors (who is on call, etc...).

- When in doubt check out what is being done already.  Not to copy it necessarily, but to have a point of reference of a business model that works.  If you can be disruptive, great!  But you need to have a point of reference.  Do not undervalue the question of "what is being done right now in the industry".  So learn what Guru is doing right and take it into account.

- There is no "community" in this.  Is Guru a community?  Hell no.  Guru is where people with needs go to find someone to solve their problems.  There's no community, only solutions in Guru.  They can go to LinkedIn for community after they hire their consultant through Guru.

Hope it helps... Sorry about putting up so many lists.


## Answer 3259

- posted by: [Jeremy McGee](https://stackexchange.com/users/-1/1152-jeremy-mcgee) on 2009-11-07
- score: 3

Nice thought, but even in technology, *people* aren't interchangeable.

For example: if you find someone to fix my system, I'd want the same level of service next time, ideally from the same person. Big open source installations will take time to understand, so why should I as the client train up two people?


## Answer 3221

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2009-11-06
- score: 2

I think it is a terrible business model.  Why don;t you start with just ONE technology/product first.

Do you or your team have any expertise at any of the technologies you mentioned?  

You're not really giving support - you are a clearinghouse or middle-man.

Unless you already have an audience (either the customers or the freelancers) your real challenge is getting the community - not the process or the technology.  You're in for an uphill battle.

Perhaps you offer free consulting to consumers and get the providers to give a few hours of consulting away in order to start the whole process.  




## Answer 3248

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2009-11-07
- score: 1

Yours is a very interesting idea, I specifically like the concept of hiring or working as a freelancer in a local market. However, as it was mentioned above, probably the hard work will be to actually create a community... that seems to be the hard part. **Just do it** and worry about everything else when you actually have a growing community. 

To answer your questions, I think you could probably ask freelancers for references, and samples of their work, make it easy for them to join your community.

I cannot help you with the revenue share question, I will just start by trying various options and adjusting the revenue share until you find a fair share that works for both the freelancers and yourself.

I do advice you however not to stop trying whatever is you want to try, as long as you believe in yourself that is all that matters. In the end, you'll find out what works better by trying, and trying, experimenting, and trying again.

Good luck!


## Answer 3256

- posted by: [Tim Post](https://stackexchange.com/users/-1/1343-tim-post) on 2009-11-07
- score: 1

I'm not authoritative on every piece of software that you want to support, but I am in the business of supporting people in Xen deployments. I've been doing it since version 2, a little over three years.

Unless you, your managers or your QA team _really_ know the products you are going to be supporting inside and out, I'd seriously consider limiting the scope of your offerings. For instance, what are the benefits of using the low level C interface for hypercalls vs the Xen API? Why is this considered a fundamental design decision?

The same, extremely specific questions would apply to almost everything else. Will your team of independent freelancers be able to maintain consistency in what your company considers best practices when it comes to design decisions? How are you going to oversee this with such a huge base of offerings?

I think you should spend more time on really consolidating your offerings, you can always grow them as you see evidence that your distributed team is coherent and consistent when delivering.

As far as the revenue share, that's a tough one. You'll also have to deal with curbing situations where the end user circumvents you and deals with the freelancer directly. Once you put them in contact with each-other, its very difficult to prevent that.

That being said, it seems sensible to just negotiate a fixed hourly price per task with the freelancer. I.e. , someone should charge you less if they are configuring some kind of service vs actually hacking at the code to modify its behavior. After that, stick on your profit and overhead, tell the sales force where they have some room to play and let your revenue guide you when fine tuning.

Really .. please consider _seriously_ limiting the scope of your offerings until you have (A) built the machine and (B) made it well oiled.



## Answer 3260

- posted by: [Claus Schwarm](https://stackexchange.com/users/-1/294-claus-schwarm) on 2009-11-07
- score: 1

As a potential contractee for Open Source software support, I'd wonder why I should care about the location of the freelancer? I want the one providing the best value!

Whereby value = (amount of work * quality)/price.

As a freelancer, I'd have no problems if you'd take a sales commission for being the middle man. *Provided* the client pays her bills in time and acts professionally, it would be OK if you'd take, say, 15% of "really large" contracts. It would be nice if you'd take nothing for "small" contracts.

There are quite a lot of tutorials and guides for freelancers on the Internet. Research them to find out about the problems of each side of the contract. If you have good ideas how to solve these problems, you may be on to something. But I doubt, location is one of them, in general.

Hope this helps.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
