## How do you bill for customisations in your SaaS offering?

- posted by: [Kosta Kontos](https://stackexchange.com/users/-1/16592-kosta-kontos) on 2012-02-24
- tagged: `pricing`, `saas`, `strategy`, `billing`
- score: 1

We provide a customisable SaaS solution, and have adopted the classic billing model of a monthly user subscription fee. However some of our clients also require us to make customisations to their instances from time to time.

Currently, if the customisation can be refactored into the main / shared codebase (thus allowing all of our clients to benefit from it), we do not bill for it. But the majority of customisations are client-specific, in which case we bill per hour (albeit at a significant discount to market-related hourly rates for software development).

I know of some companies that don't bill for their time at all, and others who bill for everything. What are your thoughts on the various strategies?



## Answer 36540

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-02-24
- score: 1

If it is a good idea I want to see globally in my SaaS, I do not take money for it.

If it is specific for only one customer, they need to pay the customization. You have also to consider if this customer can get upgrades of your product later or if the version is really forking away... in the later case this might become pretty expensive if you don't bill the change.

The best way would be to have a plugin architecture in place which does not (or less) conflict with the mainstream app. Again, I would work on a monthly rate.

Not billing for customization... well, not my cup of tea. 


## Answer 37530

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-03-25
- score: 0

We have a couple products and we handle it like this:

 - **Good idea for a feature:** We tell the client we will add it to our feature log which we work off of based on the priority we think is most important for all of our clients.  However, if this is critical and you would like to pay for the feature we can expedite it and move it higher up the list. Yes, you will be paying for this and the feature will be given to everyone else as a standard product upgrade.
 - **Bad feature idea / specific to them:** This feature is going to take your developers off of your core product and prevent you from helping the rest of your customers for some period of time. Yes you better charge for it and you better make it worth it to you :]  Some SaaS/Product companies make a fortune at this charging HIGHER then market programming rates. This is also difficult for you to maintain long term as they are not on the standard shared code base.  Their monthly fees and everything should be altered to compensate for this.

 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
