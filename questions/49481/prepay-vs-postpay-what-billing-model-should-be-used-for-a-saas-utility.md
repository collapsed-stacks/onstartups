## Prepay vs Postpay, what billing model should be used for a SaaS utility?

- posted by: [Rook](https://stackexchange.com/users/-1/9035-rook) on 2013-06-10
- tagged: `saas`, `billing`
- score: 3

We provide a utility-like service and have to charge a variable rate per API call. Most of our customers are businesses (B2B).  Just like an electric bill,  at the end of the month we can total the customers usage and then bill the customer.  We are using [briantree's vault to create new payment transactions][1],  so after we have the payment information we can charge what we like,  whenever we would like.

A similar utility is Google Adwords.  [Adwords allows customers to prepay or postpay][2] for their service.  Ideally we would force our customers to prepay for everything, however its impossible to know what the customer will use ahead of time and this maybe confusing to the user.  Most utilities use "postpay" exclusively,  however,  we are concerned a customer would rack up a large bill and then cancel their credit card.

What is the best billing model for customers and our company?


  [1]: https://www.braintreepayments.com/docs/ruby/transactions/create_from_vault
  [2]: https://support.google.com/adwords/agency/answer/6390?hl=en


## Answer 49482

- posted by: [Randy E](https://stackexchange.com/users/-1/19553-randy-e) on 2013-06-11
- score: 3

Steve Jones really should have made his comment an answer, as it's absolutely correct. There really is no best billing model. Some things to consider:

1. Are you a Business to Customer or Business to Business operation? While answering this question may not give you a specific answer, it will help let you know how long of a billing cycle would be best, with businesses preferring (generally) to enter into year long contracts and pay everything up front, individuals sometimes prefer to only pay for what they use and prefer shorter cycles, to more easily allow them to move or cancel whenever they want.
2. What do your customers prefer? See above.
3. What is the industry trend for your niche? This will let you know what your potential customers already accept as the norm. 

There are many other things you can ask yourself. But overall we can't give a perfect answer. If you're worried about people racking up usage then leaving without you being able to collect, than pre-pay would be the best option. One good thing about pre-pay is if you bill on a certain part of the month each month no matter when the company/person signs up, you will always know how much revenue you have for that month. Another good thing is it secures you from the people using your service then leaving never to return.

Postpay is good if you don't have any of the concerns above, or if the amount you're charging is trivial enough that you can afford to write off x% of your customer a billing cycle. It's also good if it's a pay per use model. 

But, you need to find out what your customers want. This can be easy or difficult at the same time. If you have customers already, consider polling them. If you're not at that point yet, consider doing some market research in other ways. Check what your competitors are doing. If they're all doing pre-pay, you have a choice, stay with the norm or add one more thing to separate you from them (post pay). 

In the end, it's all about risk vs. benefit, what your customers want, and more importantly, what your business model shows would be the best.

Everything in business is a risk, from the very beginning to the decisions you make 10 years from now, choosing a billing model is a risk. Depending on your industry, it could be a huge one that could sink you, or it could be so minimal that it wasn't even worth the time typing out your question :)

Note: Many SaaS providers prefer to charge prepay to ensure they're not losing out on resource usage income. Electric company's know that either you are going to pay their bill, or they're going to shut off your service, which most people require to live ow they want.

As Steve suggests, you can create package deals that they prepay for X amount of calls each month, and if they go over they pay Y amount for each additional ones, you can make it so they automatically go up to the next package if they go over, or you can make it per individual call. In the end, you may discover that offering both options would be good. 

I.E. If they prepay they get a bundled amount, if they post pay they are charged a little more (to offset your risk) and may pay per call.


## Answer 49533

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2013-06-16
- score: 1

The difference between prepay and postpay is (and excuse me for stating the obvious!) just a matter of whether customers give you money and you draw that down as they use your service, or whether they use your service, and periodically you ask them to settle up.

**Almost every *pricing* technique, and almost every *customer management* technique, can be implemented in prepay, postpay or hybrid billing styles.**

So, for instance, *credit limits* are as old as credit itself - a tool to limit customer surprises and manage non-payment risk. 

Given that you're B2B, it sounds as though you feel your customers would prefer postpay (which is why you talk about a possible need to *"force"* them to prepay - i.e. you think that's what they'd like less). If that's the case, you should probably run with it as your primary model. And if you're not sure, you should *definitely* test that hypothesis.

If the variability is high - one customer will get value from a few API calls a month, while another will get value from a few million - then you'll probably want to put that into your pricing structures. Thinking of your example of the utility case, it's very common for customers to be offered pricing that looks like a number of fixed fees, each with its associated usage allowance or/and unit price. That's a familiar, simple and effective way of working with customers, as it helps put the question "how much of this stuff will we be using?" on the table in a positive way.

There are two cases where I'd generally advise prepay as the primary model (remember, I'm assuming that you *know* that your customers would prefer postpay).

First, **if each API call creates a significant external cost for you,** then postpay may be too high risk unless you can back this off to your supplier or insure it. That's partly just the math, but even more importantly it's a by-product of longer supply chains, where you're less able to keep the interests of every party aligned. In this case, your challenge is to find ways to make prepay into a benefit to your customer, that will sugar the pill that they'd prefer postpay.

Second, **if the person you're selling to is also going to be the primary user, and relatively junior within the organization,** then you may be in a situation where people changes and organizational changes outside your view may result in "aggravated churn" - i.e. situations where some other party in the company will terminate the arrangement and want to dispute charges (perhaps going back some months). Prepay may in such cases be preferable to what may be a high friction and delay-ridden process of engaging with the purchasing process sufficiently to mitigate this risk (e.g. by ensuring the cost is explicitly and reasonably captured in a formal budget).



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
