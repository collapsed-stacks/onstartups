## Free trial in a tiered SaaS application

- posted by: [Anton Gogolev](https://stackexchange.com/users/-1/3720-anton-gogolev) on 2011-10-03
- tagged: `pricing`, `saas`, `trial`
- score: 2

Suppose I have a SaaS application which has several subsctiption plans (think "Basic" for 2 users and this much of storage space, "Starter" for 5 users... you know the drill)  

What will be the the best choice of a tier when creating a time-limited trial account? Signing up for the most beefy (and hence the most expensive) sounds like cheating, but less expensive plans might not have all features available.

I was thinking of creating a somewhat limited "Free Trial" plan which would have all the features available and then warning users as they go along: "if you create one more widget, you'll have to pick an Advanced plan". But again, this might very well scare them off and will generally require a lot of special-casing code-wise. 

Any ideas?


## Answer 30958

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-10-03
- score: 4

I think the free trial period should give them full access to everything. As long as you are clear about the plans and the restrictions, I don't think it's cheating.

Your main goal during their free trial is to get them to convert to your product, if all the features are going to give them the best experience, then give them all the features. You probably hope they go for your most expensive plan too, so why not give them a taste of it.

As long as you are clear about how it all works, then I don't think you need to feel shady about employing proven sales techniques. 


## Answer 30990

- posted by: [romaninsh](https://stackexchange.com/users/-1/13659-romaninsh) on 2011-10-03
- score: 1

Different applications use different approach, and by looking at your competition you might decide to either follow the same pattern or do something radical if you can turn this to your advantage.

If you are doing limited time trial, it would be always with all the features and at the end of trial, useful features would go away. Usually you should give offer with at least 2 product versions (so that users can pick). The most expensive will never be popular, so if you have 3, make the middle-one a "best deal". Don't spend your time and effort on the high-tiered one, simply put higher limits there.

In some cases you can use application without time-limit, but it limits you in some other way. For example you can only add 3 employee accounts. Freshbooks have changed their structure 3 years ago which changed the way how we use it - instead of paid account with 10 users, we started to use multiple free accounts. It might sound like bad idea, but they increased amount of subscribers by a lot with this move, so it helped them to scale-up.

Drop-box is free to use with limited disk space and you get more space if you signup friends. Remember that there are always people who will never buy your app, but you still can use them to promote your SaaS solution.


## Answer 31005

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-10-04
- score: 1

To start with, I would think of 'free trial' not as a special plan, but as a billing capability. 

Then in most cases, I would ask the question, **which is my *default* plan?**

That plan should be one which showcases your solution and addresses the most common use cases. Often you may want to create 'value' plans, with restricted feature sets - but these aren't the default plan.

And I'd offer a free trial of the default plan. That minimizes friction and allows you, for instance, to offer better help and support to triallists, as they all start at the same point.

If you've built upgrade / downgrade logic, in my view it's fine to let this apply to trial users (unless it's not robust in the case of free trials and generates spurious charges or credits), because that lets them get things exactly as they want them going forward. And it means that trials don't have lots of special case logic in them. You'll want to optimize in-app upgrades with paying users, and reap the benefits of this learning in the trial case.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
