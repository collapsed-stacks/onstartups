## How to deal with the technology side of a startup, or scale a technologically-oriented startup?

- posted by: [Aerovistae](https://stackexchange.com/users/-1/17844-aerovistae) on 2013-01-01
- tagged: `technology`, `technical`, `it`
- score: 0

This is two questions in one, but they're so closely related that they ought to be addressed together.

A. If I were founding a non-technological start up -- say a financial services group -- how would I go about setting up the IT side of things? As it happens, I'm a comp-sci major, and I'm far from computer ignorant. But that's beside the point-- unless I were a true guru, I still most likely wouldn't know the full range of technologies needed and how to set them up as a cohesive corporate framework -- company email, databases and servers, company website and its interaction with the servers and databases et cetera, security -- the list goes on.

When someone is starting a company that's going to need all that stuff (as many companies do), and they *are* computer ignorant, how do they manage it? They wouldn't even know who to hire, because they wouldn't know what skills they need. How is this done?

B. If I were starting an entirely technologically-oriented company, i.e. one which operates around a website -- let's imagine an eBay imitator -- how do I scale? For instance, Google was started by two people out of a garage with a server or two. And now obviously they have dozens of warehouses' worth of servers and databases. What's a good place to start? Just set up a personal MySQL server and work with that until you outgrow it, then hire professionals with the necessary skills to scale you up without losing any information or compromising security along the way?


## Answer 47107

- posted by: [user23843](https://stackexchange.com/users/-1/23843-user23843) on 2013-02-02
- score: 1

B.) You almost had an answer in your question.

 1. Since you are into technology, 

 i.) create your own servers and manage from your home office.<br>
 ii.) Get a hosting account that can provide you the technology stack you are looking for and configure and deploy according to your needs. If you need full control get a VPS account.

 2. As your product/site gains traction, go for any of the services like Amazon Web Services. You need to finish the research where to go much before you might want this account so that you have expertise to setup ASAP. To be even better equipped create the stack but switch off all the instances and just pay the bare minimum fee to maintain your account. As others suggested, just sit and flip the switch to scale when you are in need.

The cost for technology for a startup is initially high compared to your revenue. But, as you grow the cost of it will considerably go down compared to other expenses. So concentrate on your growth. If your idea is an instant hit, you can go to option 2.) immediately.

Good Luck!


## Answer 45401

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-01-02
- score: 0

Quick answers:

A) One hires a local PC / tech services company. Depending on how many people / technical savvy on staff, setup / training / on call service agreements are signed to keep business flowing.

B) How to scale is the last question one should ask when starting out. More important is validating what your product / market / opportunity is, then addressing the scaling issue when it becomes necessary.  Yes, you need to make sensible choices at first, but typically what you start with to support 10's of customers isn't remotely similar to what you deploy to support 10M customers. Cash  enables you to consider alternative approaches unavailable during lean times. 


## Answer 45403

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2013-01-02
- score: 0

A) I would employ a "IT/Business Analyst" type person to help.  To find them I would search for companies that help you set up Google Apps for email, docs, etc.  That would give you someone that understands using cloud technologies and services for businesses.  They likely would then be able to help in other areas like that too (eg. accounting tools, CRM, etc.)

As for how people find them, I don't think they do.  That's why so many companies have terrible IT infrastructure and systems.

B) Use cloud services to host your application/website.  Try Amazon Web Services for example, or a fully managed service like Heroku.  This way you can "flick a switch" to increase capacity.  In practice it's not as simple as "flick a switch", but it's as close as you get.




## Answer 47090

- posted by: [CaseySoftware](https://stackexchange.com/users/-1/11314-caseysoftware) on 2013-02-01
- score: 0

Those other two answers are the ***correct*** answers but not what happens on Day One.

Usually when someone gets an office space, there are one of two things that happen:

 - The space is already run for network access. Then - unless they know the right answer from above - they call the local ISP (Comcast, Verizon, etc), get that activated, plug their computers, printer, etc and call it done. There's no plan in place to "design" let alone manage or maintain the setup.
 - If the space isn't run for network access, they go to Best Buy and choose an access point *or* their ISP just gives them one for $X/month. Then repeat all of the above.

Once things become a mess and/or there's a major failure, they hire the local IT/business services group to do the ***right*** thing.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
