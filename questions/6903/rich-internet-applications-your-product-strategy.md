## Rich Internet Applications - your product strategy

- posted by: [AKA AK](https://stackexchange.com/users/-1/1711-aka-ak) on 2010-01-21
- tagged: `strategy`, `platforms`, `products`
- score: 1

Could someone share your experiences if you have created a rich internet application ([Adobe AIR](http://www.adobe.com/products/air/)) version of the web application?  Or, created a hybrid or lighter version of the web application as a complement to your full fledged product using the AIR platform.  

One example in the web world that I can think of is the [TimesReader](http://firstlook.blogs.nytimes.com/category/times-reader/).  

I am looking information regarding product development, technical aspects, pricing, support etc.

Thanks in advance.


## Answer 6915

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2010-01-21
- score: 4

Checklist

**1. Why?**
It's important that you have a good understanding of what you want to build and why. Make sure that you only build if the AIR app is adding value. A lot of people make the mistakes of thinking that because the AIR framework allows you to use it off-line this is valuable to them. But given that you product is a website it might not be any advantage at all. My advise would normally be do it if one of the following criteria are met.

A. You can save the work you do with your app. (Check out sliderocket.com)
B. It's some sort of feed that would benefit from notification (Tweetdeck.com)
C. It would benefit from being as big pixelwise as possible. (Check out prezi.com )
D. You want to provide a portal into the larger site (Widgets such as for Nick.com Nickeloden)
E. You want to provide a service on top of the sites that people visit (check out the ebay air-app)
F. It's an application or service you use often and want to combine the ability to access webcontent and somehow mash it up with something in your air-application

**Scope**
Make it as small as possible and remember just because the AIR platform supports something it doesn't mean you should do it. All too often people believe that they should push the Air platform. But not all features of the environment are built equal and equally stable. Be mindful of this.

**The team**
Focus on getting as small a team as possible. The skills of the team should overlap each other as much as possible.

What you need is

UX (To create the wireframes and think about structure)
Visual Design (To Visualize the wireframes and think about transitions and flow)
Flash Frontend (to ensure that things actually transition properly)
Flex Backend (Make the app work)
Other backend (Hook up with web platform, database access etc)
Experts in specific areas if needed. 

For instance when we did the Nasdaq Market replay app we got a mathematician who was good with flash to help us do zoom in and out algorithm since it required tricky thinking.

The more these people overlap the better. I would normally advice against getting both a designer and a UX guy on the team but instead go for someone who is a combination.

**Timing**
It obviously depends on how complex the project is but I can give you some indications about how long it should take.

A. Design and Prototype (3 Weeks)
This is to create wireframes, design and a clickable prototype. Anything longer than that and your project is going too big for it's own good.

B. Development (1-3 months)
The shorter the better. It is so much better to build something simple and test it than to build the entire thing. If your prototype is done properly you can use all the assets from it (everything should be done in vector)

C. Q&A (2 Weeks)
Test with customers.

This is the average time it all should take. It can take longer and sometimes will but the smaller your team are the faster you will reach something useful.

**Product Development**
The best advise I can give you I wrote about here http://000fff.org/beyond-aesthetics-design-tips-for-startups/ 

**Two teams working together**
In order to avoid problems with two different tribes (and probably religions) working together I would normally propose to clients that they create a third project. Building an API. That way both teams will have to work together but about something that is not related to how each team do things, but rather how to build a way to speak with each other. 

It might sound stupid but I have just seen so many times that teams with often different and opposing opinions will fight each other on the correct way to do something. So instead of wasting time on that, give the teams a project that don't put them in direct conflict but rather forces them to find ways to speak indirectly with each other.

**Customers**
Be honest and transparent. If you are doing the project that you believe will benefit the customers involve them as beta testers as soon as possible. 

**DON'T** get customers involved in developing the product. Ask them what they would like, but be very clear on why you want to do the project in the first place. Usability studies is for refinement not for innovation (More about that in the Article)

I have many other tips but I hope this gives you some ideas. 

If you have other questions let me know.


## Answer 6905

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2010-01-21
- score: 0

<p>I have done quite a few Air/Flex projects for Adobe among other the <a href="http://www.adobe.com/resources/business/rich%5Finternet%5Fapps/?ogn=EN%5FUS-gntray%5Fsol%5Fria#nasdaq" rel="nofollow">Nasdaq - Market Replay</a> and my buddies actually did TimesReader</p>

<p>Is you question what is involved in creating an Adobe Air Application? I just want to understand what you are after.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
