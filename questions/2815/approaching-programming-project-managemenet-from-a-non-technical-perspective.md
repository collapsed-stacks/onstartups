## Approaching Programming/Project Managemenet from a non-technical perspective?

- posted by: [Jaret Manuel](https://stackexchange.com/users/-1/1148-jaret-manuel) on 2009-10-30
- tagged: `co-founder`, `software`, `project-management`
- score: 2

I recently asked a question of should I start dabbling into programming or should I stick to what I am good at: Sales, Marketing, Planning, Presentations, etc.  The feedback was overwhelmingly pointed at sticking to what I am good at which is what I thought but I figured I would ask anyways.  
My next question is trying to figure out the crazy art and science of understanding programming from a project management approach. I have read 37 signals Getting Real which I really like and I want to build upon that approach.  I guess what I am trying to ask is what sort of programs should I be seeking on the back end or will it always vary?  What sort of skill sets should I be seeking in a technical co-founder?
My understanding from 37 signals Getting Real is that you sketch/mockup (paper or Balsamiq, etc) to HTML and basically get to a front end design and then work the back end design from there. That is where it starts to get fuzzy for me in what I should be looking for at that point but I have a feeling it will always vary based on the situation at hand. 
I am trying to tighten that high level knowledge of managing a project and any pointers would be appreciated. Thanks. Jaret 


## Answer 2839

- posted by: [Jeffrey Hicks](https://stackexchange.com/users/-1/1090-jeffrey-hicks) on 2009-10-30
- score: 2

A common backend for web based applications is the [LAMP Solution Stack](http://tinyurl.com/yhe5nau)

* Linux (Operating System)

* Apache (HTTP Server)

* MySQL (Database)

* PHP (Scripting Language)

Its worth noting that LAMP comes in many flavors.  For example, an analogous flavor that would appeal to programmers that subscribe to 37 Signals would be:

* Linux (Operating System)

* Apache w/ Phusion Passenger (HTTP Server)

* MySQL or PostgreSQL (Database)

* Ruby On Rails (Scripting Language and Development Framework)

In addition to knowledge and skills with these basic components of a backend, you might specifically seek out skills with: 

* [Agile Methodologies](http://agilemanifesto.org/) - don't be fooled by the lame site design

* [Database Design](http://en.wikipedia.org/wiki/Database_design)

* [Scaling](http://railslab.newrelic.com/scaling-rails)

* [Security](http://www.rorsecurity.info/)

* [Testing](http://guides.rubyonrails.org/testing.html)




## Answer 2860

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-31
- score: 2

As the non-technical part you may be managing the development team, but your tech co-founder should actually be responsible for the technical part. You would ensure that he has electricity and perhaps the hardware that is needed, but other than that, your responsibility should end.

You should have an idea about different ideas in development, and if you want to see how some of the best programmer around think you can read "Coders at work". So far it is truly fantastic.

You should understand the jargon, so be aware of what agile methodologies are, and what parts you may or may not like. For example, pair programming has it's uses, but you may not want to use it exclusively.

For frameworks and languages you could look at Java and it's frameworks, such as Spring, WAMP (Windows, Apache, MySQL, PHP) which is like LAMP, just a different OS.

But, your tech partner should be making the ultimate decision, though you may want to have a discussion as Windows or Linux will have different costs, and the availability of developers will affect the rates.

You should be focusing on how to help market the application, and helping to decide which features must be in before it can start to be used by internal, or alpha testers, as the feedback from testers should help drive what features may need to be modified/added/removed. That info would need to go back to the tech partner.


## Answer 2873

- posted by: [Nathan Kontny](https://stackexchange.com/users/-1/973-nathan-kontny) on 2009-10-31
- score: 2

<p>Take any technology you think you are going to be using in your endeavors and try it yourself first: </p>

<p><a href="http://37signals.com/svn/posts/1296-do-it-yourself-first" rel="nofollow">http://37signals.com/svn/posts/1296-do-it-yourself-first</a></p>

<p>Your not going to become an expert or do very well at it, but that's not the point of the exercise.  It's about having empathy for your partner and the people you manage.  And sharing some of the same language.  </p>

<p>Afterall, <a href="http://blog.inklingmarkets.com/2009/10/how-successful-would-football-coach-be.html" rel="nofollow">How successful would a football coach be without ever having played a single game of football?</a></p>



## Answer 2848

- posted by: [Gabriel Hurley](https://stackexchange.com/users/-1/1005-gabriel-hurley) on 2009-10-30
- score: 1

There is no right solution for your technology choices. LAMP (as mentioned by Jeffrey) is quite common, but you could just as easily find yourself working with Python, Ruby or ASP.net *which is what the StackExchange sites are built on, btw).

Your description of the software architecture process is *one* way to go about it, but that particular model tends to work best only for fairly simple web applications. For complex projects you'll probably want to really think through all the ins and outs of your application, figure out your data models, and worry about the layout/design of the site a little later on.

All in all, make sure your technical partner has a solid background (doesn't have to be a CS degree; more important is what they've actually *done*).

One last piece of advice: try to avoid reinventing the wheel. That was one of my constant mistakes when I was new at programming. There are innumerable frameworks, plugins and modules for any programming language that people have spent hundreds of hours on so you don't have to. (just make sure their license permits commercial use)


## Answer 4742

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2009-12-08
- score: 1

Managing any project, independent of technology or type, really revolves around 4 things:

 - Plan: You have to have a plan on what you want. It really does not matter if it's the space shuttle or a piece of code. The plan has to have what you want to build and what defines success
 - Execute: Doing something always moves thing forward. Even if your plan is not solid, doing something will show you where your weaknesses are.
 - Monitor: Defining and monitoring what is critical to the projects success is what managing is all about. Define up front what success and monitor your progress towards it.
 - Adjust: Projects always need adjustment. Being rigid in approach or what success may be will only frustrate your team. Adjustments should always be in the best interest of the project and the team.

Your background in planning and sales should at least give you the first 2. The other thing to remember is that technical people need to be guided, not ordered around. Give them the goals of the project and let them figure out how to make it work. Support them by removing barriers that are in their way. That will gain their respect.






## Answer 2847

- posted by: [Max Cameron](https://stackexchange.com/users/-1/293-max-cameron) on 2009-10-30
- score: 0

<p>Honestly, don't worry about technical implementations - that is what your technical partner is there for in the first place. The best way for you to understand programming from a non-technical approach is to understand the functional aspect of your application. That means deciding what your app does, the interactions it incorporates, how it serves its users, how it communicates with its users. </p>

<p>So my advice is, get good at the 90% of everything else that a programmer can't do in a technology company. Trust me, 90% of running a technology company has nothing to do with programming. My company's blog is a good place to start. You can also check out Hacker News, which has a lot of articles about being a non-technical partner. </p>

<p>Best, </p>

<p>Max 
the non-technical co-founder of <a href="http://bigbangtechnology.com" rel="nofollow">Big Bang Technology</a> in Toronto. </p>



## Answer 2901

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2009-11-01
- score: 0

<p>I agree with Nathan. When possible, do it yourself first. If programming seems to hard for you, <a href="http://blog.scrum8.com/2009/nov/01/why-django-perfect-choice-startup/" rel="nofollow">you might want to try out django first</a>. It is built by people with journalism background. If he can do it, you should be able to do it too.</p>



## Answer 4739

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2009-12-08
- score: 0

The best part of your question I came up with is you are looking for a technical co-founder. You may know of someone who is technically skilled but not be interested. This person could be a guide/consultant to help you find a candidate.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
