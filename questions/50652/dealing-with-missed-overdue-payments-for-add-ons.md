## Dealing with missed/overdue payments for add-ons

- posted by: [F21](https://stackexchange.com/users/-1/13598-f21) on 2013-08-28
- tagged: `payments`, `saas`, `subscriptions`
- score: 1

We are building a SaaS product where there will be some plans to subscribe to.

In addition to subscribing, the user can also buy some add-ons for more functionality. Since these add-ons do not cost so much, we do not bill them straight away. Instead, we collect the charges together and lump them into an invoice every so often and then charge the amount on the invoice to their card.

The problem is this:

John subscribes to plan A, which costs $100 a month. This is billed and charged immediately.

He then adds 2 users (each costing $10). When he adds the first one, we have not charged his card yet. When he adds the second one, the system combines the charges into an invoice and attempts to charge him.

Let's say the charge fails, and after 2 more reattempts (this is currently our threshold), the charge still fails.

What do we do at this point? We could try to disable those 2 users, but it can be confusing on John. In addition, it also increases the complexity of the application as now, we need to be able to suspend individual parts of it and reactivate them based on the payment of the invoice.

We are currently leaning towards just disabling the whole application and showing a page to update their credit card details. However, the problem with this approach is somewhat unfair as the user did pay for the subscription and is only delinquent on payments for the 2 users.

What should be done in these sort of circumstances?


## Answer 50663

- posted by: [Ross Mann](https://stackexchange.com/users/-1/27113-ross-mann) on 2013-08-28
- score: 0

I would create a grace period along with a bunch or reminder e-mails to start. Once his card can not be charged send an e-mail reminding him and provide a link to update billing info. Remember if you can't bill now you likely can't bill when the subscription is up for renewal. Lets say the grace period is 7 days, try e-mail him each day reminding him that the add-ons are still due and in 7-x days they add-ons will be removed. I would avoid (if possible) flipping off his subscription as he did pay for that at least till the end of the month. Once the grace period is over turn off the add-ons. If the person is actually using the system the frustration with now not having his two extra users will get them to jump on solving the problem right away. You can do the same with the subscription.

Also why not charge for the add-ons right away? This would protect you against abuse , the person has already given you money which means they trust you and expect you to charge them. If you can pull that off this whole problem goes away. You could even provide a annual discount if they purchase the add-on for a years time upfront. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
