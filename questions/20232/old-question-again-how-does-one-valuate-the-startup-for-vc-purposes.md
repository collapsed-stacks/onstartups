## Old question again: how does one valuate the startup for VC purposes?

- posted by: [Igorek](https://stackexchange.com/users/-1/4395-igorek) on 2011-02-14
- tagged: `funding`, `venture-capital`, `valuation`
- score: 5

I've been running a bootstrapped startup since last year and am running into definite limitations as to what I can do without further funding.

Startup enables elasticity for Microsoft's cloud platform: Windows Azure.  We are B2B.  First iteration of the software is complete and has been released. There are a number of paying customers who are very happy with the product.

Potential of the product is as good as Microsoft can make with Azure (assuming that MS does not move in with a similar product).

Any Azure customer is my potential customer.  I know total number of Azure customers today and can make estimates on how many Azure customers there would be going forward.
I know how much each customer of my product can bring in a year on the average.
I know how much it costs in OpEx to support each customer
I think I know how much money I'd like to raise at a minimum to continue new development and marketing efforts

What I dont know is how to value my company today. I realize that alot of VC pitches are all about gut-feel and how hot the market is, etc.  Suggestions as to how to value my company, given the number of variables mentioned would be appreciated.



## Answer 20309

- posted by: [Philippe](https://stackexchange.com/users/-1/6113-philippe) on 2011-02-16
- score: 2

There is no answer to this question. Pre-money valuation is a negotiation, not a calculation. As an illustration, the rule of thumb that Guy Kawasaki cites is: "add 500.000 for every full-time engineer in your company, subtract 250.000 for every MBA."


## Answer 20303

- posted by: [broiyan](https://stackexchange.com/users/-1/7780-broiyan) on 2011-02-16
- score: 0

You should use your intuition and your own estimates.  Investment bankers will be able to do no better than you can.  Presumably you trust yourself more than bankers.  The answer is both trivial and impossible to get precisely.  Sum the present value of estimated cash flows, discounting each cash flow for time and uncertainty before summing.  These cash flows are after costs have been taken out, and costs include any interest paid.  Since you don't know how competition and adoption (customer response) and many other variables will affect your profits, the discount will be significant but the fact that you already have paying customers mitigates the discount.  If you need more details on how to estimate the value of your business, just pick up a finance textbook like Brealey Myers.  It's interesting and easy to do.  

I must emphasize your expertise.  As a founder you will have a good sense of what the risks are and how attractive the benefits are to customers.  You will understand the effort necessary and challenges faced by your competitors.  This is why your estimates and expertise are important (regardless of the fact that self-interest makes your opinions important to your biased self.  May be some people are not self-interested and they just want an unbiased estimate, but such people are rare).  Some people care only about money but some other people care about both money and control.  Controlling your business may be very important to you.  May be you think control is rewarding or fun.  May be you think your expert control will lead to more money for yourself.  In that case, consider accepting a debt investment instead of equity.  Debt provides the investor with some sort of promise and helps you to maximize control.  This could be a win-win (if both sides think it is a win-win).  Consider that perhaps a certain VC has information and skills that will help your business.  The business is likely to be rapidly evolving so perhaps it is better to just accept a smaller investment until the time comes that both founder and investor have an easier time estimating value.

You should try to find comparables.  Find startups in a similar industry or specialization and see how much they were valued at.  See what metrics you can compare between yourself and the comparables.  Do you have 1.5x the customers as competitor X.  Do you have 2.0x the revenue as competitor X.  Are you increasing customers at 100% per year but competitor X is increasing it at 50% per year.  Is Azure growing at 0.5x the speed of Amazon EC2.  These comparisons will help you estimate the value of your business.  Value is relative in the real world.


## Answer 20433

- posted by: [burritoboy](https://stackexchange.com/users/-1/7868-burritoboy) on 2011-02-18
- score: 0

In addition to the bottoms up approaches (comparable companies and discounted cash flow) consider a top down approach, which investors will use to smell test your valuation expectations.

Identify how much an investor is looking to invest and his/her expected return (i.e. $5M investment for a 5-10x return, i.e. a $25-$50M return).

Identify what you think are reasonable ranges for exit scenarios: A) $50M-100M, b) $100-200M, c) $500M - $1B.

If you believe bucket A is the appropriate range of exit scenarios, the $5M investment will require the investor to hold 50% of your company, i.e. your company would have a $5M premoney, and $10M postmoney today assuming the investment goes towards working capital. 

If you believe bucket B is the appropriate range, the $5M investment will require you sell 25% of your company. Bucket C will require you to sell 10% of your company.

Note, this is rough math and would have to be adjusted for different features of securities (dividends, liquidation preferences, etc), any assumption around future financing events, and any accrued cash.


## Answer 30935

- posted by: [Reed](https://stackexchange.com/users/-1/11349-reed) on 2011-10-03
- score: 0

There are a few approaches to valuate a start-up company.  But I must first clarify how VCs look at investing a company.

Generally, VCs look at 40%~100% annual growth over 3~5 years.

Suppose your pre-money valuation today is $1,000,000, VC require 40% growth.

Your future valuation 5 years down the road at $1,000,000 x (1.4)^5
= $1,000,000 x 5.38 = $53,800,000

~~~~~~~~The above is a simple view.  Here is a more realistic view:

You claim your company will worth $70,000,000 5 years from now. (assume you can back it up)

You need to raise $1,500,000 today to achieve the growth.

VCs look at your presentation and agree with your valuation, then say: we need 70% annual return. And they give you $2,000,000 (more than you have asked)

The calculation:
Discount $70,000,000 by 70% for 5 years = your Present Value
PV = $70,000,000 /1.7^5 = 4,930,073

The VC require this percentage of your company: (2,000,000/4,930,073)% = 40.6%

~~~~~~~~ Here is what happens in real life

VCs think you need another round of financing of $5,000,000 at the end of 2nd year to achieve the growth.  And they still want 70% annual return.

the 1st round investor require 70% annual return over 5 years

the 2nd round investor require 40% annual return over 3 years.

you need to raise:

$2,000,000 @ 1st round end of year 0 (future value @ y5 = $28,397,140)

$5,000,000 @ 2nd round end of year 2 (future value @ y5 = $13,720,000)

$70,000,000 valuation at the end of year 5.

In the end of y2, this is your stock structure:(after money)
You : 39.8%, 
VC1 : 40.6%, 
VC2 : 19.6%,  

Pre-money:
You :49.51%, 
VC1 :50.49%, 

Since VC1 don't want to control the company, they will take 49.9% for a $2,000,000 deal.

~~~~~~~~~~
Okay, now you need to know how to come up with a valuation @ the end of year 5.

That's quite simple, just add up your projected net earning in year 5,6,7,8,9, each adjacent year discounted by a % rate(purely hypothetical number)

Discount rate: 30% (we just assume, but don't go lower)

Your net earning:(before tax)

Year 5 : $16,400,000

Year 6 : $21,000,000  discount by 1.4   = $15,000,000

Year 7 : $27,000,000  discount by 1.4^2 = $13,775,510

Year 8 : $36,000,000  discount by 1.4^3 = $13,119,533

Year 9 : $45,000,000  discount by 1.4^4 = $11,713,869

Add it up : = $70,008,912  

Yes! here is your Future Value. However, you must be able to explain, how did you come up with the net earning.

----------------

A final note: 

There are more than one way to calculate the above numbers. I just showed what is the easiest to illustrate in a post like this.  For full details, go to amazon.com and buy a book on business valuation.

Reed




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
