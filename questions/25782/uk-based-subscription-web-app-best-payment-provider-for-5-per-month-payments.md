## UK based subscription web app - best payment provider for $5 per month payments

- posted by: [Sam Delaney](https://stackexchange.com/users/-1/10978-sam-delaney) on 2011-06-02
- tagged: `saas`, `uk`, `subscriptions`, `billing`
- score: 5

I am currently developing a SaaS product and am at an impasse in terms of how to charge.

The subscription is only going to be $5 per month. Although I'm in the UK, my main market is going to be the US, so it's easier to just charge in dollars.  

I have looked at Google Checkout and Paypal, but their charges for small amounts are huge, and would be a massive percentage of my revenue.  I know there are companies like chargify and recurly, but they work on top of merchant accounts, so there'd be even less money at the end.

I also need to ensure that the monthly billing is simple, and can be prorated to simplify the billing cycle.

Offering staggered payment options could alleviate this, but this would mean I'd have to alter the monthly payment to ensure I'm bringing in the same money as forecasted.

Has anyone else come across the same problem, and is so, how did you solve it?

Is it really this difficult to create profitable web app subscription services?


## Answer 25904

- posted by: [Rafferty Pendery](https://stackexchange.com/users/-1/11003-rafferty-pendery) on 2011-06-04
- score: 1

We have gone through a similar process in the past. I suggest you consider charging $60 annually and then charge more for monthly, giving them the incentive to pay by year. Maybe charge $8/month instead (just throwing out a random number). 

When you are talking about such small amounts per subscription, charging monthly or yearly seem to be the only two options you need (wouldn't see quarterly or every 6 months as necessary options)

Recurly makes the billing and pro rating VERY simple and is really easy to integrate to. We hook that up with Quickbooks Online as the payment gateway and merchant and have been very happy with the integration. 

Good luck!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
