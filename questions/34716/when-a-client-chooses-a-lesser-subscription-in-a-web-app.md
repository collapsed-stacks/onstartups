## When a client chooses a lesser subscription in a web app

- posted by: [Mihalis Bagos](https://stackexchange.com/users/-1/15564-mihalis-bagos) on 2012-01-11
- tagged: `pricing`, `business-plan`, `webapp`, `subscriptions`
- score: 1

What happens when a user had a greater subscription plan but chooses to convert to a lesser one?

Of course, the features should be locked/limited, but what happens for example in this case:

    Subscription: GOLD
       Maximum clientele: 500

    Subscription: Silver
       Maximum clientele: 200

Will you just simply not let them add more clients, or force them to delete some of the clients?

What happens in this more intricate case, where the client is able to add another user to help him manage stuff:


    Subscription: GOLD
      Maximum additional Managers: 5

    Subscription:Silver
      Maximum additional Managers: 2

Is is clear that 3 manager accounts have to lose access, but which ones? Again, do you simply not let the client register more managers, or force him to select which ones to keep?

Maybe a universal policy isn't really feasible, but I think a general guideline arises from examining the two aforementioned examples. Do you have any other examples/suggestions? 



## Answer 34718

- posted by: [Paul Cezanne](https://stackexchange.com/users/-1/14795-paul-cezanne) on 2012-01-11
- score: 7

They should not be allowed to downgrade until they drop the manager and clientele counts to the silver level. 

If you were to enforce this, by dropping say the most recent managers (or least recent or even random managers) then the customer would have a right to complain. "Hey, you dropped my favorite one."

By prohibiting the downgrade, and instead popping up a dialog telling them to reduce their usage, you've put the selection process into their hands, which is where it should be.


## Answer 34722

- posted by: [Ryan Chatterton](https://stackexchange.com/users/-1/3753-ryan-chatterton) on 2012-01-11
- score: 2

Thanks Mihalis,

I like to compare fremium models to other businesses using them. Take Wufoo for example, known for incredible customer service.

When you downgrade with them and are above the form limit or are using other premium features, **they ask you to remove the excess forms before you are able to downgrade.** Additionally, this experiment was done with a premium account attempting to downgrade to a free account.

If your user is using the service at the gold level, then it's likely that he really needs the features contained within. **Take this opportunity to explain *personally* the benefits of his plan and that you're *personally* concerned** that downgrading would limit his growth, stifle his productivity, etc, etc.

That being said, if this is happening with a lot of your clients, it's possible that your pricing may be too high or that you aren't offering enough benefits with the gold plan for them to be satisfied. **Try rewarding the 'golden ones' with some extra fluff.** 

Finally, you can try to create something in between the two levels. **Maybe silver is too low for your clients, but hey have no other option.**



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
