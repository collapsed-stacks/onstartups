## What are the top problems (and solutions if they exist) with outsourcing software development overseas?

- posted by: [ClayNichols](https://stackexchange.com/users/-1/3534-claynichols) on 2012-01-30
- tagged: `outsourcing`
- score: 4


I've tried outsourcing software development (I'm a developer but don't have time to do all that I need to).

Some issues I've had:

* Poor Unit Testing skills : the developer does not test the units they code. Or does not test them very well. Has not thought through the testing. Just sends it over and says "what do you think?"

*  They don't understand the task and just make their best guess. When outsourcer says "yes" they may mean "yes, I heard you".

*  Don't read and implement the spec fully.
*  Their time is split b/t you and another customer(s) so they are always "context switching". And they may just stop working on your project for a few days. This is mostly a problem if they are not extremely well organized.



## Answer 35468

- posted by: [Dmitry Leskov](https://stackexchange.com/users/-1/2093-dmitry-leskov) on 2012-01-30
- score: 5

I've been on the other shore of that sea since 1995 and can tell you that  __communication or lack thereof__, especially at the early stages of the project, __is the single source of all problems__. This includes selecting an incapable provider based on a brief interview, not checking references, not propagating user feedback to the contractor, and so on.

__Poor of insufficient communication results in wrong assumptions, misaligned goals, and expectations that do not match each other on both sides.__ Don't you think your project would be doomed if you had such problems with your in-house team?

Otherwise, if the skill set is right, the compensation is right, both parties share the definition of the success of the project and are committed to it, there will not be more problems than if you hired a telecommuter.

For instance, we have a four-people team working on a very roughly defined project right now, with much success - we are already on version 2.1 and our client's customers love it. Moreover, the project lead is also a consultant working remotely from a third country. What we do is we have regular on-site planning meetings with him and constantly stay in touch over Skype. Having the right infrastructure in place (issue tracker, wiki, build server) also helps.

**P.S.** You may also wish to check out the book "<a href="http://www.softwarewithoutbordersbook.com/">Software Without Borders</a>" by Steve Mezak - I have just noticed it is now freely downloadable in PDF format.


## Answer 35460

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2012-01-30
- score: 3

People that I have worked with say that outsourcing overseas can work well, but it depends upon the circumstances.

In general, it seems that you have to be incredibly precise in specifying the requirements, as they will obviously not understand your business culture, and may not even be aware of location-specific regulations, etc.

Also, it can be very hard to ask for changes to the specifications, as new requirements come to light, without costs spiralling out of control.

Overall, it seems to be a severe lack of flexibility, which is just what you'd expect really.

If you know what you want, and you won't change your mind, it is probably a good thing. However, in my thirty years of experience in working for business clients in various industries, I have never known a client who really knows what they want on day one. Mostly it is a process of discovery, and so outsourcing is not a good solution.


## Answer 35464

- posted by: [Chris Lively](https://stackexchange.com/users/-1/1306-chris-lively) on 2012-01-30
- score: 3

To me, the Number One issue is the quality of what you get back.  Think about how most of those overseas operations work:

1. Receive spec.
2. Deliver code so that meets spec.


The first issue is generally with 1.  You have to be able to define exactly what you need.  Any deviation from your expectations and what they produce is the result of a bad spec.  For example, you might have stipulated that the back end is SQL Server.  And they code it to take advantage of SQL DataCenter....while you were thinking SQL Express.  Be specific; very very specific.

Often times it takes almost as long to develop the spec as it would to code the thing in the first place.   If you are a lone developer I'd encourage you to simply hire local talent that can roll with you.

The next issue is with number 2.  These people are paid by their productivity, specifically, paid by meeting the spec in the quickest way possible.  

If it is easier to copy / paste an existing page versus abstracting the logic in a reusable container, then they are going to copy / paste.  Code quality, unless it's written in the spec, is not a concern.  

I've run into numerous projects that started overseas whose code base was ludicrously large and buggy because the dev's simply don't have any concept of how to properly structure code for reuse.  This isn't just an "overseas" issue but rather one due to low quality programmers.  You will get exactly what you pay for.

For me, the only time I would consider outsourcing to another country is if I ultimately didn't care about code quality.


Having written the above, a great way of thinking about it is that the overseas guys are just like a bunch of computers.  The more specific your instructions the more likely it is you will have a good outcome.  Otherwise: Garbage In, Garbage Out.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
