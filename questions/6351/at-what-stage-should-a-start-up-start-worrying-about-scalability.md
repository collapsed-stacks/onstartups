## At what stage should a start-up start worrying about scalability?

- posted by: [Dheer Gupta](https://stackexchange.com/users/-1/2052-dheer-gupta) on 2010-01-12
- tagged: `scale`
- score: 2

**Background:**

For the past few weeks I have been working on the minimum viable product for a hosted CMS idea that I have and for the note I'm not looking for any opinions on the CMS industry or the idea in itself. For the final product (so to speak) I do plan to have it as a on-demand cloud computing based system.

**The Problem:**

I have hit a bit of a road-block, I have to decide between launching the MVP on a great dedicated server or work a little more on the development and utilize cloud computing IaaS.

I am personally bent towards the cloud solutions as it would ensure graceful expansion along with other added benifits, though on the negative side it adds a significant amount of time to the development; 

***on the other-hand*** 

going on a dedicated would be great in the early stages (with the exception of redundant resources) but would eventually be a significant liability in terms of the time it would take to make the product cloud-ready.
 
I know I am at a very early stage and that the success of the product and the time that it would take to reach a level of success that would warrant worrying about the scalability is uncertain.

**The Question:**

**Do you think** its a wise choice to spend extra dev-time to make the product scalable from the start?

**If not**, what are the reasons for this?

**Have you** ever regretted not worrying about scalability from the start?

___________________________________________________

*Additional Info*

I currently dont have a co-founder, I would have loved to have someone to take a bit of my load off, but my search for someone for my current project has been very unfruitful.

Hence I am currently the guy wearing the Marketing, Design and Development hats, I am great at all three, but all three simultaneously can be a bit taxing, hence there is a possibility that I am spending more time than necessary on the scalability concept when compared to the time it may actually take to make the MVP scalable.

For the most part I am a perfectionist, hence there is a high likelihood that I will make sure that the MVP is scalable, though I am still very keen on knowing if there is absolutely any reason why I should or should not be spending the extra dev-time. 

All opinions and feedback on the question itself are welcome.


## Answer 6361

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-01-12
- score: 4

I wouldn't spend the extra development time just to make sure your application is scalable... specially when your application might not have the need to scale at all, why waste that extra time and effort now? if your application is successful and you start getting lots of users, then you'll probably have the resources by then to scale your application if needed, don't worry about this right now.

The example given above (Twitter), it is an extreme example... if your application becomes as popular as Twitter, then you'll have the money and time to fix it... just like Twitter did. Go ahead and build something great and don't worry about scalability issues for now... that is my opinion.

Good luck!


## Answer 6362

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-12
- score: 2

Do you have **reason to believe there will be a large surge of users just after launch**, i.e. are you planning a large marketing push, do you have a substantial amount of pre-release signups etc? If so, develop the cloud version before launch.

If not, my suggestion would be **to err on the side of lower cash burn**, and launch as soon as you can. And of course continue work on the cloud version after you've launched, while you're steadily getting more customers.

Keep in mind that you can buy quick performance fixes for dedicated servers if needed. For example, you can easily migrate to 2+ dedicated servers, one for your webapp and one for your database, and get a good performance boost.

I'm a bit **surprised that it should require so much additional development to use cloud computing?** With Windows Azure, you can port a standard .NET webapp to the cloud in hours. With Rackspace Cloud or Amazon EC2 you can use MySQL on their platforms, so again porting a basic LAMP app to the cloud shouldn't take long. Keep in mind that you don't have to use all those scalable non-SQL storage APIs from day one; just move over the app as-is at first, and switch to more complex data stores later...


## Answer 6370

- posted by: [RonGa](https://stackexchange.com/users/-1/218-ronga) on 2010-01-12
- score: 2

It depends on your business plan.  If you are profitable without being scalable, and will not need to support many users in the future, then scalability is irrelevant.  If you don't make any profits before you reach a critical mass of users, then you need to plan ahead for that.

When I say plan ahead, it doesn't necessarily mean develop could support immediately, assuming that the costs are significant...  It could be using your dedicated server, but designing the system so that it is easily moved to the could when the time is right.

In many fields, scalability is crucial since economies of scale dictate the market, and in others there is room for boutique businesses...  I don't know enough about your market to tell in which you are...


## Answer 6359

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2010-01-12
- score: 1

Making it work on cloud computing shouldn't add too much development time, but, I had my application working without cloud computing as a plan, and I didn't realize that Medium Trust is the norm, and that I have 30 seconds to respond back to the main code behind page or the load balancer kills that instance of my application, so, dealing with that has been about 20 hours of work that wasn't planned.

If you design with a specific cloud in mind, and work within their limits then it should be minimal impact.

Design as much as possible for scale, as, much like Twitter, you may find that you are more popular than you expected, and then you will have unhappy users as you can't handle the load.


## Answer 6395

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-12
- score: 1

1) Prove the concept first matching system / services with paying customers / sustainable revenue streams framed by cash burn and steady adoption of your system ver # in the cloud. Good luck..



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
