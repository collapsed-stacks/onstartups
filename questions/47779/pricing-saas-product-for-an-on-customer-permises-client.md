## Pricing SAAS product for an on-customer-permises client

- posted by: [carbuncle](https://stackexchange.com/users/-1/25263-carbuncle) on 2013-03-01
- tagged: `pricing`, `saas`
- score: 0

We are selling a Ruby on Rails application on a SAAS model.
The monthly fee is determined based on the number of operators and the number of projects each customer is using.

We have been approached by military contractor (their identities has been confirmed) who seems really interested in buying our software. However they :

 1. Would like to have a "one off" fee
 2. Have the software run on their servers

They don't want to benefit from future updates of the software and they are ready to pay for several month of support to help them install and setup the software on their servers.

So basically it would be a deal like : "get $XXX, come and install you stuff on our servers, show us how to use it and never hear from us again". Or at least that's the plan.

How can we estimate the price tag we can put on that. We have been talking about the number of users / projects they tell us they would use, so we were going to multiply the monthly price tag for this by a certain number of month (how much) and add a premium to get it on their servers. But we have no way to ensure that they are not actually giving us a number of users/projects that is far below their real use.

Is there any industry standard or the like to calculate that ?

 


## Answer 47781

- posted by: [bhttoan](https://stackexchange.com/users/-1/23673-bhttoan) on 2013-03-01
- score: 2

We get asked to do this all the time but have always pushed back and said no - our business model is SaaS and if the potential customer doesn't want to use that deployment method then there are plenty of other providers who provide an on premise offering.

The reasons we decided not to do this are:

1. Support - they will expect support. With no visibility or control over the hardware or software platform can you really support your offering without doing extensive compatibility testing first? Even if they agree to deploy on your recommended hardware and software that will be upgraded at some point and it may break - how would you manage that?
2. Updates - they may say they don't want updates but if something breaks or there is a security bug which you become aware of you will have to provide an update. What mechanism do you have to test and distribute the update?
3. Your code will become available in the public domain - you could use something like ionCube but it is an additional cost and more complexity to support.

Basically, if you were adapting or changing your business model to add this for anyone who wanted it then it may make sense as you would have these processes and procedures in place for many customers but to do it as a one off doesn't make business or technical sense especially as they are unlikely to want to pay more for the privilege of getting it on premise.

It is hard to turn down revenue in business but sometimes it is better in the long run to do that as it can cost you much more in money, time and reputation later down the road.


## Answer 48343

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2013-04-02
- score: 2

If you are not doing this for others and don't really plan on offering this model to others I wouldn't do it.  With your saas offering ou are trying to build a predictable business model.  Predictable in your monthly revenue, predictable in support and maintenance.  

As soon as you start having variables outside of your control you are opening yourself up for those late night calls and emergencies.

If you are on the fence about it, then price it something you would consider ridiculously high. If they don't buy it good, if they do buy it, well at least it is **very** worth it. Don't bust out of your business model for money... only bust out of it for a ton of money.

I don't know what the industry average is, but let's assume that your average customer stays with you for 3 years. On average, 3 years is how long a customer uses your software.  At a minimum I would charge them 3 years x 12 x your highest plan.  Minimum. 

Plus they must have a Purchase Order with $X,XXX for support at $XXX/hr in case they need it. If they don't great. If they do then you don't want to have to hassle with getting your money. You want there to be an open PO that you can bill against no questions asked.

I understand it's hard to turn away money. But when I think back on deals I said no to, I never, not once, have regretted saying no to those. 

If you decide to do it, just make sure it's **more than** worth your while and be comfortable justifying it to them. 





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
