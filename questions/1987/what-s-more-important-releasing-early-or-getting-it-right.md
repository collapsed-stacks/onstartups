## What's more important: releasing early or getting it right?

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2009-10-20
- tagged: `research`, `infrastructure`, `software`
- score: 22

From your point of view and experience, what is more important when you are building a web based app: 

1. release ASAP (eventhough it might not follow best practices) or 
2. release it rather late as long as you get the architecture done right

Currently I'm in the middle of the two. Somehow having background as technical person, I really want to get the architecture done right and follow best practices but sometimes if I have to adhere that, I would spend more time doing the research.

**EDIT**

When I say getting it right, it's more to the underlying architecture instead of features. It's more to scalability, code maintenance, security architecture, best practices, DRY, etc. Sometimes I can get caught up with architectures & best practices without releasing any feature to the table.


## Answer 1995

- posted by: [Del Putnam](https://stackexchange.com/users/-1/671-del-putnam) on 2009-10-20
- score: 28

Release your software earlier than you think you should.  Then follow up with quick feature releases.

Software, like art, is never finished.  But thankfully, due to the nature of software, what you put out theredoesn’t have to be static, especially if you are running a web-based business.  It’s easy to roll out new feature updates after your launch.

Don’t let this need for speed push you into releasing something with tons of bugs.  Release on quality, not on date. Instead, put fewer features into your initial roll out.  You can always add more features later.

The beauty of this model is that it lets you get early feedback from your customers and allows you to make changes…maybe even before you implement a feature.  So, listen to what they have to say.  And follow up on it.  Make your customers happy and they will stick with you.

If you have to prioritize, put your best stuff out front.  Put your most interesting feature on the front page of your website.  Make the best feature of your software completely obvious.  Show everyone why you your steak sizzles.

I you get someone hooked with the really cool feature, they will hunt around for the more mundane ones.  If you lead with the mundane, they will move on before they even understand what you are about.

Software is a journey, not a destination.


## Answer 1988

- posted by: [Slavo](https://stackexchange.com/users/-1/530-slavo) on 2009-10-20
- score: 4

Both are more important :)

It all depends of course. If you are launching your own product, you need to get it out and collect feedback, this is probably the single most important thing. If you delay it, you might be building something people don't want, and no matter how good the architecture, it will be a waste of effort and time.

On the other hand, you need something reasonably stable and good. If you know you will surely need some extensibility points from the start, spend the time and make it good. In general, if launching an app that would only be used by non-tech people, I would launch as fast as possible, they don't care about architecture - it's invisible.


## Answer 2000

- posted by: [Siddharth](https://stackexchange.com/users/-1/969-siddharth) on 2009-10-20
- score: 4

Releasing faster with bad architecture is definitely not advisable. You end up with support calls/bad name, migration issues etc etc. They just get added to waste/cost. I think the answer lies in getting a right balance between these two. From my experience i can say that more importance should be given to right architecture/performance etc rather than quickly releasing a bas software. The fact is when the right architecture is in place, your software can just takeoff from there! You can focus on features over a robust infrastructure. 

Regards,
Siddharth


## Answer 3698

- posted by: [Adam](https://stackexchange.com/users/-1/433-adam) on 2009-11-16
- score: 4

The answer is the minimum viable product.  You should release with the goal of testing your assumptions. How can you get it 'right' without knowing what the marketplace wants?  If you have already had successful products in this space, you may have a feel for what the marketplace wants but otherwise your guesses could be wrong.

Building a great architecture that supports functionality your users don't end of caring about is waste. 

http://www.startuplessonslearned.com/2009/08/minimum-viable-product-guide.html

http://www.startuplessonslearned.com/search/label/minimum viable product





## Answer 2004

- posted by: [Scott Brooks](https://stackexchange.com/users/-1/1014-scott-brooks) on 2009-10-20
- score: 3

I agree with Del Putnam above.  It wouldn't let me vote his answer up, so I added this one.


## Answer 1989

- posted by: [kender](https://stackexchange.com/users/-1/1011-kender) on 2009-10-20
- score: 2

In my opinion releasing early and fast, with just enough features to catch user's attention and just as much bugs to not scare them off is better then waiting. Especially trying to polish the architecture is not that important. 

Releasing a web application is a matter of balance, but architecture is something that could be fixed just any time. Focusing on delivering useful features for your users/customers usually works better then endless technical discussions. 


## Answer 2002

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2009-10-20
- score: 2

Forget about getting the architecture right, especially forget about scability. Only thing you can't forget about is security, security problems can eat you alive. 

First things first get it out. You can always fix it later. Also your customers will shape the product what if you spend scaling or designing "Y" feature and then see no one actually cares about it?

It's a web app so you can fix on demand, so release early, release often, forget about perfect code, scalable architecture.

But you need define the release as well. If we are talking with a launch and lots of advertisement then yes you need to think more about getting things **reasonable** right before release.

If we are talking about "a release" where people start to use your beta version then go for it.

*FYI: This is not my first hand experience as I'm not in the business of web for quite a while now, but this is more of an observation and personal opinion on the subject*


## Answer 2089

- posted by: [Oleg Kokorin](https://stackexchange.com/users/-1/968-oleg-kokorin) on 2009-10-21
- score: 2

Not only you need to release fast, and forget about features and scalable architecture... 

First thing to do is to release a mockup and see what happens. Anybody finds your site? Anyone willing to leave her email address to receive a note when the product is released?

We do this, and we get hunderds, sometimes thousands of users before we even release anything.



## Answer 2137

- posted by: [Nate Kohari](https://stackexchange.com/users/-1/1051-nate-kohari) on 2009-10-21
- score: 2

It's a delicate balance, but with SaaS, I think you should release as fast as you possibly can without sacrificing the core quality of the product. Nothing is real until someone is paying for it. Once you're live, continue to make rapid releases -- preferably one release per feature -- to match the needs of your customers.

After you've got some customers on board and money is starting to come in, don't be afraid to slow down feature work when necessary to refactor and improve your code. Code quality and product quality are not synonymous, but the former leads to the latter. The easier your code is to work with, the faster you'll be able to roll out new bug fixes and new features.


## Answer 2082

- posted by: [Adam Webber](https://stackexchange.com/users/-1/1027-adam-webber) on 2009-10-21
- score: 1

Think Fast!

A company that you should look at, if you are not familiarly with them yet is IDEO.
your question strikes at the heart of one of their rules to success: Fail faster to succeed sooner.

Develop in quick iterations. Don't get attached to your first model, it's going to change. If you don't get into the jungle, you'll never know the tiger.

this is why companies roll out with private Beta's. Understand > Observe > Visualize > Evaluate & Refine > Implement.

Do it quick and often and over again. You need to operate without a net, too much time deliberating is a harmful net. 


## Answer 2138

- posted by: [Dan Finch](https://stackexchange.com/users/-1/674-dan-finch) on 2009-10-21
- score: 1

I'd recommend releasing early - you can use feedback to make your architecture better and get more realistic use cases.


## Answer 3558

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2009-11-13
- score: 1

I started my software almost 10 years ago. It's still in alpha.

So from my experience, I would definitely tell you NOT to do what I've done. 

You should release as fast as you can to get a Version 1.0 that has the minimal capabilities you need to differentiate your product from what will be your competitors.


## Answer 3640

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-14
- score: 1

I always have in mind the 20/80 strategy.. Release the app with 20% of planned features that 80% of users will use .The quality of code is important for future development so this is a must.


## Answer 3704

- posted by: [Darius Dunlap](https://stackexchange.com/users/-1/1470-darius-dunlap) on 2009-11-16
- score: 1

Also useful resource is Steve Blank's blog, where he talks about Customer Development: 

http://steveblank.com/ 

For a much deeper (and dense) explanation of Customer Development, Steve Blank has written a book, called Four "Steps to the Epiphany"

http://www.cafepress.com/kandsranch




## Answer 3705

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-16
- score: 1

When it's early, you don't know what's "right."

That's not just true of features; it's true of architecture too.  Anyone who claims to already know exactly which DB queries will be responsible for the bottlenecks or exactly how tables should be designed is kidding themselves.


## Answer 3711

- posted by: [Winfield](https://stackexchange.com/users/-1/1020-winfield) on 2009-11-16
- score: 1

Release when you've got enough functionality for Minimum Viable Product and remember you also need to be able to measure and observe the behavior - how much do people like it?  Is it achieving the goals you set for it?

The combination of those two things and challenging yourself to release earlier than your comfortable with are the key to being able to evaluate and iteratively improve what you deliver.


## Answer 3712

- posted by: [Joe](https://stackexchange.com/users/-1/1420-joe) on 2009-11-16
- score: 1

There are already a lot of great answers to this, but thought I would share a relevant quote that I heard (can't remember source):

"If you're not embarrassed by your product when you release it, you've released too late."

 


## Answer 20425

- posted by: [zippy](https://stackexchange.com/users/-1/7781-zippy) on 2011-02-18
- score: 1

Many of the answers above talk about "releasing as fast as possible," which is too vague from my perspective. The principal choice you have to make is whether to let a certain date or a certain level of completeness determine when to release. My belief is that you should set a release date and stick to it-- even if it means stripping out features that were intended to be part of the release. This will create a precedent for all future releases being linked to specific dates and assuming missing the release deadline is not an option, it will allow you to determine which projects and teams are able to produce significant, functional releases versus those which are not. This practice will also create a culture in your company that missing deadlines is not tolerated which will force people to prioritize and come up with the features that will matter and be delivered on time. Naturally, the notion of iterating and releasing often still applies, but always on the basis of fixed release dates.


## Answer 20518

- posted by: [neoneye](https://stackexchange.com/users/-1/7922-neoneye) on 2011-02-20
- score: 1

If you write iPhone/Mac software for the appstore then watch out you don't get a poor rating because you had released too early. A 1-star rating sticks around forever. Polish core functionality until people have no reason for giving 1-star ratings and then submit it to the appstore.


## Answer 1991

- posted by: [Tiago](https://stackexchange.com/users/-1/359-tiago) on 2009-10-20
- score: 0

Release fast and improve it on a weekly basis.


## Answer 2088

- posted by: [kabir](https://stackexchange.com/users/-1/849-kabir) on 2009-10-21
- score: 0

while there needs to be a balance, however, for a startup I would agree with what most people are already saying. It is better to release fast than to try to perfect the architecture at first. It is instead better to release something in the market that works and is of reasonable quality and then get feedback on it and iteratively improvise on it. Focus more on the selling features and less on others. Architecture also can be improved as the need for scaling up happens. 



## Answer 3633

- posted by: [Joe A](https://stackexchange.com/users/-1/60-joe-a) on 2009-11-14
- score: 0

You want to release as soon as possible, but you want to get the architecture right. Don't be a software purist but in the minimum have some sense of clean, robust, and modular code. That way, when you launch you can spend more of your time adding new features and less time fixing bugs.



## Answer 20427

- posted by: [Nicko](https://stackexchange.com/users/-1/7870-nicko) on 2011-02-18
- score: 0

This is a great topic.  I'd agree that releasing faster is better and getting user feedback from a basic set of **working** features is much more valuable than fretting over all sorts of future scenarios.  I'd devote a bit of time to envision the blue sky a bit at the beginning, especially for the non-technical stakeholders.  If your business folk see a feature or change very quickly, it can really mess up your ability to manage expectations down the line, e.g., something like "well we built this secure, private thingy with all that encryption and stuff - now how do we put it on facebook?. What's that...about a week?" 


## Answer 20470

- posted by: [Jamie](https://stackexchange.com/users/-1/7889-jamie) on 2011-02-19
- score: 0

Deciding when to release is a balance of many factors. By putting off the release of your product you may start a vicious cycle of continuously redefining your goals, re-doing work and therefore never releasing the product at all.

You should ask yourself the following questions:

 - Do I have a consistent definition of 'right'?
 - Am I adding additional features rather than releasing versions?
 - What feedback am I getting on the work I have done?

You should start by writing out a roadmap for the product development project. You should ensure that you set realistic 'barebones' features for the first version. Get the architecture right on this, but don't worry about including non-core features. Stick to the goals, and release once the product is of sufficient quality.

You may want to release to a small number of people or segment of your market. This will give you feedback on the core product, and allow you to refine your future roadmap. Feedback on your project is important, so make sure you plan in time to analyse what you are doing after you have released.

Prioritise your development. Security is important for most projects. Scalability may not be initially. After the initial release then user-feedback can help guide your priorities.

Don't let perfection be your enemy!




## Answer 20525

- posted by: [Coda](https://stackexchange.com/users/-1/7926-coda) on 2011-02-21
- score: 0

Release fast and release/update often. And yes care and attention should definitely be given to the fundamentals.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
