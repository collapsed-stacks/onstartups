## Is it feasible to manage 3 to 5 developer interns at a new startup without being in the office?

- posted by: [Thierry Lam](https://stackexchange.com/users/-1/23979-thierry-lam) on 2013-02-12
- tagged: `interns`
- score: 6

There's a brand new startup which has a lead developer. The other co-founders who are not technically savvy are thinking of bringing in 3 to 5 developer interns during the summer because the government pays for their salary. The lead developer also doesn't work full-time for the startup but part-time.

How feasible is it for the part-time lead developer to manage 3 to 5 interns without being in the office during day time?


## Answer 47348

- posted by: [CaseySoftware](https://stackexchange.com/users/-1/11314-caseysoftware) on 2013-02-12
- score: 15

It's not feasible.

Check out the Mythical Man Month. It talks about almost this exact situation in great detail. When you have someone who knows the system, project, etc and you add someone new:

 - the *total* knowledge of the team hasn't changed but the *average* has dropped by 50%.
 - the amount of time spent on communicating that knowledge increases immensely therefore slowing the progress of that first person.

It leads to the adage of "adding new people to a late task only makes it later."

And that all assumes that they're perfectly competent team members who just don't know about the system.. you're getting people who have probably never even been involved in a real site/project in the real world.


## Answer 47342

- posted by: [cdkMoose](https://stackexchange.com/users/-1/12756-cdkmoose) on 2013-02-12
- score: 13

To me, this sounds like a recipe for disaster:

 - A single intern requires a reasonable amount of active mentoring, 3-5 interns could easily take all of the time of your lead developer.
 - This is a startup, so I would wager that the technical vision for the company is not fully fleshed out.  I don't think you want a team of interns with limited technical leadership making those decisions. 
 - In my experience, I would not put mission critical development tasks in a team of interns.  I would consider adding interns to an existing stable team.


## Answer 47359

- posted by: [Adonis](https://stackexchange.com/users/-1/23990-adonis) on 2013-02-12
- score: 1

If you do not have someone to manage and overlook the code generated (even when you are co-located) you will find yourself in a lot of trouble with whatever app produced. 

I would advice against it.  Just be saying the word "interns" you are basically have to teach more than produce, so get less interns if you can.

If you do expect the following:

 - Code rewrite of segments made by interns at a later stage.
 - Slowing of the work beyond what you have today.
 - Lead developer not be able to bring everyone up to speed (5 to 1 ratio)

You can however bring them if you want to write documentation, have already Unit Tests that will catch issues in code, conduct code reviews every 1-2 weeks (assuming you are doing some kind of agile development)

Hope this helps..

 


## Answer 47454

- posted by: [stevejpurves](https://stackexchange.com/users/-1/22372-stevejpurves) on 2013-02-15
- score: 0

It won't work..

. For the very good reasons in the other answers, which do all assume that they will be working on an existing system.

If these interns are going to be brought in why not, remove the management burden on you lead dev forgetting about the manage them bit,  give them a real problem(s) that is important to the business, and let them solve it any way they can, independently from current systems / code base etc... 

Seems a better way to utilise them, see if they can innovate around your current approach to the problems, even if what they produce isn't production quality, you may learn from their solutions.

disadvantage is a possible time sink for non technical people in the startup in describing the problem domain.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
