## Should I go to the basics of software development/programming before starting up?

- posted by: [user14058](https://stackexchange.com/users/-1/14058-user14058) on 2012-01-29
- tagged: `software`
- score: 3

I have an idea for a software product. But I'm not technically strong in the theory of Algorithms, Databases and stuff. i.e. 
I can manage to write code that works, but I don't know if it would scale and so on. 

So I have been learning the theory for the past couple of months, but I'm itching to start coding. A couple of my friends I want to start up with
have the same problem too (and are taking up the online free courses from Stanford :) )
and don't consider themselves as 'ready' yet .

We don't want a sophisticated MVP, but will eventually use machine learning and want to scale (like any other team :)).

Should we bide our time and get the basics right or dive into the deep end straightway and learn the hard way as we go along?


## Answer 35432

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-01-29
- score: 5

<p>Often projects are started before there is a clear understanding of many of the necessary components will be designed and built. Consider for example when President Kennedy announced in 1963 that America would put a man on the moon before 1970; there was a lot of stuff that had to be figured out before that could be accomplished. But if America had waited until everything was known before starting it would have taken a lot longer.</p>

<p>When building out a computer system it is common practice to <a href="http://en.wikipedia.org/wiki/Method_stub">stub out</a> functionality that one knows will be required but which one is not ready (for whatever reason) to develop at this time.</p>

<p>Lets take a simple example; suppose you want to build a webpage where a user enters a number and the website returns the square root of that number. You know how to build websites, but you don't know how to compute a square root (and assume you don't already have a language function or subroutine to do it). You know you will eventually need a routine to compute square roots, but you want to get started. What you do is write a simple subroutine that if you are passed 4 you return 2, 9 return 3 and anything else you return "unknown". Now you can build out the website and have it work as long as the user enters either 4 or 9. Meanwhile while the majority of your team is working on the website you can have someone else working on figuring out how to compute a square root.</p>

<p>You mention machine learning. As you know, algorithms are constantly being developed and improved. Even if you had the best possible solution today it is highly likely that you would want to change it in the future as better methods are discovered. Why not build your software product using an extremely simple algorithm (like make a random guess) but in such a way that it is easy to swap out one algorithm for another. That way when you learn something new or have a better idea you can easily implement it.</p>



## Answer 35430

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-01-29
- score: 2

If you plan to get and stay involved in the start-up, software product, technology world it is worth it to learn how to code enough to get things done.  It doesn't have to be the most elegant code, it doesn't have to be the best, but it should do what it needs to do.  

You can do a lot with just knowing the basics.  A more veteran programmer may get some laughs out of how you did it but if it works it works - especially for just getting something going. 

Most important thing is to just start. Just make something. Then refine, grow, hire better programmers then yourself and let it evolve.  

You'll see this comment a lot.  Don't worry about 'scale' today... that's a problem for if / when you need it. Re-work it when you need to, but I would urge you to learn to code and get involved at a level where you can really understand your product. 


## Answer 35436

- posted by: [Ryan](https://stackexchange.com/users/-1/465-ryan) on 2012-01-29
- score: 1

For a software startup 'the code' comprises much less of the total work and even less of what will eventually determine success, so start right now but on the other parts.

Edit - Some of the other parts :-

* Who are you going to sell your product to.
* How are you going to find them (or get them to find you).
* How much (if anything) are they willing to pay.
* How much cash will you need to run your venture.
* How you will finance that (Bootstrap or Investors)


## Answer 35445

- posted by: [Nick Stevens](https://stackexchange.com/users/-1/15902-nick-stevens) on 2012-01-30
- score: 0

Currently, the "Startup Industry" seems to be very hot on "all non-technical founders must learn to code". Personally, I find this to be somewhat puzzling. I understand the benefits of having team members that understand some level of code - but, there's also a ton of other things that need to get done, that don't require code knowledge.

Obviously, someone has to be able to write the code - but that doesn't mean you all have to learn in parallel and forget about the other stuff that needs to get done.


## Answer 35456

- posted by: [JohnTESlade](https://stackexchange.com/users/-1/14442-johnteslade) on 2012-01-30
- score: 0

Consider what the Lean Startup calls a "concierge MVP".  So rather than spending time on complex machine learning algorithms can you achieve the same results to the user by hiring a human to do the task (either yourself or maybe something on the mechanical turk).  Yes this doesn't scale but it validates you have customers for your product.

Once you have customers you can worry about the detailed algorithms and hire in the relevant expertise to build a product that scales.


## Answer 35463

- posted by: [Chris Lively](https://stackexchange.com/users/-1/1306-chris-lively) on 2012-01-30
- score: 0

I'm pretty sure that facebook, twitter and others had no idea the scale their sites would have to get to when they started.  I'm equally sure that their dev team had zero experience in building the sites up to handle the load levels they are both at now.

There is a saying "don't preoptimize".  In other words, get something out there that works.  If you are in the lucky position of dealing with scalability issues then you are doing something right and should be able to afford to hire those who can help.  If not, then it didn't matter anyway.

Incidentally, this is also why they say "release early, iterate often".  The point is to get your idea to market quickly and respond to what the market says as fast as possible.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
