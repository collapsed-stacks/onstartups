## How much time should we spend on the technical documentation/design?

- posted by: [Wil](https://stackexchange.com/users/-1/3747-wil) on 2010-07-09
- tagged: `design`, `development`
- score: 4

So I'm in a little bit of a tug of war with some other cofounders on our project.  We've just started out after spending alot of time on the BP and that side of things.  The other developer/cofounders are from corporate backgrounds.  

I'm really trying to move forward with an extreme agile methodology (very basically the newer development paradigm which focuses on quick development/release, get feedback and keep iterating that cycle over planning) in trying to get our product prototyped.  They feel the need to document everything, do use cases, full test cases etc.  Can anyone help with resources to point out that this is a waste of time?  Or do you think I should be spending time documenting all of this stuff that way?  (I know how to do UML and all that fun stuff, but in my mind, we should build a decent architecture and then start delivering on the prototype)

(was debating if this should even be posted on here, but I think it makes sense here than somewhere like StackOverflow)


## Answer 12631

- posted by: [user1377](https://stackexchange.com/users/-1/1377-user1377) on 2010-07-09
- score: 3

Developers are trained to avoid "code debt", particularly in profitable enterprises.  Minor bugs, extensive documentation, comprehensive test suites and so on are all important things to have in mature code, but creating them takes time.  By deferring them until you have revenue (or have at least proven that you will), you give yourself more time to actually create the product and prove people will pay for it.

Documentation and testing are insurance, protecting the investment you're making in your code and protecting your customers from problems.  Developers with an enterprise background are familiar with a process aimed at protecting a healthy revenue stream and large customer base; they frequently apply that process blindly because they don't recognize the underlying purpose of it.  Since you don't have code and you don't have customers, the level of process you describe is probably unwarranted at this stage.

Remember, it's not at all uncommon to discover that customers don't like your product, forcing you to throw a bunch of code away and try again.  It is a mistake to cherish early code.  Get it done, get feedback, and validate your idea with people who aren't drinking the kool-aid.



## Answer 12630

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-09
- score: 2

I assume "BP" means 'blueprint' here, and not an oil company?

Have you engaged with potential *customers* to the point you're *certain they want your product to look more or less as you imagine it now?* If not, then you're probably writing test cases for features that will be killed or at least substantially changed before going live.

I think you need to light a fire under the butts of your cofounders. It seems **you're all procrastinating, by doing tasks you are comfortable with, rather than engaging with customers.** Your priorities should include a healthy mix of:

 - Talking to your potential customers by any means you can; getting hard data on what the customer need is.
 - Finding ways to minimize how much software you need to write, by offloading tasks to 3rd party services, or finding mature 3rd party software (open source or closed) to build upon in your project.
 - Laying down a sensible architecture for your project, one that avoids over-engineering and builds upon proven patterns, while remaining adaptable.
 - Building minimal prototypes (think more like Photoshop or Balsamiq GUI mockups than like working code) to test on potential users.

You wrote "extreme agile". I always worry when I hear that, because it sounds like charging mindlessly ahead. You should not skimp on architecture discussions and reviews; and note that XP is actually pretty demanding on this. You should also not skimp on code documentation. But writing long test cases -- nah; better write good unit tests or possibly even automatic functionality tests.




## Answer 12652

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-07-10
- score: 2

Could this be a sign of bad things to come?

I find it unlikely that this will be the *only* way in which your business philosophy diverges from theirs.  Startups are hard enough without also having this sort of dissonance.

Food for thought...


## Answer 12629

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-07-09
- score: 1

<p>One potential angle is to spend time documenting the customer development side - there is a significant effort in the customer development iteration where you document all your hypothesis's and use this to drive development &amp; fuel customer validation.  This ties customer development and product development together in an agile fashion.</p>

<p>An image of this process can be found <a href="http://steveblank.files.wordpress.com/2010/01/scalable-startup.jpg" rel="nofollow">here</a> from this <a href="http://steveblank.com/2010/01/25/whats-a-startup-first-principles/" rel="nofollow">article</a>. More <a href="http://steveblank.com/category/customer-development/" rel="nofollow">info</a> behind customer development methodology can found here (the book is good too)</p>



## Answer 12653

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2010-07-10
- score: 1

From my personal experience, my best advice on this is to document your assumptions and write down interfaces.

Anything that has to touch an outside customer, partner or department should have a clearly defined interface document that allows the other party to be successful. If you don't do this, you will end up spending countless hours getting others up to speed -- which is a waste of time.

Your other partners seem to want more of a formal process (due to their corporate backgrounds). You should embrace the good parts of that and really strive for some common ground on what your company wants to do. In the end, it's up to the three of you to agree on what your development methods will be.




## Answer 12626

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2010-07-09
- score: 0

Documentation is very important. You should make documentation as one of the selling point of the product. Django is one of the example of that. Everybody just kept praising about its documentation. 

But again you need to brainstorm with your team what is the definition of DONE here. Does a feature counted as complete with or without documentation.


## Answer 12628

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-07-09
- score: 0

You're going to have to compromise. Go through the design process with them, but behind their back (not as nefarious as you think) write some code; just say you were restless and just had to get your code on. Show them a little something once in awhile. Developers like code and everyone likes working software. Maybe you can pick something that came up during design discussions as difficult. Have a little documentation. Maybe some sketches that you used. 

Make sure that they are not using all this talk as a way to get out of doing work. Nobody buys what's on the white board.

And yes, your code will change. Better ways of doing it will arise. Features will get dropped, but just show them how easy it is to get over that and write some more code.


## Answer 12693

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-07-12
- score: 0

You make the following statement:

> in my mind, we should build a decent
> architecture

If you think you can do that without documenting the requirements, etc, then make a case for that, but any time I have had to build anything that had "an architecture" it needed a bit more than "let's just start writing code and see if it works" kind of mentality.

You need to work this out with your partners.  Get everyone to agree on some sort of precess - whatever that may be.



## Answer 12744

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-14
- score: 0

I feel it is always better to document everything so as to avert any issues down the line. I have similar experiences earlier where we tried to go ahead cloning a product without much documentation but ultimately it lead to a serious confusion when debugging the application.

What I feel that if you can spend some time to prepare document at the initial stage (which may seem a waste of time now) it will really help you down the line to identify a problem and solve a crisis.

Any software application before launch needs rigorous testing and a product development backed by well documentation can really save your time and money.

Thanks and Regards
Dave


## Answer 12638

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-07-10
- score: -1

Documentation? it is a waste of time in my own opinion, the code is your documentation :). No one reads documentation. 

The amount of testing and planning depends on the type of project, if this is a simple non-critical application then some unit testing will suffice, remember that the real user acceptance testing will be done by your users/clients.

The way software development is done in a startup vs. the corporate world is very different. In the corporate world is all about people signing off on features, endless meetings, more features, more meetings, 6 - 12 months software development cycles (or more), etc... it is slow and not efficient at all. In a startup you have to take advantage of your flexibility and develop fast (with quality) and release the first version as soon as possible... that is the only way.

I am not implying to release buggy software... what I suggest is to release software fast by eliminating most features and leave only the basics... then let your users give you some feedback and go back and make some more changes, keep doing this until you end up with a product that users love :)

Below are some links to some great articles and books about the subject:

37 Signals - Getting Real: http://gettingreal.37signals.com

37 Signals - Rework: http://37signals.com/rework/

Paul Graham - Want to start a startup: http://answers.onstartups.com/questions/5268/what-companies-failed-because-they-released-too-early

Release Early, Release Often: http://catb.org/esr/writings/cathedral-bazaar/cathedral-bazaar/ar01s04.html






---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
