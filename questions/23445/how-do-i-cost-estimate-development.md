## How do I cost-estimate development?

- posted by: [anonymous](https://stackexchange.com/users/-1/9669-anonymous) on 2011-04-15
- tagged: `software`, `development`, `cost`
- score: 1

I've developed a working prototype; interface and core functionality for a pretty complex system. (I need the prototype for capital-raising purposes and proof-of-concept.) I am *NOT* a professional programmer; it's not my gift.

It'll take significant resource to expand/refine my prototype into a full-fledged, scalable, consumer- and business-ready on-line application, for which I'll soon seek early-stage seed money. Initially, I thought I would outsource development, but have reconsidered. It's easy enough to submit RFPs to development shops (assuming I could identify the best candidates, which I'm not sure I easily could), but:

1) How do I figure out how roughly many man-hours would be required to re-code my prototype (after hiring in-house expertise)? Do I seek great programmers, for example, qualify them, then show them a modified prototype and ask "How would you program this, and how long would it take?" Should I still pursue the outsource route?

2) The application is database-intensive and performance-critical, with a rich client (Web) interface. I'm platform/language agnostic -- I just want the thing done in the "best-possible" way -- but doesn't this complicate the process of identifying best programmer candidates, or should I first settle on a platform/language stack and then find associated specialists?

3) Finally, my old-school rule-of-thumb for project management was always "best guess, then double it." If there's a decent spec. with clear parameters, do programmers actually deliver on-time/on-budget these days? Is there any reason there shouldn't be penalties if time/performance milestones aren't met?

Thanks, -J.


## Answer 23463

- posted by: [Mehdi Maujood](https://stackexchange.com/users/-1/9681-mehdi-maujood) on 2011-04-15
- score: 1

> How do I figure out how roughly many man-hours would be required to re-code my prototype?

This actually depends on how big your software is. Estimating time for completing software is far from easy and companies regularly fail at estimating them correctly. If your project is relatively small (can you imagine it being built in a couple of months? three months?), it shouldn't be *that* hard. In any case, you'll need an experienced software person to make the right estimate.

You can definitely request companies to give you a proposal. Their estimates wouldn't be too off. You can also break your software down into individual components (function points or use cases, for example) and try get yourself (or a software guy you know) to estimate the development time for each component. You can also post a brief overview of the software on some programmer Q/A place and ask them to give you an estimate. You can combine all these and get a good estimate.

> should I first settle on a platform/language stack and then find associated specialists?

If your application is complex and performance critical, then you should be concerned about the platform. The best thing to do here, once again, is post a description of the performance-critical portions on some programmer Q/A place and get their feedback.

> with clear parameters, do programmers actually deliver on-time/on-budget these days?

With clear parameters, clear requirements a clear prototype (you already seem to have that), a good programmer *should* be able to deliver on time and within budget. Bad/changing requirements and bad programmers are what I've usually seen ruining the time/budget.


## Answer 24978

- posted by: [Flignats](https://stackexchange.com/users/-1/10488-flignats) on 2011-05-16
- score: 1

> How do I figure out how roughly many man-hours would be required to re-code my prototype (after hiring in-house expertise)?

Why exactly do you need to estimate the man hours?  Will you be bringing someone in-house on on a salary to develop the application?  Or will you be contracting out the development?

If you are bringing someone into the company, then I would concentrate on the quality and confidence in your new engineer.  If you have confidence in their talent, then you are confident that they will spend the appropriate amount of man-hours to build the company the product it deserves.  

Also, no project is really that simple to estimate - especially not a 'pretty complex system' there will be new needed man hours discovered along the product development.  So, this ties back into looking more closely at the quality of your new engineer.  

If you are unsure of how to appropriately test an engineer because you are less skilled - check out using a service like http://rankmind.com - you'll be happy you did.

If you are going to contract out the development then I would go this route: Network yourself around hacker meetups and find yourself a talented, already successful, been there done that engineer.  Then get him to fall in love with your idea.  Then get him to be an advisor for your company, a tech advisor (you'll persuade him with a small percent of equity and your charm).  Now go out and find yourself that contract company for the development work.

>I just want the thing done in the "best-possible" way

Yeah, me too!  You said it yourself, you are not the expert here.  You built yourself a prototype - KUDOS! Now let's get a quality engineer and he can make the necessary tech decisions.  Of course, if your product is far enough along as a prototype then it may be too costly to redevelop in a new language.  Do a cost-benefit analysis.


>Finally, my old-school rule-of-thumb for project management was always "best guess, then double it."

If you can recruit a quality engineer that is vested (equity) in your company, then you should be able to feel confident that they will be delivering as fast as they can be.

If you are using a contract service then you will most likely want that tech advisor to your company, to spot critical errors and steer you back on the right path.  He can also help with identifying a good contract company that he trusts and give you an intro - ensuring quality work.

Hope that helps!




## Answer 23453

- posted by: [abenetis](https://stackexchange.com/users/-1/3397-abenetis) on 2011-04-15
- score: 0

1) Did you know how long it took to build your prototype? Which Percentage of the final stage is your prototype? Lets say its 10% and you needed 300 hours, then your final System will need 3000 hours + 10-20% Risk-Recognition. Just multiply the time with the rate of a good programmer.
If you outsource, you need to be very specific about what you want your System to be. If you change Milestones or Features over and over again, it will hurt your Budget hard. But it will be a good idea to let the one or the other programmer review the prototype and estimate how much time they would need to program your System.

2) It's not bad if you have a bit of a clue about the Platform/Language you like to use. There are many Programming Frameworks out there. Thus "Best Programmers" should know about some Frameworks and should be able to recommend one for your specific purpose. Frameworks will also speed up the development time.

3) IMHO it's ok to agree with your programmer on terms like deliver dates/milestones and penalties. But you should also think about Incentives you give them, like when they do it faster and better as you specified, then you should reward them.

Hope this helps. Good Luck with your Venture.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
