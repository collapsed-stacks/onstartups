## Would you (Java Developer) learn PHP? if management decided opensource (PHP) projects could fulfill business requirements

- posted by: [gMaximus](https://stackexchange.com/users/-1/638-gmaximus) on 2009-10-13
- tagged: `ecommerce`, `software`, `technology`
- score: 4

(Apologies for the long post. I'm really keen to get sound and balanced advise. The only way to do that is to provide you with a good overview of the situation.. :) ..)

I would like to say upfront that i am not a programmer. I'm 1 of 3 partners in a small start up. Two of us have a business and sales background, whilst the third guy is a very experienced Java Programmer/engineer (and a good friend).

As with most start ups we believe we'll be the next big website. We have found a opportunity that the "Long Tail" really describes well. By this i mean a product range that isn't currently being tapped into online. As with Amazon, our model is about offering every available product within the niche. Through the availability of everything outside the fast selling products, we hope to become best website for the niche.

We have placed a lot of focus on building the business/technology system that allows us to build our inventory information very quickly. This was because we knew that the size of our inventory would make or break our usefulness to end users.

So now i come to the problem that prompted me to seek your help.... (please help)... :)

In my (non-technical business) mind, we now have the ability to build our inventory quickly. This is just the start though, as a business we also need the following solutions before making money:

1) A shopping cart application to allow buyers to search our inventory, communicate with our business and make orders etc.
2) A CRM application that would then allow the effective management of customers and orders.

I found my way to Magento and SugarCRM both of which appear to be very impressive. The idea being to use Magento for the buyers (search,buy,interact etc) and Sugar for our staff (order processing, customer service etc).

In my mind the long term rewards of being able to update these core applications from the communities, would far outweigh the steep learning curve. Not to mention the time/money that would be required to even attempt to catch up with what already is stable and tested....

My friend and business partner is unwilling to consider anything in PHP and to a large degree opensource. He's of the belief it would be best to start from scratch. This feels painful as he currently has a full time job and as with most start ups, we're not cash rich. My second worry is how would we keep up with any competitor who may choose the Opensource route.

Here's further details about our operational requirements:

1) Our stock is currently held across 30+ different branches. Which means that we'd need a way for each branch to sign in and manage their own customers.

2) Our business has regions and each region has branches. In order for us to focus the various management levels of the business, it would be ideal if each management level could see the business relevant to them. For example National manager (can see everything), Regional manager (can see all branches in his region), Branch manager (can see everything for his branch with certain admin rights) and Customer service (can see everything in their branch with minimal rights). This is the only way we can have one umbrella site, which can be serviced by staff in branches nationally.

3) Over and above managing orders, it also makes sense that the messages are managed centrally through the application. This way any member of staff can easily see the past history with the customer and assist. I'm thinking that the questions would almost always come in through "Ask a question about this product" link, so incoming messages could be routed to the branch who has the part. If it's aftersales, then the branch who sold it. For general questions through contact us, we'll allocate a member of staff at head office.

4) I think it would be appropriate to show buyers upfront on the product page which branch has the part and the branch information.

5) Our inventory size is currently over 300,000 products. The business plan is to rapidly increase this to 10 times that figure.

6) The products are spare parts. Therefore the buyer would need to search by the original product that the parts fits... Each part can often be used on various products.

From a language agnostic business person (non-programmer) - any opinions or advise on our situation would be much appreciated...

I'm keen to find a way of us unlocking horns, either way... I just struggle to see any strong value in "re-inventing the wheel"....

Thanks in advance, 
Guy


## Answer 1156

- posted by: [Vineet](https://stackexchange.com/users/-1/24-vineet) on 2009-10-13
- score: 7

Programmers often have a severe NIH (not invented here) syndrome - they want to build everything from scratch. It doesn't work at large companies that have alot of resources and it rarely ever works at a startup. You couldn't pay me enough to work on any team where the members want to do all the parts themselves - it just doesn't make sense.

Programming is about using the right tool for the right job. If you can get alot of benefit from PHP you should definitely do it.

In general a startup should choose the language that the founders are comfortable with, as learning a new language can take effort and time which you might not have. You should seriously evaluate if there are equivalent software in the Java world as the ones that you can see in PHP. Then again you give a good programmer a new language and he can be fluent enough in it in 24 hours.

You might need to consider if you need a partner with PHP experience. 

My personal bias: I actually belong to the same category as your programmer - I am a strong Java developer and can tell you all the reasons why I think PHP is a bad idea. But Facebook using PHP in itself is an argument that it can work in many situations - so I am not going to elaborate on those.


## Answer 1171

- posted by: [John Soer](https://stackexchange.com/users/-1/96-john-soer) on 2009-10-13
- score: 2

Some random thoughts
<li> Developers like to develop their own products.
<li> I hear this a lot if we go open source we can just modify it ourselves and they make it sound like it is trivial. In-order to modify an open source system takes a considerable amount of effort and commitment. 
<li> Going from Java to PHP is kind of shock. Even though the two languages have similar syntax the fact that Java is very consistent and uses strong type checking makes it far easier to maintain the application in Java over the long haul. (I have developed major projects in both Java and PHP)

If the open source product works for your current need most definitely go with it but if you want to make major changes to it to make it fit your business model I would do some investigation to make sure that it is still worthwhile to use the open source route. 



## Answer 1160

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2009-10-13
- score: 1

First things first: You can check the validity of your idea using open-source tools for say 6 months or so. During these 6 months, you'll learn a lot about e-commerce and customization etc.

In long term, you'll want to build your own e-commerce engine customized to your business needs and offers excellent experience to your users.

So yes, start with something that's already there, put things into action and side by side develop your own. Execution matters!


## Answer 1173

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-13
- score: 1

I agree with Vineet.  You should choose the tool that is necessary for the job, not the other way around.

There is nothing inherently wrong (or right) with using PHP or java or open source for a project.  You should fully understand the impact each decision you make will have on your business now and in the future.

It sounds like your partner isn't able to explain the reasoning behind his desire to use java very well.  ...at least not in a manner that makes sense to you.  If there is some sound reasoning, listen.  But if the arguments are what I call "religious"...in other words biased for or against some certain technology, but without specific logical foundation, then I think you may want to more carefully consider working with this partner.

Additionally, the use of open source has certain implications about your ownership of the technology and your obligations to the community of its users and developers that you need to consider.

To help answer this question, I think you should consider what investors will value about your business.  Will investors attribute your value in part based on the fact that you own the technology?  Or is your value based on the fact that you provide your service better for some other reason?

As for writing the code from scratch, in my experience it's almost never a good idea to re-invent the wheel.  Don't re-write something that has already been developed just because you want to re-write it.  The best reason to write new code is because you need to do something that hasn't been done before.

Think of all the countless hours that have been put into creating and debugging code that is already in use.  New code must be tested and debugged prior to being put into production.  That is a huge effort.

I'm curious to see how this turns out for you.  Be sure to let us know!


## Answer 1248

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-13
- score: 1

Firstly I would like to politely disagree that strong typing offers any benefit over loose typing in terms of ease of maintenance. Experienced OOP ( object oriented programmers ) will tell you that strongly typed languages sometimes require their own idioms to implement what can be done in a loosely typed language more succinctly. But I will focus my post on the business aspect of it not the technological aspect, which is only fair.

You raise two important issues, PHP vs JAVA, and Open Source vs Coding from "scratch". Firstly, I would like to point out the logical fallacy in that statement. JAVA started as and still is, an open source community effort. http://www.sun.com/software/opensource/java/ ( laughs ). If open source is good enough for the SUN corporation, it is good enough for you.

Any operational enterprise system is going to use some back-end storage mechanism, either a relational database, an object database, something like couch DB, etc... Next is your friend going to insist that you guys license copies of Oracle server for this startup? My point is not to berate him though, I am just pointing out that almost every piece of technology in existence "calls" into some lower code. Almost every smart phone made in the last few years uses linux, which you guessed it... is open source.

My point is, even if you write your own e-commerce package, you will still use open source to do it. Like it or not :-) You would be using JAVA which is OS ( open source ), if you use postresql or mysql thats OS, if it runs on linux thats OS, if you use any other OS libraries you are also committing a "sin".

So then if you can't avoid open source 100%, how can you specifically say to draw the line at your operating system, your compiler, or your database, etc..?

I think the correct answer is to take an incremental approach. It would probably take months to get a prototype working if you "invented it here", then you need Quality Assurance, rounds and rounds of testing & bug fixes. Then you need to do usability testing ( don't tell me your friend can get that right on the first 'try', large fortune 500 companies are always tweaking that kind of stuff ). My point is it would take a long time to reach a high level of maturity implementing all these operational and reporting systems from scratch, and in the mean time you guys are loosing money.

Get a working solution online first with your 300,000 products. Start putting it in front of real users, they will provide 1,000x better feedback then some "yes man" quality assurance guy who holds back his suggestions or is not engaged enough in the idea to offer real feedback. Use your users and bottom line as a way to steer you in the right direction.

For example, if you rolled your own solution is it *possible* you could spend a whole year before you go live, and then after the first quarter you guys decide you wanted something totally different? Would it make more sense to test each decision over time, and allow your incremental development to fund itself, or even fund the home-brew system at the same time? I would say do whatever you can to start making money fastest. Whether that means java, PHP, open source, closed source, or a little bit of everything.


## Answer 28603

- posted by: [bumperbox](https://stackexchange.com/users/-1/5727-bumperbox) on 2011-08-11
- score: 0

i would suggest trying magento and sugarcrm even if it is only to evaluate the two products to see if they work as you expect. it won't cost you much except for your time to evaluate them both and make a decision. writing  a shopping cart and crm to handle the number of products you suggest is going to take quite a while (if you are only doing it in the weekends). 

there are also a number of opensource java projects that cover some of the features you want, if that is preferable to your friend.

Also by taking the opensource solution (even if it is just for the short term), you can start selling in a much shorter timeframe. once your business idea is proven and develops, then you can look at customising the software or creating your own to give you a competitive advantage. 

I am a php programmer (who used to and still sometimes writes Java code), so just a note of warning Magento is probably one of the most complex php apps i have looked at. If I was a beginner php programmer i would be reluctant to start learning with that application




## Answer 28618

- posted by: [Areshchanka Alexandr](https://stackexchange.com/users/-1/8736-areshchanka-alexandr) on 2011-08-11
- score: 0

First of all I would suggest you to search similar java open source solutions, there are also good projects in that field for sure. But if still they don't fit you I would suggest two business guys concentrate on ideas and requirements. Then hire 1-2 outsource programmers, it will cost 2-3k per months. And third (Tech) can concentrate on management of developers and during that time learn php and related tech things needed for you business.


## Answer 28626

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-08-11
- score: 0

I am a Java and PHP programmer. I am skilled with both languages as I have started with PHP in 1998 and with Java in 2001. Even when the most stuff I work on at daylight is in Java, I write PHP code weekly. Java is a very good language, and PHP has some flaws, that is true. But if you start with Java, you need simply more time for your project. Not every project has this budget. Later, after lets say 4 or 5 months, when the project has grown, you become quicker with Java than with PHP. PHP is very quick if you start from scratch, but due to the kind of its language (easy types for example) you might have problems to stick on clean code. Especially if you have young programmers in team, it is easier to oversee Java code than PHP.

That being said, if you have 2 or 3 dedicated PHP programmers who -want- to do quality work, they can do it, even with huge projects. I have seen PHP software with 100.000+ lines of code which was excellent. I have seen PHP software with 10.000 lines of code which was a mess.

But the same can become true with Java software. After all, you can have a mess or quality software in each language. It is just easier with Java in huge projects, because you have tons of analysis or refactoring tools. 

That being said, what is your need? Do you need to get a quick start and do you think your product has limits in which you can see clearly the size of it? If the size is low, the budget is low and you need to go quickly, I would choose PHP.

If the size is huge, you cannot oversee the dimension of where the software can grow and probably need all of the cool refactoring/analyzing tools- go with Java. 

Another point: is your software for the cloud? Then go with Java. more tools, better support.


Now to Open Source vs from Scratch. From scratch is almost idiotic in the most cases. Even when you do not choose a ready product, you should choose a framework were you can build your product upon. You cannot avoid to use Open Source. It is excellent software (in many cases) and gives a benefits in terms of competetion, speed etc.

If the question is, a Open Source Shop or not. How complicated are your needs? Once I wrote a pretty simple shop with a few articles and a basked in 1 months fulltime (PHP). This was pretty basic. I never could simply download any of the cool plugins like for example wordpress offers, I have to write it myself. I didn't want to do that, so my shop died.
But if you have lots of requirements, like multiple currencies, translations, different shop categories, sub shops, credit card transactions etc et al, then you are wasting some time with doing it from scratch.

There is one exception. I would never use xt:Commerce/os:Commerce. This shop system is open source, but it is pain to code. You have a pretty quick start with it, but if you need to modify something you loose time and time and time

Finally I would like to add:
I would learn any language, if the tool I can use with it would solve my problem the most pragmatic way. 

Cheers


## Answer 28650

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2011-08-11
- score: -1

I am going to leave my opinions of languages and frameworks to myself. I am a biz guy and there is a reason we hire CTOs.

BUT, I do have to say that most incredible software engineers (over 200 of them so far, most full-time working for cos I've been part of) I have worked with were all platform agnostic and could learn another language literally in under a month and master it in 3 months. Those who were too married to any platform usually did not last.

Best technology decision we have made were from building experiments and beating the heck out of them.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
