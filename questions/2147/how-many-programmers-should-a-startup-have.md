## How many programmers should a startup have?

- posted by: [user1056](https://stackexchange.com/users/-1/1056-user1056) on 2009-10-22
- tagged: `hiring`
- score: 7

You've got an early software project, it's reasonably popular. There's no known limit to the product's potential size or usefulness. You've just gotten funding.
How many programmers do you hire?


## Answer 2165

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-22
- score: 7

Even though I agree with the former answers on not having enough information, I would recommend to keep the team small.

Most products can be done in small teams. Larger teams often produce much more overhead and therefore are slower to market. So if the size of the product does not demand for a large team, don't go there.

If your product is customized for different clients, the team size will be bigger too. Here it is like in marketing: target similar clients with a similar feature set to keep the versions and custom code small, or - whenever possible - decide on a product where all get the same. This again will help you start or even keep going with a small team.

Two programmers are better than one, as there is a fall back if something happens. Ideal teams are 3-6 people, as they usually self organize with little to no overhead.


## Answer 2202

- posted by: [Mike](https://stackexchange.com/users/-1/853-mike) on 2009-10-22
- score: 4

As few as possible. Only hire when you're hurting.


## Answer 2148

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2009-10-22
- score: 3

There's not enough information to answer your question, but I'll provide some parameters.

1. It really depends on how much funding you got. It's a really different approach when you get the proverbial $5M VC from an early stage $100K friends and family.

2. If you got plenty of money, you don't need to figure this out, hire a CTO and he'll know the right answer :-).

3. OK, so let's say you hired me as the CTO :-). I'd probably hire no more than 5 developers initially. Better, I'd try to bring in people/a team that I've worked with before.

I think that's really the answer you're looking for. Like everything else in life, you can't build things too fast, even if you have tons of resources, or they'll fall apart. Hire a CTO. The CTO hires 5 senior people who get to define the next generation of the product, get familiar with it and with each other. The CTO and his people can in turn hire a 15 more people and break them into teams, and so on.

One other thing that you need to realize is that a team of 5-6 developers can a lot in a new product. At the end of the year, they'd put in 5-6 man years into the product :-).





## Answer 2152

- posted by: [Nathan Kontny](https://stackexchange.com/users/-1/973-nathan-kontny) on 2009-10-22
- score: 3

Right, too little information.  If this thing is still early and small, and your investors aren't forcing you to hire more, I feel like a great number is 3.  1 designer, 1 developer, and 1 guy who helps fall in between.  Maybe he does some design, maybe more development.  But can help both other folks.  37signals also shares this same advice and built basecamp originally with this number.


## Answer 2204

- posted by: [Miro](https://stackexchange.com/users/-1/863-miro) on 2009-10-22
- score: 1

As was mentioned previously, hire as few people as possible. The more employees you have, the more "overhead" (read hassle) you will have to go through because no matter how good the CTO is, you will still have to deal with payroll, holidays, sickness, slacking and other interesting problems that occur when people work in groups.


## Answer 2206

- posted by: [Olivier Lalonde](https://stackexchange.com/users/-1/1030-olivier-lalonde) on 2009-10-22
- score: 1

From my own experience as a software developer, one rock star programmer is worth ten. You'd better get a team of the 2 greatest programmers you can find than go and hire 10 unexperienced ones. They'll get more done in the same time and do it better.

I would add that the choice of technologies is as much important. As a startup, you probably want to go for open source and languages that offer high productivity. You shouldn't worry too much about performance or scaling issues at this point. Focus on what you're good at and let cloud providers do the heavy lifting.

Talking from my own experience though, this might not hold true in all cases.


## Answer 2253

- posted by: [Manuel M](https://stackexchange.com/users/-1/1085-manuel-m) on 2009-10-23
- score: 1

Hire one really strong, seasoned developer (or ideally have her/him on the founding team and pay less), and add 2 more. Pick a fast dev platform, and race away in an agile mode. Keep management issues to a minimum and get product built. If you can afford it at all, bring in a virtual CTO/advisor who can help set up your overall technical direction right so that you don't have to rip out *all* your code later, but can actually refactor it all :) 

Also, demand automated testing at the unit, functional, integration and UI level, and you'll get a ton done very fast.


## Answer 34629

- posted by: [Henry VIII](https://stackexchange.com/users/-1/15463-henry-viii) on 2012-01-09
- score: 1

1 but an awesome 1

_s/he'll help you to figure out if you need more_


## Answer 2200

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2009-10-22
- score: 0

Depends on the product, depends on the requirements, depends on the legacy code. 1 KLoC or 50KLoC code or not code at all?

If you are just starting feel free to go up to 5, if it's legacy code I don't see a point more than 3 since you can't let them just dive into the code. So get 3 first train them, when they are confident about the code, application and the vision then you can hire 6 more if you really really need it. But it's darn rare that you'll need 10 developers in that early, and it'll pain to manage.


## Answer 2212

- posted by: [Cary](https://stackexchange.com/users/-1/937-cary) on 2009-10-23
- score: 0

I would recommend the following strategy:

 1. Hire the best engineers you can afford, but only ones that have "been there, done that".  It is true that 3 or 4 rock stars will get you more bang for buck than a group of 10 or 20 mid level or mediocre senior level engineers.  You will want engineers that are passionate about the particular technology or space you are in.  These are the kind of engineers that will strive to deliver the best possible code/design.
 2. "Been there, Done that." - Engineers who have already solved the problems you are about to face won't waste time learning how to solve the same issue, thus your development will go much quicker and they can share experience for business decisions.
 3. Make sure the product/service is built right from the very beginning.  Short cuts taken early on always bite you in a critical moment down the road.  What will happen is that all the engineering debt piled up from taking a year of short cuts will cause you to not be able to execute what should be a simple refactoring in a crucial time for that whale of a customer.  So, while it might seem wasteful to spend a day discussing some design pattern or technology, that discussion and the implementation that stem from it will pay you big dividends in the long term.
 4. Hire a really good QA Engineer so that you have established testing procedures at all 7 levels right from the beginning.  This is also a best practice that will save you time and money in the long term.
 5. I agree that a group of 5 is a nice size group, however, this number really depends on how much work there is to do, how big the product/service is in terms of functionality, features, scope, etc. and how much specialization you need to begin with.  You may not need that many generalists, but you may need specialization in release management, scalability, database, User Interaction, etc. depending on what your product/service is.  If you can afford it, I would recommend that your rock stars each have a specific specialization.  This way if you need to expand the team further you have engineering group team leads already in place.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
