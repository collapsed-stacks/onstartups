## Can a consumer oriented startup be .NET based?

- posted by: [Asaf R](https://stackexchange.com/users/-1/7422-asaf-r) on 2011-03-09
- tagged: `venture-capital`, `microsoft`
- score: 6

I'm about to join a new startup as their CTO and we need to choose our server software stack. The client side is a mobile application (Android, iPhone, etc.) so the server side exposes an API and little to no UI.

My experience is mainly with the Microsoft stack which is why I'm leaning towards using it for our server development. However, we were told this would be frowned upon by potential valley VCs. We were told to go with "anything open source", such as PHP or RoR.

- In your experience, is a consumer oriented startup based on Microsoft technologies something frowned upon by VCs?  
- Is the Microsoft option really more expensive given BizSpark and the advantages of a single vendor?




## Answer 21304

- posted by: [Filippo Diotalevi](https://stackexchange.com/users/-1/4482-filippo-diotalevi) on 2011-03-09
- score: 7

I don't think VCs should care about the technology stack you are using too much. Sure, I've heard some of them saying "we think our startups should be using RoR/Python, not Java", but I honestly don't take them too seriously. There are examples of startups using .NET, and Stack Exchange/Stack Overflow is one of them.

I'd say: at the stage when you are ready to talk with VCs, you have already proved you can build the product, run it and can serve a good amount of users. So don't worry about that, just choose a technology you know well.


## Answer 21310

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-03-09
- score: 3

If your Microsoft experience means you've been building great apps for the past 5-10 years and you can do one more in your sleep, then stick with it. VC's would be more impressed with that. 

Otherwise, consider the licensing fees (SQL Server can get expensive at the Enterprise Level), and the skill sets of developers you can most likely recruit. Are those that have been involved with Open Source projects more willing to join your firm and take stock options over salary?

Are you located in Silicon Valley, have had a previous startup (success is optional), and went to a top ten university? I hear they like that as well. Might as well go all out.


## Answer 21305

- posted by: [luis.espinal](https://stackexchange.com/users/-1/8395-luis-espinal) on 2011-03-09
- score: 1

I think you were told bullshit. A VC shouldn't care what you use to build your products, only that you can (and that you have a sensible business plan.)


## Answer 21318

- posted by: [Levi Figueira](https://stackexchange.com/users/-1/6511-levi-figueira) on 2011-03-09
- score: 1

Sorry to break it down to you, but it's sounding like they're just using that as an excuse when they might not have any intention to fund you.

Now, given that, going with Microsoft tech for web development is not very smart. Microsoft has failed repeatedly at even being a significant player in the web so why would their tech be any good? In the same way, maybe the reason why so many startups are using RoR et al is because it really is a lot more efficient *and* cost-effective.

It all falls back to this:

 - You should just build whatever it is you're building. Don't worry about funding and/or technology. Just build it with whatever tech you're comfortable with.
 - Be ready to learn new technology as the business develops. Be willing to refactor. Be ready to even build version 2.0 from scratch in a completely different language/framework.
 - Once 1.0 is built and shipped, tinker with alternative languages and frameworks. Ruby/Rails and Scala or Earlang are good examples of languages that are used together quite a bit within the same app, for different tasks.

Most of all, keep an open mind about what is the most practical solution and what is the best solution. 1.0 should always be the practical. Worry about the "best" (ever-moving target) after you ship and just plan on incremental changes for the life of the code.

Good luck. :)


## Answer 21321

- posted by: [Tony_Henrich](https://stackexchange.com/users/-1/5619-tony-henrich) on 2011-03-09
- score: 1

You can build anything with .NET. I am a .NET developer. I think the biggest concern is licensing fees and its added cost. If you have many servers as backbone to your business, you will have to consider the costs of license fees for Windows Server, SQL Server.. and the other server software from Microsoft. Maybe that's what VC's might be concerned about.

With a LAMP stack for example these server software are potentially free. Linux, MySQL... etc.


## Answer 21326

- posted by: [Stuart](https://stackexchange.com/users/-1/8316-stuart) on 2011-03-09
- score: 0

I think you could spin the .Net angle to a benefit if you wanted to - there are startups on Microsoft - StackExchange is a prime example!

There's also a Mono angle you could use to reduce server costs and there's plenty of Windows supported database stacks (e.g. MySQL). If you do wanted to, you could also leverage MonoTouch and MonoDroid - and MonoWebOs? - for app development.

To me, the bottom line is that hosting costs are generally not the major determining factor for your Startup - salaries and marketing costs are likely to be the highest factors for at least the first year. After that, if your technical architecture can scale at a cost which will mean the business plan is profitable, then surely that will persuade the investors. 

Good luck - and hope you enjoy the new job 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
