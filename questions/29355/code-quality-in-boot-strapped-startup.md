## Code Quality in Boot Strapped Startup

- posted by: [nextgenneo](https://stackexchange.com/users/-1/5085-nextgenneo) on 2011-08-28
- tagged: `employees`, `code`
- score: 7

I am running a boot-strapped startup with another technical co-founder and we are making revenue (not profitable yet) and things are extremely tight. We are both experienced programmers and my co-founder has experience working at one of the world's largest software companies. We both make a lot of effort to continually learn and follow as many best practices when coding (mostly .Net / webapp / SaaS). Its something we feel is really important to the long term health and growth of the company.

For instance we work hard to:

 - Use BDD / TDD / Unit Test where appropriate
 - Separate application logic from ui logic
 - Follow best practices in stuff like Code Complete
 - Follow a lot of agile / extreme programming guidelines

Obviously as we are a startup so we cut corners occasionally and no-one is perfect so we continue to learn and strive towards writing better code.

The main issue is right now we have an employee who is doing pretty much all of our css/js/html for our front facing websites (we have a graphic designer). He's been with us for about 6 months and we've spoken and tried to teach him good practices but he doesn't seem to care or want to learn.

His background is a IT/scripting where it was all about "getting it done". The positives with him are he is very cheap and does get stuff done although good luck if anyone else ever needs to work on it or we need to make any changes that aren't trivial. The stuff he is working on is all our front facing stuff that we will need to continue to improve / refine for the next few years. 

We have a policy that anyone can order technical books and everyone has a Safari Books account. I budgeted a lot of time recently for him to work through an MVC 3 book as we were porting our website over from basic Asp.Net. The book promoted all the best practices and I made him do the tutorials. He hasn't followed pretty much anything from the book with our website port and I've been too busy to enforce / go over stuff.

In the short-term this is good as it frees up the co-founder and I to do a lot more specialized complicated back end coding which would cost a lot per hour ($80+) to contract out but in the long term its really going to come back to bite us.

I guess my question is should we:

 - Keep working on trying to make him improve (code reviews etc) and if he doesn't improve  fire him if he can't learn how to code well.
 - Keep working on trying to make him improve (code reviews etc) and if he doesn't improve keep him on but don't spend any more time teaching him.
 - Try to get more money from somewhere to hire someone who produces better code and not bother spending our time trying to teach someone who doesn't / might not be capable of learning.
 - Don't worry about it get things hacked together as soon as possible and try to become profitable / make money and then worry about it when we are making $1,000,000+ rev a year (random number)
 - Any other suggestions?


**Cliff Notes**

Have a super cheap employee who does all js/css/html but produces working but crappy / unmaintainable code. Seems like he doesn't want to learn. Suck it up as its so cheap and it works? Put lots of time into improving him? Find the money from somewhere to get someone better?


## Answer 29357

- posted by: [Alex](https://stackexchange.com/users/-1/12744-alex) on 2011-08-28
- score: 3

Following best practices when coding is great, and strict adherence to them at the start can save you significant time and pain later on down the road. Having said that, whenever I go to implement something, I always try to put things into perspective and ask: is focusing on this the best use of my resources at this point in time? 

For the majority of web apps, the front-end (be it HTML, CSS, JS, whatever) is the light-weight side of the application. It is typically much, much easier to change this later on down the road versus the back-end where the application's core logic and functionality is handled.

You said it yourself that money (and likely time) is extremely tight right now. I'd recommend keeping him on given your situation, and keep trying to nudge him in the right direction, but also start making preparations to replace him in the future if he doesn't improve.

Worst case scenario, having to redo the HTML, CSS, and JS later on, shouldn't be too expensive--especially when comparing it to having to replace this guy at a critical time, deal with any fallout, and then not only having to find a new employee, but also bring them up to speed.


## Answer 29356

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2011-08-28
- score: 1

Only you can answer this question, as I'm sure you realise ;-)

Really, it is a cost-benefit conundrum.

I guess you should give your employee an opportunity to improve and be really honest with them. Tell them straight that you are not happy and impress upon them how critical their performance is.

If the stress of managing this person is too large, let them go, and do the work yourselves in the short term.


## Answer 49563

- posted by: [bhttoan](https://stackexchange.com/users/-1/23673-bhttoan) on 2013-06-18
- score: 1

This strikes me as a simple performance management issue - the fact he is a programmer is not relevant nor is that he is cheap as you are just storing up issues for the future. 

This is a business issue and one which it may appear to be easier and simpler to ignore but it is not. It is also an area which many startups ignore or neglect as it is seen as a unecessary expense and time wasted.

If you do not do something then what happens next time he decides to do something his way against your requirements or you take on new employees who either decide to follow his lead or are demotivated as they have to follow the rules whilst he does not?

Make sure you have a robust employment contract in place with clear disciplinary policies and start enforcing them or you are starting down a slippery slope.

Caveat: this assumes you are in a country/region where you can realistically enforce performance management etc


## Answer 49569

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2013-06-18
- score: 1

This is a problem.  You know it too.  It's not easy to deal with it but you do need to.

Not only is code maintance really important, but more so company culture is.  Do you want to be a company of programmers that pride themselves on their work and are constantly improving? You set the tone for your business early, don't let this be the tone you set.

As for the cost, bad code will cost you money.  It's not faster, it's not cheaper, they are justifications we tell ourselves but it's not true.

Make the hard decision and fix this problem, your company will be better for it.


## Answer 29361

- posted by: [Bahadir Cambel](https://stackexchange.com/users/-1/9645-bahadir-cambel) on 2011-08-28
- score: 0

I do think you are forcing him to the wrong rode because obviously he does not want to learn ASP.NET MVC ( or any other web frameworks) . 

Your time, energy and the money is what brings down to the lean startup. Don't forget it is not only the money. If you can pay 10 bucks more and get one without any crappy code, I do believe it is more valuable rather than going down the road with energy, time and the MONEY. But don't expect they are willing to learn. They might say yes, but test the assumption!

One more option is to teach him not to produce crap. Pair program with him to refactor some of the code. Put refactoring into the task list and be strict about it. Make it a rule or whatever suits well. Focus some of your energy on this, not the MVC part IMHO. I believe this is a long road, and I don't suggest in your case.

At the end it depends on how hard the problem you are solving at backend. Stick with bootstrapping rather than asking money. 

If you can produce good code with half of the time of his and capable of all the task he does; fire him, do the job by yourself. Earn more money and get a better one.

If not and you have money; get a better one. As you know, good ones cost a lot. Cheap ones produce crap. Life is not fair for a startup.

And excuse my quick brain fart :)


## Answer 49556

- posted by: [eddyparkinson](https://stackexchange.com/users/-1/26527-eddyparkinson) on 2013-06-18
- score: 0

Improve QA process:

1) Work through the excesses at the back of "A discipline for software engineers". 
  i.e. do this yourself. I have been there and done that, I highly recommend it. Will save a lot of time, money and improve the quality of the product.  I.e. Learn to follow the numbers, let the numbers guide your QA decision making. (course on QA software reviews/inspection is another effective option)  
 
2) Insist on a group requirements review and design review, before he writes any code. These should be minimal and quick. Collect the numbers to ensure they are time well spent.


## Answer 49561

- posted by: [Itai Sagi](https://stackexchange.com/users/-1/12742-itai-sagi) on 2013-06-18
- score: 0

It sounds like you're wrecking up on technical debt, always make sure that your technical debt is something that is manageable.

Saying you'll replace the code later is fine and dandy, but in the reality of it, it usually doesn't happen and small non-business critical systems, especially when created early on, might become a pillar of your startup, making them extremely hard / expensive to replace.

My only suggestion to you: tread carefully, think about replacing him in the following features and create a culture of least-debt possible by hiring proffessional people, skimping on that now, will cost alot more when the systems are operational!


## Answer 49562

- posted by: [andy](https://stackexchange.com/users/-1/21737-andy) on 2013-06-18
- score: 0

`He's been with us for about 6 months and we've spoken and tried to teach him good practices but he doesn't seem to care or want to learn.` That's a major red flag there. Of course, there may be reason for this so ask why. For instance, I've had people that use different styles of code and actually have valid reasons behind why it looks messy.

You should make sure he does care and put in practice code reviews. For instance, here we have a git repo and anybody that works on that project can clone the repo and begin work. However in order to get their code merged into the repo, the code must be of good quality and not full of commented 'die("test")'s. They can submit a pull request and then we can look over the code and merge it if it meets criteria.  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
