## E-Myth Revisited - how does it apply to an ISV startup?

- posted by: [Ryan](https://stackexchange.com/users/-1/465-ryan) on 2011-10-21
- tagged: `management`
- score: 3

A few people have recommended the "E-Myth Revisited" book to me (and its on Joel reading list IIRC) and it gets very consistently good reviews.

http://www.amazon.com/Myth-Revisited-Small-Businesses-About/dp/0887307280

I struggled through the hubris, the excruciating dialogue and misuse of capital letters and was left with...

"Work on your business, not In it."

Most of the wisdom was about procedurising everything so it can be followed by anyone to create predictable results - McSoftware.

Struggling to see how that can be applied to an ISV? Apart from the 'obvious' stuff about unit testing/source control/continuous build etc I am at a loss for other actionable insights.

What am I missing?


## Answer 31889

- posted by: [Kenny Evitt](https://stackexchange.com/users/-1/7597-kenny-evitt) on 2011-10-25
- score: 3

I think you're missing how "... procedurising everything so it can be followed by anyone to create predictable results" does not in fact lead to "McSoftware". Your 'procedures' don't have to be actually executable by a computer! Think of these examples:

1. A support tech (you do have people answering phone calls from your customers, right?) takes a call from yet another irate customer because your hosted web-service (or hosted web-app [who still provides a 'local install'?]) is down.
2. You need to implement and deploy a hotfix for a mission critical bug for your largest customer.
3. While your developers are working on the next feature-sprint, the pool of unresolved bugs in your support system (you do have a support 'ticket' system, right?) is growing faster than your support techs or support developers can resolve them.

Now – what do these people do in these situations? And how do the managers or owners of this startup know what's everyone's schedules and priorities are and whether they need to be adjusted? How can all of the requisite _data_ be collected so someone can even _estimate_ this info? Here are some example procedures, in response to the example scenarios listed above:

1. Your support techs know [and they were taught via the procedure "read this document ..."] enough about the web-service or web-app to know that the problem affects all of your hosted customers; they add a comment for the relevant ticket in your support system that the customer called and they lookup the latest comments in the ticket assigned to the tech or developer that's working on fixing the problem to learn that they estimate that the problem will be fixed in 30 minutes. When the problem is fixed, all of the relevant support techs are notified so they can then call all of the soon-to-be-less-irate customers.
2. The relevant tech or developer creates a hotfix branch based on the release version for the affected clients. They check-in, build, and test changes using only that branch, and when it's deemed ready, it's deployed to the relevant production environment [itself another 'procedure'; hopefully some of these really _can_ be executed by a computer!].
3. Gary [huh?] is responsible for reviewing the pool of unresolved bugs in your support system each week – and techs know to escalate sufficiently important or urgent bugs before then! – when he notices that several bugs pertain to an area of your software for which recent changes were released, he pulls the relevant developers off of their new-feature projects to fix several related bugs.

The benefits of 'proceduralization' is that everyone that knows those procedures can then _cache their decisions_ and everyone else that knows the same conventions can also easily know what to check to determine who's done what, when, why, and how. Procedures can be committed to mental 'muscle memory' so everyone can figure out the _really_ hard problems of your business, instead of things like:

- What should I name the build output folder for the latest version of the app?
- Should I create a branch in source control for the latest feature I'm developing?
- Who should I notify when a project or task I'd previously estimated as requiring 3 hours will now require 6?
- How should I layout the controls on this form?
- Should I name this table 'clients' or 'Patient'?

The Ruby on Rails community calls this same general pattern [convention over configuration](http://en.wikipedia.org/wiki/Convention_over_configuration). The point is to remove unnecessary decisions by adopting conventions (procedures, 'best-practices', etc.).

But don't forget that there are 'meta-procedures' which are responsible for reviewing _and adjusting_ all of the other procedures as appropriate. There's nothing wrong with doing things differently, but it's _immensely_ valuable to have an in-place way for everyone to do the common, routine tasks that make up a lot of the time working for a software company.


## Answer 31908

- posted by: [Aymeric Gaurat-Apelli](https://stackexchange.com/users/-1/4785-aymeric-gaurat-apelli) on 2011-10-26
- score: 1

It means:

**Systemize your business procedures**

List all the things that you do every day. If you'd leave for one week, what are the essential things that would require your presence?

Some examples of procedures can be: 

- How to get more clients
- How to market a new product before launch
- How to do bookkeeping
- How to do annual tax report
- How to answer a customer

**Delegate or outsource what can't be automated**

Now that you have a documentation of your business, you are one step closer to be able to get someone else to do part of it for you.

**Working on your business**

Working on your business is looking at your business like a product that you are trying to sell. What things would you do if you had in mind to sell your business in a few years?

You'd probably make sure your finances are tidy, your web accounts are documented somewhere, you have more than one revenue stream, subscription preferably, etc.

Disclaimer: I run an outsourcing marketplace, and I am about to launch a product that helps people document their business processes.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
