## Ideal iPhone App Developer Team

- posted by: [Cluelessbear](https://stackexchange.com/users/-1/5170-cluelessbear) on 2011-01-17
- tagged: `website`, `development`, `iphone`
- score: 0

I'm planning to develop an iPhone application that will connect to facebook and our own company website.

I know that I will need a developer for this. But what's the ideal team to get this kind of project launched successfully?

Thanks in advance guys :)


Jay


## Answer 19148

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-01-19
- score: 3

<p>The core team (if there's no significant web service back end, which it sounds like there wouldn't be) is typically:</p>

<ul>
<li>A developer (with understanding of design)</li>
<li>A designer (with understanding of development)</li>
</ul>

<p>In iPhone, it's often the designer who anchors the team. Whether that's an anomaly or a sign of a long-term shift is an interesting question - but for now let's steer clear of that rabbit hole!</p>

<p>Technology-wise, you have some choices on how to go. </p>

<p>The apparent default choice is to build a true native app from the ground up. The development environment is famously unloved, but plenty of people out there have developed the skills and are hammering out apps.</p>

<p>For me, the real default choice is to leverage HTML 5's ability to deliver app-like experiences that access services from the phone. Typically, this means that the native app is a simple loader using a Safari instance - and you can prototype and refine as rapidly as you do for regular websites.</p>

<p>This works well in a surprisingly large number of cases, and delivers some great benefits. Covering multiple platforms is far easier, and routine updates don't require app store re-submission as the app itself doesn't have to change. </p>

<p>Another approach to multi-platform development that leverages web technologies but creates native apps is to use <a href="http://www.appcelerator.com/" rel="nofollow">Appcelerator's Titanium</a>. This allows you to target both iPhone and Android, and either avoid native coding altogether or confine it to modules accessed from your app.</p>

<p>And finally, it's worth mentioning <a href="http://monotouch.net" rel="nofollow">MonoTouch</a>, which lets C#/.NET developers create iOS apps - which gives you access to a vast skill base. This is a great solution if you have those skills in-house. You'll probably still go out-of-house to execute the project, but you will have the option to bring the maintenance and ongoing development into your team.</p>

<p>Those are technical choices. Meanwhile, I'd recommend you use a wireframing tool such as <a href="http://balsamiq.com/" rel="nofollow">Balsamiq</a> to turn your plan into something visual. If nothing else, this will help you through some of the thinking about what's important to you. Even if this changes beyond recognition (and experienced app developers will often lead you through thinking that turns your ideas upside down!), you have a common reference point. Too many app projects produce disappointing outcomes because the specification is either way too loose (so the new team is guessing at the ultimate success criteria) or way too prescriptive (so you get what you ask for but not what you need).</p>

<p>Good luck with the project. If all these choices seem like too much, start out with the default (HTML 5) and change when and only when you have to.</p>



## Answer 19069

- posted by: [Fred](https://stackexchange.com/users/-1/6384-fred) on 2011-01-17
- score: 0

If you're going to use one of the freelance websites like elance or odesk, you can search for mobile app developers and find plenty.  Also, you can ask your question *inside* the job posting and get lots of free advice that will also help you to ascertain the level of expertise of applicants.  If your project is big, you might even want to post a job for a project manager.

I would also recommend getting a book about mobile app or iPhone development and read through it.  You don't have to do the exercises or learn programming in detail, but having an idea of what goes on behind the scenes will help you to 1)know whether the person/people you hire are professionals, 2)know whether the person/people you hire are billing you fairly, and 3)probably save you money by enabling you to more effectively communicate what you want done (thus avoiding lots of rewritten code).

Hope this helps.


## Answer 19141

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-01-19
- score: 0

You know a lot doesnt have to be done by an IPHONE developer.  you could just build a good old HTML app with that supports mobile resolutions.

The reason this is attractive is that you dont have to build 1 for iphone, one for droid, one for blackberry, 1 for ipad, and so on.  Too bad Iphone sucks when it comes to accepting flash because flash would be a great way to do this (The reason for flash is Jobs knows that everyone would rather code apps in flash, killing sales for those who have to buy macs to build native iphone apps, and also killing the apps marketplace, or putting a big dent in it).

You could just hire a kick ass HTML (HTML5) CSS designer and tell them to design your site for Iphone.  Its easier to update, its easier to manage, its probably cheaper to code, and will give you greater coverage.

Go with a native app if you need something complex, or need to support users when there is no wifi, or net connection.

Best of luck.


(PS, jquery touch framework is pretty cool!) 




## Answer 19146

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2011-01-19
- score: 0

It depend of the type of the application you are trying to build. For example if you are building a game for iPhone, I would say you need:

- developer
- graphics designer and probably musician.

If you are building application that just connect to Facebook, you just need a developer with good enough skills.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
