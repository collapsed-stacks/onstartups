## Handling pro-rated upgrade/downgrades

- posted by: [Nimbuz](https://stackexchange.com/users/-1/19209-nimbuz) on 2012-11-26
- tagged: `subscriptions`, `billing`
- score: 2

I'll be handing recurring billing with pro-rated upgrades/downgrades. Although upgrade seems simple, but I'm unsure wether to provide a refund incase the remainder amount exceeds the required total for the upgrade.

So for example:

 - Plan A: $10/m ($0.33/day)
 - Plan B: $90/yr ($0.24/day)

**UPGRADE:**
User is subscribed to `Plan A` and after `21 days` he decides to upgrade to `Plan B`:

 - $10 - ($0.33 × 21 days) = $3.07 
 - $3.07 + $86.93 (charged on upgrade) = $90 will upgrade him to Plan B

**DOWNGRADE:** 
User is subscribed to `Plan B` and after `21 days` he decides to downgrade to `Plan A`:

 - $90 - ($0.24 x 21) = $5.04
 - $10 - $84.96 = -$74.96 

So my question is what is the standard practice for refunding the downgrade remainder? I have no problem refunding but since my gateway doesn't refund the transaction fees, I'll have to bear it which is not possible. 

I'm thinking of allowing pro-rated upgrades only, downgrades only from the billing cycle, does that make sense?

Thanks!


## Answer 44500

- posted by: [markasaurus](https://stackexchange.com/users/-1/21770-markasaurus) on 2012-11-26
- score: 3

For upgrading your account, I would say either the same day or at the next billing cycle would be fine. As for downgrades, I wouldn't allow it until after their cycle has ended. 

Reason is - you paid a (yearly) amount to save money. If you weren't sure, then you shouldn't have went into a one year contract. 

As for the business owner, this is were a trial for a day or week comes in handy to sell those long-term subscriptions. You as the owner get the money up front. This money is used to invest into your business.


## Answer 44499

- posted by: [ashutosh](https://stackexchange.com/users/-1/18112-ashutosh) on 2012-11-26
- score: 2

Your policy of "allowing pro-rated upgrades", and "downgrades from the billing cycle" only makes sense. I suppose that you are facing the mental block of "dont be evil" while putting this in your Terms&Conditions, but believe me- the mental peace of lesser operational overhead will be negligible if your product is good-Users will ignore that minute detail and it won't be a blooper. 

Or, 
You can also let users opt-for "adjust the remainder in my next month's bill" ; in this case, the user will pay next month=downgraded rent - remainder.
 Only one exception will be there: in-case an user stays for 1 downgraded month, then wants to exit with refund, at that time only, you can opt present him with option to "Deactivate my account and refund my $XX" instead of "Deactivate my account".



## Answer 44630

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2012-11-30
- score: 1

Presumably, the reason you have two different plans is because you want the certainty of having somebody in there for a longer time and are willing to give them a reduced rate for that certainty.  Allowing them to go from Plan B to Plan A doesn't do that.  

Say, after 1 month, somebody on Plan A wanted to switch to Plan B, and then cancel.  Instead of paying the monthly rate of $10/month, dropping down would allow them to pay only $7.50/month.

So, no, you shouldn't let customers down-grade.



## Answer 44622

- posted by: [Sachin Jadhav](https://stackexchange.com/users/-1/21850-sachin-jadhav) on 2012-11-30
- score: -1

You can add the additional amount as credit to customers account and later use it for next billing cycle.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
