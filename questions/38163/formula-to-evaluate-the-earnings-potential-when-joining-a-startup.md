## Formula to evaluate the earnings potential when joining a startup

- posted by: [Nick P.](https://stackexchange.com/users/-1/16997-nick-p) on 2012-04-13
- tagged: `software`, `equity`, `tax`, `job-offer`
- score: 1

I'm trying to come up with a rough formula to help decide if I should join a startup.  I'd like to weigh my current pay vs joining a startup, taking into account opportunity costs and possible final payout, all weighed against the inherent risk of joining a startup.  Here's what I'm thinking ATM:

    curr(time) = time * CurrentPay

    Startup(time) = time * (BaseSalary - OpportunityCost)
    Investment(time) = curr(time) - startup(time)     (e.g. the amount of pay cut you took)

    Payout = (net?)SellPrice * EquityShare

    TimeToSell := how long you were at the startup before it sold <= BreakEvenTime = curr - (startup + Payout)

    SuccessProbability := odds that a company will be sold for the assumed price
    Roi(time) = Equity - investment(time) / investment(time)

    MakeMeMove(Investment, Payout, TimeToSell, SuccessProbability) = ???? = do it!/don't do it!

That last part is where I'm stuck... How do I turn Roi/risk into a "make me move" number? Given a statement such as "If the payout is a cool million then I'm willing to take a chance on a company that has a one in ten chance of succeeding.", what formula could I use to evaluate an offer?

> ###Completely arbitrary Example:###
> Person joins company with 50% chance of selling for $10M in the next two years.  Person gives up a job making $100k to make a base salary of $80K plus 1% equity.  Given an equivalent amount of work, this person could make an additional $10K/yr  in side work had they stayed at their old job. Company beats the odds and successfully sells for $10M after two years...  

> Curr = $200k<br/>
> Startup = $140k (salary - opportunity cost)<br/>
> Investment = $60k (curr - startup<br/>
> Equity = $100k<br/>
> Roi = 67% on an investment that had a 50% of returning nothing



Other Questions

 - How much equity share is typical for a: founding engineer (at a software company)? A non founding engineer(e.g. Brought in, say 2 years later). Vague question I know, just looking for some general guidelines...
 - What is the avg time taken to sell a startup? (again, looking for hard and fast guidelines)
 - If the company does sell, is your equity payout based on the sale amount or net profit? Other mitigating factors?
 - How is the payout taxed? Cap gains? Income tax?
 - Are there any tax benefits/liabilities to being an equity holder?


Any advice would be greatly appreciated!


-----------------
Edited title to highlight the financial focus of the question.


## Answer 38184

- posted by: [adib](https://stackexchange.com/users/-1/8883-adib) on 2012-04-14
- score: 1

There are at least four dimensions that you need to consider whether to join a startup as an employee (or from the flipside, getting other people to join your startup) - those are:

 - Paycut (or opportunity cost) – as opposed to what you can earn if you take a job with a large corporation (like those in the Fortune 1000 list)
 - The company's _unfair advantage_ – as in what interesting factors in the job that the startup offers and more established companies cannot possibly provide.
 - Work/Life balance – often startups are terribly resource-constrained, and you may have to work significantly longer hours due to this.
 - Boss' (or founders') working attitude – It's pretty common for startup founders to be a bit arrogant and you might want to gauge this for the particular startup that you're interviewing with before signing the deal.

If you look closer at the four factors above, only two can be valued with money. Those are _paycut_ and _work/life balance_ (because working hours can easily be translated to dollars). Since the other two can't be easily (and objectively) mapped into dollar values, I suggest you seriously **reconsider your approach of making this decision based on financial factors alone**.

Note that these factors are only applicable when you join as an employee and **not when you also given a large portion of equity** that allows you to join as a member of the board.

I've written an article on how to [entice experienced employees for your startup](http://cutecoder.org/business/employees-startup-compete-megacorp/), and the materials are also applicable to see whether you want to work for a (particular) startup.



## Answer 38173

- posted by: [dolan](https://stackexchange.com/users/-1/17493-dolan) on 2012-04-13
- score: 0

Regarding your equation, it seems you are going in a decent direction.  I mentioned in my comment above that you could personalize this equation based on your preferences on things like risk-adversity, amount of savings in bank, etc.

    riskAdverse = 0.9
    daysSurvivalOffSavings = 90
    estimatedDaysToFindNewJob = 30
    curEligiblityUnemploymentMonths = 6
    etc.

    (daysSurvivalOffSavings - daysSurvivalOffSavings)*riskAdverse + ....

Getting lazy on calculations, but hopefully my point of personalizing gets across.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
