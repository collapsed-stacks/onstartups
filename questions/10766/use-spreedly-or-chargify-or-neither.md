## Use Spreedly or Chargify or neither?

- posted by: [user2306](https://stackexchange.com/users/-1/2306-user2306) on 2010-04-30
- tagged: `payments`, `saas`, `subscriptions`
- score: 5

I plan to add subscription plan(s) to my website (built using ASP.NET). I may be using Paypal as the payment gateway for now. I might consider adding credit card payments in the future. Although paypal supports monthly subscriptions, it appears that integration, upgrades/downgrades and cancellations become really easy with Spreedly or Chargify.

However, since these services charge money, I was wondering if it's really worth having a service in between your site and the payment gateway?


## Answer 10776

- posted by: [michael](https://stackexchange.com/users/-1/3279-michael) on 2010-05-01
- score: 2

It might be worth looking into recurly as well: http://recurly.com. They don't have a per-transaction fee. 

We're currently looking into using a similar companies to get away from our "rolled our own" system.


## Answer 10772

- posted by: [user3298](https://stackexchange.com/users/-1/3298-user3298) on 2010-05-01
- score: 1

Yes, it is worth it. It can save you a lot of problems in case PayPal decides that you are evil and freezes your account (and they apparently sometimes do so).

Read here how spreedly has saved someone a lot of lost sales because PayPal banned them and they were able to switch very easily: http://cooking.fourbeansoup.com/post/322154074/paypal-is-evil


## Answer 31824

- posted by: [Sire](https://stackexchange.com/users/-1/14002-sire) on 2011-10-24
- score: 1

There are a lot of competent services out there, but they differ a lot in what payment gateways are supported, and also in features and polish. Price is NOT very significant unless you have zero budget, after you get your first 50 customers the price difference is about 3% or less. 

You can sign up to almost all of them for free to compare features and try them out, do this!

Here are a few comparisons:

- http://simplestation.com/locomotion/chargify-vs-recurly-choosing-a-recurring-billing-platform/
- http://bashireghbali.com/technology/compare-chargify-vs-recurly-vs-cheddargetter-vs-braintree-vs-spreedly-vs-saasy/
- http://news.ycombinator.com/item?id=975301



## Answer 10794

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2010-05-02
- score: 0

I would suggest using chargify because they don't charge you until you have over 50 customers. Besides that, the control panel of chargify is more informative.


## Answer 10907

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-05-06
- score: 0

<a href="http://www.braintreepaymentsolutions.com">Braintree</a> also offers managed recurring billing. And to answer your question about if it's worth using a service to manage your billing, we (Braintree) have heard that we've saved merchants lots of time and headaches by managing billing for them. Although we wouldn't have built the functionality if we didn't think it would be valuable. :)


## Answer 31832

- posted by: [Nicko](https://stackexchange.com/users/-1/7870-nicko) on 2011-10-24
- score: 0

I use chargify, and of some of the others mentioned here, I've also looked into Braintree.  You were wondering "if it is worth having[a 3rd party service]." It definitely is.  Depending on your reporting requirements, features desired, integration capability with other platforms, user base - you can come up with your own decision-making criteria.  We built our own payment system for a while, and I'm much happier that we have a dedicated payment platform now.  

I feel that the headaches that went with billing weren't worth it, and I can devote more energy now to building in conversion opportunities rather than managing payments, PCI and all that **** I don't want to touch.  


## Answer 31865

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-10-25
- score: 0

I use Chargify and have been happy enough with the decision. It seems to me they are the best of the choices available, although definitely not perfect.

I wouldn't have rolled my own system though, not just the time to get it up and running, but then the time to maintain and improve it as time goes on. With a system like Chargify, subscription billing is all they do, so they add new features and improvements which you get for no effort down the track. With your own system, nothing improves unless you do it.

As for my experience with Chargify:

**Pros**
- It was quick to get subscription billing up and running
- Good customer support
- They are now adding new features regularly (I suspect since the recent funding boost they got)
- Good set of features (including flexible tax support which was important for me).

**Cons**
- Average documentation
- Average/Out of date examples
- Missing some fundamental features I would expect (reporting is very ordinary without you doing your own) 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
