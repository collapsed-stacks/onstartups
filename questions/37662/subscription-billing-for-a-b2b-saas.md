## Subscription billing for a B2B SaaS

- posted by: [user3462](https://stackexchange.com/users/-1/3462-user3462) on 2012-03-28
- tagged: `payments`, `subscriptions`, `micro-startup`
- score: 1

I understand I can either go with a combination of:

Payment Gateway (ex: Authorize.net)
and
Subscription management service (Spreedly, Cheddargettar)

or go with one solution that provides both these functionalities (Ex: Authorize.net, Paypal, FastSpring has a way of handling subscriptions and they can be integrated with their API)

What's the value in signing up with a subscription management service?

I am creating a service that's untested at this point and am looking for a professional way of accepting payments on a monthly basis. I'd like to support upgrades/downgrades/cancellations.

Any suggestions are really appreciated.


## Answer 37663

- posted by: [Jay Neely](https://stackexchange.com/users/-1/1801-jay-neely) on 2012-03-28
- score: 2

Actually, Spreedly just wrote a blog post about this: http://blog.spreedly.com/2012/3/27/spreedly-core-use-cases-single-gateway-why-do-i-need-spreedly

Boiled down a bit, it's because you want the freedom to switch payment gateways (and merchant accounts, which many payment gateways may bundle in). If you're not using a subscription management service (or storing the credit card data yourself *(shudder)*), you'd have to get every one of your customers to reauthorize their subscription with whichever service you switch to.


## Answer 37674

- posted by: [Chris Kluis](https://stackexchange.com/users/-1/9207-chris-kluis) on 2012-03-28
- score: 0

There is also the issue of advanced dunning management that both chargify and recurly include. 

Infact, chargify has a whole email management process for late payments.  I think the value of subscription billing providers isn't just in the ease of accepting payments and flexibility of switch gateways, but their expertise in billing.


## Answer 37812

- posted by: [Dan Engel](https://stackexchange.com/users/-1/17285-dan-engel) on 2012-04-02
- score: 0

It's a question of how much of the work do you want to do yourself. There are full service solutions, which are all-inclusive, making it so there is little development work needed, just about every feature you'd need now/later is available, including global currency, language, and tax support. Then there are plenty of more basic solutions, which may be a good fit for you if you're open to doing a lot of the development work yourself or if you don't need most of the features offered by a full service subscription management and e-commerce solution.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
