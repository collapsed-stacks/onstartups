## Charging annually based on number of users. How to grant flexibility on the number of users?

- posted by: [Clash](https://stackexchange.com/users/-1/21685-clash) on 2012-11-19
- tagged: `pricing`, `saas`
- score: 5

We have a product that the customer pays based on the number of users. Suppose it costs 10$/mo/user and that the client has 10 users. That is, he pays 100$ per month for his 10 users. We want to offer a discount if he pays it anually, making it 1000$ for 1 year. However, the number of users may float every month, so how can we grant flexibility for the customer? We don't want him to only be able to have a maximum of 10 users. Suppose that on the 2nd month he has 5 additional users, totaling 15 users. Should we bill him for the 5 additional users? Or should we reduce time from his 1 year quota?

How about if we introduced a new currency, let's call it credits. Each credit is worth 1 user*mo. Using the previous example where he had 10 users, by paying anually, what he is doing is actually buying 120 credits. Now if he has 15 users, it would use 15 instead of 10 credits per month and his time would just end shorter. Is this an acceptable solution or is it too complicated?


## Answer 44331

- posted by: [Billy Chan](https://stackexchange.com/users/-1/21618-billy-chan) on 2012-11-19
- score: 2

I suggest not to use credit, which may make things complicated.

Your original idea is easy to advertise and remember:

"All customers only need to pay 10 months if paying annually."

For the situation of changing scale, it's just some recalculation work done by computer.

For example, after used 4 months under 10 users plan, the customer want to increase user numbers from 10 to 15, then program do the following:

1. Stop the old plan of $1000 per year
2. Calculate the balance of old plan: (1000/12)/*(12-4) = 666.67
3. Calculate the new balance needed for new plan: ((15*10*10)/12) * 8 = 1000
4. Calculate the balance the client needed: 1000-666.67 = 333.33  
5. Charge client for the balance and start new plan which only lasts 8 months.

For downgrading, it's similar, just replace charging to refunding.

This solution should be very fair to customer. They can feel free to do anything, upgrade, downgrade, with only balance charged or refund.

Your bottom line should be only accepting changing plan based on month, but not days which is too ridiculous. If a customer want to change plan from 10 users to 15 at Nov.20, sorry, I need to charge whole November as 15 users, or starting from next month.


 


## Answer 44339

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2012-11-19
- score: 1

How you manage this and do your billing reminders is another question, but since you don't offer any number of user discounts, it seems like you have individual annual licenses. They purchased several at a time, so those will all expire at the same time and the customer has the option to renew as many as they want. There isn't going to be a single annual billing renewal. 

You could avoid this, if you allowed them to not only get a discount for paying the annual fee upfront, but also pricing breakpoints for total number of users. This may allow a growing company to plan ahead if they feel they will reach one of your breakpoints during the year. 

Try to keep some negotiations open. If they add a user or two in the last quarter of their contract, you may want to let them have those for free, knowing they're working on their budget for next year. This could be an incentive to renew.

I wouldn't take too drastic of measures to alter your billing until you see this as a significant issue with your customers. Although they may like the single payment for simplicity and a discount, they may not want to over-commit, so they pay monthly for the extra couple of users for the rest of the year. Maybe their staff size is seasonal? You really have to see how they react. 


## Answer 44332

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2012-11-19
- score: 0

If they tell you they need five additional users for a month, they will expect to pay $50 extra, using your figures ($10/month/user).

Don't need to make it any more complicated than that.


## Answer 44338

- posted by: [DJClayworth](https://stackexchange.com/users/-1/12762-djclayworth) on 2012-11-19
- score: 0

Allow you users to buy 12 months of N user-licenses up front for ten times then monthly cost. If they don't go over N users then they pay nothing else. If they go over N then they pay an extra 1/N of the monthly fee for each user over.

If after M month they think they are going to have more users on a regular basis, they can stop their yearly contract and replace it form one with a higher N. Credit them with M twelfths of their annual payment back and put it towards the new annual payment. The twelve months starts again from the new payment.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
