## Making Account Creation Compulsory?

- posted by: [Yasker Yasker](https://stackexchange.com/users/-1/21710-yasker-yasker) on 2013-02-15
- tagged: `online`, `account`
- score: 1

I'm hoping to start and finish a simple application (simple, so in 3 months?)

To declare the opening of a startup, and because I would like to incorporate communication between my application's users, I have considered asking them to create an account so that everything they have regarding the app won't just stay in their devices but also online (among other possible benefits).

Is it okay to require them to do so? Or will I end up sinking my ship before it even sails?


## Answer 47463

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2013-02-16
- score: 2

Anything which increases the friction of getting started with the application, such as registration, will reduce the number of users you get. Most app developers consider it a "best practice" to eliminate all forms of friction, hoping to get users to register later, if and when they are addicted to the application and its functionality. In doing so they hope to get the largest number of users.

There are some notable exceptions to this rule; Twitter and Facebook both require registration to do anything; those applications were so compelling that large numbers of users were happy to jump through the hoops.

The only way you can find out for sure is to test both approaches and see what percentage of testers become regular users under each scenario.


## Answer 47469

- posted by: [Nilzor](https://stackexchange.com/users/-1/18135-nilzor) on 2013-02-16
- score: 2

An alternative to *creating* an account is *linking to* an account - i.e. Facebook, Google, OpenId or Twitter. This will still allow to to store personalized data for each user and it will lowers the "sign-up"-barrier significantly. 

I'd be very cautious to launch a site or app these days that don't offer any of the alternatives just mentioned, given that you want an account system at all.


## Answer 47436

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2013-02-15
- score: 1

It is not unusual for an application to store information online including personal information especially if its used to communicate between users (in fact most users will assume it does, if they think about it at all)

A few things to think about:

 - Determine what information will be stored, where and for what length of time. Making sure you have a clear data retention policy and explain what data is shared between device and your server in your privacy policy will help relay some fears.
 - Linked to the first one, make sure you have a way to remove the data if the customer asks and be sure you know where there data is.
 - Think through what happens if they don't have access to the internet and wish to use the application, will certain functions still work?





## Answer 47440

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-02-15
- score: 1

There a many approaches developers can use to persist data without requiring the creation of an account.  But if you want the data to travel across devices (be it different browsers, platforms, etc) creating an account makes sense.

Which strategy you use depends on your offering, target market, etc.  





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
