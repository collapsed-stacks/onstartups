## Dilemma: to outsource the coding or do it yourself

- posted by: [BlackRider](https://stackexchange.com/users/-1/13723-blackrider) on 2012-08-05
- tagged: `outsourcing`, `bootstrapped`
- score: 34

I develop and sell iPhone apps. I've released one app, and decided to build a few more, in parallel. I thought about outsourcing some of the coding, so I went on Elance and posted some jobs there. The estimates I've got from the contractors there turned out to be a bit higher than I had expected, and were generally comparable with the software engineer salaries in the US (e.g. they ask for $1000 for what would be maybe 4 days worth of work for me). I wonder if the lower rates of the oversees contractors often get offset by their lower productivity? 

So I started doubting if the outsourcing approach is worth it. My company is new and is not making money right now. I'm bootstrapping it with my savings. I could invest some money to get things done by other people, or I could invest some of my time and save the money. What should I do?

I'd appreciate any insights and advice about my situation :) 


----------


**[UPDATE]** Thanks so much everybody for such thoughtful and helpful responses! If I could accept all of your answers, I would. I'll briefly summarize my own experiences so far. It is true that writing a very detailed requirements document is both essential and time-consuming. I've discovered that as I work on that document, and think about the potential ways a feature might be implemented, I'm really doing the hardest part of the job, and leaving just some fairly straightforward coding to the contractor. As a developer, it's pretty easy for me at this point just go off and write the code myself. 

So out of the 2 jobs that I wanted to outsource, I decided to do one myself (a foundation for a new app), and outsource the smaller one (a well-defined feature for an existing app, implemented as a standalone app so I don't have to share my code with the contractor). The developer (based in Russia) has already sent me the code, and I'm happy with how is it going so far. To be fair, when I talked to him on Skype, we spoke in Russian since that's my first language too. I think it'd be more difficult to communicate with him in English.

I've read some stories of people successfully outsourcing entire apps, with the UI design and all, but I'm not sure how common that is. I.e. I really suspect that for one person who got lucky with that there may be many who have just wasted their money.





## Answer 41084

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-08-05
- score: 30

I am from Germany and have worked with several companies from India. In addition, I have some friends who outsourced to Russia. Our experience is all the same: The biggest problem remains the communication. If you want something easy, like a Wordpress template, it might work fine. But if your app is a little complex, you need to write down every little detail. You are human yourself, so you'll find out that you have forgotten something. 

My experience is that they take your spec and do it exactly as you wrote it there and don't mind the things which you have forgotten. So please be prepared to use a good amount of time to do a great specification which is error free. In some cases, I have seen that spec + implementation time exceeds the "do it in your own office" by a factor of 4. You need to speak simple English or have clear phrasing. 

Another pitfall is that you mostly are not able to get somebody on the phone (own experience) on your working time. If you get somebody on the phone, please be prepared for hard to understand English. In my case, I am not a native speaker myself, so it was pretty tough to explain it in such good English that they could understand. If you are from the US states which have a strong accent, be prepared!

One day, I calculated how much we saved from the cooperation with India. They have had a lower hourly rate, but all the spec time, communication time, re-doing work because of misunderstandings and so on summed up so much that it would have been cheaper to develop it all in house.

Another thing might be that you outsource to a company which promise you heaven but give you hell. We had to fire one company because they told us they were some kind of SAP gurus with good Java knowledge. After a while, we figured out that they have just a basic understanding of SAP and worked in a lot of performance problems. With Java, they just knew the syntax, which really does not help in a JEE environment. We have lost a good amount of bucks and time there.

My suggestion: If you know the company and have seen some references, call them. If you can understand each other very well, make sure you have called to the actual developers. If they are replying promptly, and if it seems that they use their for more than just API digging, then you might give them a try. And if you find such a company, please write me an e-mail. I am still looking for it.


## Answer 41087

- posted by: [frenchie](https://stackexchange.com/users/-1/15155-frenchie) on 2012-08-05
- score: 25

**Outsourcing software development can be a positive option but has major downsides. I've been badly burned with outsourced developers so here are 3 lessons that might help you.**

First of all, realize that the more valuable the software you want to create, the less likely you are to successfully outsource its development. In other words, if your software might generate a gazillion dollars of revenue and you're outsourcing its development for a few thousand dollars, then the developer will have very little incentive to perform miracles for you. How would you feel coding for dollars a software that might make someone else a few million dollars? This is especially true if you're outsourcing the first version of a software: **specs kill creativity** because it's only AFTER seeing the coded result of a spec that you realize that such and such functionality should actually be done differently. If you're creating something new, the spec should be a roadmap to the discovery of the final product, as it's being built. I don't think you can outsource the creative process that goes into the first build of a new software. On the other hand, if you're porting an existing product to another platform and everything is already figured out, then outsourcing might work. So in my opinion, **don't outsource software development that requires lots of creativity or that's critical to your business. That's why for startups, outsourcing is usually a terrible idea.**

Second, in terms of payment, here's the biggest lesson I've learned. **At delivery, the contractor should NEVER EVER be paid up more than 50% of the amount due.** That way, if at delivery the outcome is in any way botched, the contractor is still holding 50% of the bag and has some incentive to fix it. If instead the contractor is nearly paid in full at delivery, then he has little to no incentive to fix any bugs that the software may contain; he might then in fact ask you for more money! So heed this lesson: at delivery, never more than 50% paid up. And if the contractor doesn't have the resources to float his operation, then he might be facing some financial troubles which may or may not influence the outcome of your project...

Third, if you outsource development, **you MUST remain in control of the Q&A**. As you know, there are many ways of writing code and some ways might be undesirable shortcuts that may come back and haunt you later. **Be involved in the major architectural decisions and make sure that the code is at all times testable.** If you hear *"waterfall methodology"*, run for cover; if you hear *"agile test-driven development"* or *"source control access"*, stick around. In other words, only outsource what you could yourself do so that you can supervise and understand what's happening, in a clear and transparent process.

Hope these help you with your dilemma and good luck with your business.


## Answer 41094

- posted by: [Drover](https://stackexchange.com/users/-1/19092-drover) on 2012-08-06
- score: 7

Since your business plan is to build multiple applications I have a suspicion there is some common aspect between the applications. i.e. each application is not unrelated bespoke development. If so, employ the rule of threes and use the first two or three apps to build your "formula" that defines the core of your business. This means key architecture patterns, key code that is automatically re-used between projects, test rigs etc.

It is possible to outsource well-defined problems. This can be a cookie-cutter implementation of a well-known technology, or it can be a variation on your formula. The previous comments are correct. Communication is critical. In my experience, existing examples is one of the best ways to communicate. Examples provide expectations and boundaries.

Until then, you need to be in control of your intellectual property (formula). No out-sourcer will build that for you (unless they have serious experience and are paid accordingly).

If time is problem then outsource something else (cleaning, mowing the lawns, cooking dinner...) and take ownership of the core of your business.




## Answer 41085

- posted by: [Alex](https://stackexchange.com/users/-1/19052-alex) on 2012-08-05
- score: 5

If you have the time and the expertise to do it yourself I would say go for it, there are numerous benefits:

- Saves money
- You know it'll be done right
- Easily manageable should any errors occur
- Easier for you to upgrade should it be required

Once you start making money is when you might look to outsource as it won't affect you as much financially.

It might slow your progress slightly, but for the assurance and cost savings it's definitely worth it.


## Answer 41095

- posted by: [Mike Kelland](https://stackexchange.com/users/-1/19100-mike-kelland) on 2012-08-06
- score: 5

I would not write off outsourcing completely based on the price of offshore development.  The other option is to look to a North American firm - I think you'll find that you get a better result, faster and for cheaper that way. 

I've seen this from two sides.  First, when I was running my own startup, we attempted to outsource development both in North America and overseas.  In order to level the playing field, we insisted on a fixed price per phase approach.  What was surprising was that, as you say, the total price overseas, even when using a firm with a North American presence for project management, was significantly higher than using a North American firm.  The rates were way lower, but the number of hours were significantly higher.  

From the other side, we've found that by exercising Canadian tax incentives and keeping only top development talent on the bench, we can produce an extremely high quality result for a lower total cost by running fixed price contracts out of Canada rather than going overseas.   

**The most important thing when outsourcing - whether its to a North American firm or an overseas one is that they align with your motivations and methodologies.**  If you are running against the Lean Startup methodology for instance - make absolutely sure that they understand that and are working and billing in line with that go to market approach.  They need to get what an MVP looks like for you, understand your business approach and be constantly augmenting your code with the right hooks so that you can get relevant metrics and data out of it every step of the way.  They need to be flexible enough to scale up and down with you as you need them.  They also need to be partnered up with you to the point where their success is at least partially dependent on yours. 

We've worked with a fair number of startups to build out product for them and have been consistently successful based on this one principle.  


## Answer 41090

- posted by: [MrTelly](https://stackexchange.com/users/-1/9073-mrtelly) on 2012-08-06
- score: 4

Not a direct answer but an observation from the trenches, outsourcing especially of an Android/iOS app development is great when you have a running example and need it ported to multiple target devices. In that instance the spec problem is much less and the economies of many cheap hands writing the code is a huge time and money saver.

In this instance as it's a core part of your business I'd develop in house, and build relationships when you want an Android port done.


## Answer 41098

- posted by: [OpCoder](https://stackexchange.com/users/-1/19097-opcoder) on 2012-08-06
- score: 3

I do think outsourcing really works(even when using those websites).
But you need to try to have a strategy in order to make sure you choose the right people.

I read what others wrote here about their experiences and it made me smile.

@Christian:
**How could you even hire and start working with someone who doesn't know English fluently?
How can you hire someone who knows only Java syntax when you need him to work on SAP?**

If you talk with manager/team lead X, you will have to ask them who exactly are the developers which will be working on your project. You need to know what apps they worked on, and what were their roles in the dev of those apps.
You should know exactly who are the people which will be working on your project.

Don't be surprised you get high quotes when you didn't describe what you expect from your app. 

Selecting someone only based on the bids\quotes is a big mistake.
I would suggest the following recruiting process:

#1. Ask for a portfolio with project description(in your case it should include links to the actual apps in the store).
But it's not sufficient to mention it, they need to say what was their role in the development(did they do it from scratch? if not, what was their actual role? Did they do the backend, the UI or what was it). Also, they should mention the frameworks they used, etc. It's important I think sometimes to see if they know about the right tools.
   
  
#2. Select those which send a portfolio according to #1.
You will be surprised to see how few are which did that!. 
If they can't follow a basic request to send their portfolio, they will surely not be right to hire to code your app.
If you think you will need to have meetings on Skype, schedule a Skype few mins interview with them, and ask questions about their apps they did.
If you are talking with manager/team lead X, you tell him you want to meet the people which actually will work on your project. 

At this point you will have a pretty good idea if you really found some people good candidates, with a good experience to code your app.

#3. You should have a simple specification, about what you want to do in your app.
Send them the specification and ask them to make milestones on the features, and ask them to estimate them.
If the project is big and you cannot make a complete specification, then split the project by features, and at least do a specification for first features.
It's far better than posting the project without any specification at all or spend a lot of time creating specification for something which might change along the way.


I am a coder myself. I saw a lot of stupid people and projects.
I saw employers posting project and expect quotes for something they didn't even bother to describe the features.
How could someone realistically estimate something if there's no description on the feature which need to be implemented?
I never bid on projects which is not clearly defined. I sometimes try to ask employer for clarification/specs.

Isn't it stupid to ask for quotes on something which was not even defined?
Isn't a quote supposed to be in correlation to an estimated effort in hours multiplied by an hourly rate?

I have good knowledge in recruiting and working by outsourcing.
Some employers are asking for trouble, when they get burned, it's sometimes because of their own fault.




## Answer 41093

- posted by: [Mugunth](https://stackexchange.com/users/-1/19087-mugunth) on 2012-08-06
- score: 2

Making a simple iOS app takes 50-100 hrs.
Making an fairly complex iOS app takes 300 hrs.

At $20 an hour, the complex app costs $6k

At $100 an hour, it would cost $30k. For most businesses, the additional $25k (which is far less if you include communication overhead with an outsourced team) is a no-brainer.

Unlike enterprise application software, iOS apps are less complex and you won't save a huge chunk by outsourcing it.


## Answer 41099

- posted by: [Faster Solutions](https://stackexchange.com/users/-1/19103-faster-solutions) on 2012-08-06
- score: 2

I'm sure there are outsourcing companies and developers who are very good, but that's not really the issue.

As a new company you're building a reputation and a brand.  These will primarily come from:

 1. User feedback on your apps.  Clients will want to see consistently
    good feedback on your app portfolio. 
 2. Client feedback on their
    "experience" with working with you.  Clients want "on-time and
    on-budget" while providing changeable requirements, often because
    they don't really know what they want.

What you're currently selling is you.  Your ability to work with clients and your technical and design ability.  I also assume that you like what you do and take pride in what you create.  It sounds like you've got a couple of people interested and that's great, but now comes the hard part.

You've gone out and sold yourself to your clients; will thy be happy finding out that they've got someone else writing their application?  They have hired you to do the work.  If the projects are delivered late and/or not developed/designed particularly well it'll be your reputation that is being damaged.

One of the hardest things to do as a developer or a businessman is say no.  If you're orderbook is full then you need to let clients know when you can schedule them in.  If you find you're turning away more business than you're comfortable with, perhaps you should hire someone part-time (know any colleagues who are any good?).  Whatever you do, don't over-extend.  This will damage your reputation and your ability to make a success of your business.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
