## Billing for addons - how?

- posted by: [F21](https://stackexchange.com/users/-1/13598-f21) on 2012-12-05
- tagged: `subscriptions`, `billing`
- score: 1

We are building an SaaS service that will be billed on a monthly basis. For example, if the user's service starts on 4th December 2012, then we bill them on 4th December 2012 for the month's fees. We then bill them again on 4th January 2013 for the next month and so on.

If the user wishes to change his plan, we either give them prorated credit (if switching to a cheaper plan) or charge their credit card a prorated amount until the next billing date immediately. In other words, based on the above example, if the user changes their plan on the 20th of December 2012 to a more expensive one, we calculate the prorated charge from 20th December 2012 to 3rd January 2013 minus their current paid amount from 20th December 2012 and 3rd January 2013 and charge that immediately to their card. The benefit of this is that it prevents the billing day from shifting when plan changes occur. Is this a good idea?

The application also has add-ons that can be subscribed to. The add-ons are also billed on a monthly basis. Add-ons can be subscribed and unsubscribed to at any time. Should add-ons be billed immediately with the billing period calculated so at it matches the plan's billing day? Based on the previous example, if a user adds add-on Y to his plan on the 20th December 2012, we only immediately charge him for the 20th December 2012 to 3rd January 2013. Is this a good idea? Or should we have the system add up all of those addons that are subscribed to between billing dates and just charge them that whole amount at the next billing date?

Our goal is to have a system in place that is the fairest, least confusing and easiest to understand for customers. This prevents customers getting confused, which results in lots of customer support queries, and worst, disputes and chargebacks (think chargeback fees in addition to the refunded amount!) which can be expensive and unproductive for us.


## Answer 44875

- posted by: [Rajaraman](https://stackexchange.com/users/-1/21983-rajaraman) on 2012-12-08
- score: 1

The way you handle the proration is the most logical approach. Also as mentioned, its preferable to keep the user's billing dates intact. So based on your example, on 20th December the customer should be charged for the balance period in her current term. However, if she is moving to a plan with different term say quarterly, the billing date can be changed. 

Watch-out: If you have discounts in the current subscriptions, ensure those rates are considered while calculating the proration.

Generally add-ons align with the billing interval of plans. Going with your example, when the customer adds a new add-on, she should be charged only for the period 20th December 2012 to 3rd January 2013(remaining period in the billing term). And its not a common practice to accumulate all the charges till the end of billing term. Completing transaction immediately removes chances of ambiguity in the subsequent billing cycle.

Also, customer should be notified as and when she makes changes in her subscription and sent an invoice immediately if there are charges to be collected. 


Disclosure: I am a co-founder of subscription billing solution.



## Answer 44845

- posted by: [Kosta Kontos](https://stackexchange.com/users/-1/16592-kosta-kontos) on 2012-12-07
- score: 0

I'd revise your billing model so that, instead of your users paying directly for access (and additional add-ons), they instead purchase credits from you. This pool of credits, in turn, allows your users pre-determined periods of basic / standard access to the system.

So for example, purchasing 300 credits would be enough for 30 days of basic access (at roughly 10 credits per day), and then your users can purchase add-ons whenever they want, which cost additional credits per day (ie: add-on ABC costs 1 credit per day).

That way your users can sign up for add-ons at any time, and when their credits run low, they top up.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
