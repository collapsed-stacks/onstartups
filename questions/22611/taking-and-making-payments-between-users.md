## Taking and making payments between users

- posted by: [joshucar](https://stackexchange.com/users/-1/9063-joshucar) on 2011-03-30
- tagged: `payments`, `saas`, `micro-payment`
- score: 0

I am in the nascent stages of developing a service that will allows some users to request a certain task and others to perform those tasks.  Money in from the user requesting, company takes a small profit, money out to the user to perform the task.

Think Amazon's Mechanical Turk.

What systems can be used to support this sort of transaction.  I want everything to be automated so I certainly don't want to be cutting checks!

Thanks in advance!

**Edit**: To further clarify, I think of the service as more than just a middle-man.  I guess it's more akin to Crowdflower/99designs/etc. where the company is providing the service and will guarantee the results.  It just also happens to use its user base to accomplish some of the tasks.


## Answer 22614

- posted by: [Mircea Grelus](https://stackexchange.com/users/-1/1822-mircea-grelus) on 2011-03-30
- score: 1

<p>It won't be easy to set up the merchant account for this type of businesses. They're called Third Party Payments Aggregation accounts. They're high risk accounts, because you're basically facilitating the exchange of money between two parties.</p>

<p>You're charging money for services/products you do not own. There's a lot of risk involved with this. How are you going to handle charge backs, who guarantees you're not going to take the money and vanish, or how do you guarantee the delivery of service.</p>

<p>Braintree has a <a href="http://www.braintreepaymentsolutions.com/blog/high-risk-mechant-account-third-party-payments-aggregation" rel="nofollow">blog entry</a> with more details. You can find out more if you google for "high risk merchant account" or "third party payments aggregation".</p>

<p>They're not easy to set up.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
