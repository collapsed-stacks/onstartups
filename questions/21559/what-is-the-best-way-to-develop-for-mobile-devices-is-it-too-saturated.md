## what is the best way to develop for mobile devices? is it too saturated?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2011-03-14
- tagged: `mobile`
- score: 0

These days, I hear apps everywhere. App for everything. 

So I'm curious how hard is it to develop for a mobile device? which to develop for? android? apple?


## Answer 21591

- posted by: [Nick Campion](https://stackexchange.com/users/-1/8639-nick-campion) on 2011-03-14
- score: 3

Mobile apps are just a channel for delivery of your application. I think its important to remember that the markets are saturated with tons of bad applications. Great apps tend to separate from the chaff either by providing an experience which truly benefits from being mobile (location based or information on the go) or by polishing an already great offering available on the web (mint.com, the weather channel).

To me, you are asking the wrong question. If your idea benefits greatly from a mobile offering, then its not entirely relevant if the market is saturated. I'm going to go out on a ledge here (and share my opinion) and say you might not know what you want to develop, but you are thinking it should be mobile, in which case I would send you back to the drawing board if you were using my money. I think mobile apps and web apps with mobile views are really a means to an end, not a destination. There is an abundance of uninspired offerings in every format you can imagine, so the key to mobile and, alas, all development is to have a product idea and use the tools to implement that idea.


## Answer 21590

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2011-03-14
- score: 1

<p>I would also consider asking the question on stackoverflow - but a recent (resurrected?) push for mobile apps is to bypass writing native applications per platform and write a webapp.  37signals did a good writeup on <a href="http://37signals.com/svn/posts/2761-launch-basecamp-mobile?63" rel="nofollow">why they went that way</a>. It's more complex that just html5 - there's typically a js framework involved, and many are evolving - but that's beyond the scope of this conversation.</p>

<p><strong>Rationale for webapp</strong>?  No revenue share / required inclusion into a walled-garden app store - mobile devices come to your site, and you service them.  Simple enough.  Sure, this doesn't work if you're developing a standalone app and / or want to leverage the platform appstore as a distribution / discovery vehicle, but many times, that's not the purpose of the app.  </p>



## Answer 21678

- posted by: [jjb](https://stackexchange.com/users/-1/8669-jjb) on 2011-03-16
- score: 1

Just a few notes to add to what others have said here:

1) The major mobile application markets are saturated with basic stuff.  That is, if you can think of any "normal" application, there's probably an application for it.  In order to stand out, you have to offer something unusual.  Unless your company has the resources, design skill and vision to execute on, say, creating truly unique and impressive mobiles games, a pure app based strategy today is going to be difficult.

So, you have to have some uniqueness.  That is most often going to come from interfacing with a service.  In this case, it's the data (your user's data, the data from the other users on your service, whatever) that makes your application unique.  In this case, your application is just another portal to access your data.  There are other ways to stand out, of course, and there's still room for truly unique apps, but this is the most common route.

2) If you have such a service, and you have data that your user cares about, your user is absolutely going to want to have access to it on the go.  Smartphone usage is growing explosively, and the sort of high information users that are going to be early adopters are even more likely to be smartphone users.  You will need to have a mobile strategy of some sort, full stop.  You might not need to execute on it right away, but you should at least be thinking about it.

3) If you can avoid writing a native application, that's good.  But the state of technology for other options isn't great right now, especially if you care about users who are not iOS or Android users.  A usable mobile website helps here, and can be one part of your strategy, but probably is insufficient on its own.  The tradeoffs involved in native application development vs. HTML 5 vs. cross-platform development frameworks are significant and are best evaluated by your technology staff.  But the rule of thumb is that the richer you want your mobile experience to be, the more likely it is you will have to bite the bullet and write a native app and the less likely it will be that a cross-platform framework will be sufficient to accomplish your design.


## Answer 21569

- posted by: [Justin C](https://stackexchange.com/users/-1/6947-justin-c) on 2011-03-14
- score: 0

<p>You either need to have programming experience or be ready to do a lot of studying. There are tons of great websites to learn more, like answers.startups sister site <a href="http://android.stackexchange.com/questions">http://android.stackexchange.com/questions</a>. Mobile programming has it's rough spots like web services programming, server programming, and desktop programming. For the most part the tools are getting better but the world of possible solutions is getting bigger.</p>

<p>As for what platform to develop for, I would recommend simplifying your interface to work on both platforms, using a system like <a href="http://en.wikipedia.org/wiki/Appcelerator_Titanium" rel="nofollow">Appcelerator Titanium</a>.</p>

<p>If you want any more details about mobile programming I would take it to a site like stackoverflow.com.</p>



## Answer 21574

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2011-03-14
- score: 0

Uniqueness isn't restricted to the boundaries of desktop app, mobile app, web app... 

On the contrary, some people build an app around an IDEA. The idea can then be accessed through desktop, mobile, web applications. See "Mint.com" for instance. The idea there isn't bound to a "mobile" or "desk" definition. It's an app that an be used from everywhere. Twitter too. 

Some apps do need the unique features in mobile - the ability to make a call, GPS geo-location services etc. All the rest can easily become ubiquitous applications.

Don't think about the PLATFORM  that you're going to implement for. Think of a SOLUTION to a problem, or an APPLICATION that you'll develop and only THEN think about platforms. Think about how people will use it, rather than on what. 


## Answer 21655

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-03-15
- score: 0

If you are going to develop a mobile app, i think its best to code it in HTML JS CSS as an app for mobile devices.  

That way you dont have to program it in AIR for Playbook, Ob C for Iphone, and whatever droid uses.  Probably make more money with ad placement then you would with app purchases. 






---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
