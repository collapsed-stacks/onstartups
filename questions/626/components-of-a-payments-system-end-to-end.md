## Components of a payments system (end to end)

- posted by: [anthon](https://stackexchange.com/users/-1/238-anthon) on 2009-10-11
- tagged: `payments`, `subscriptions`, `credit-cards`
- score: 3

What are the components of a subscription/payments processing system/platform?

Does anyone have a good explanation of how providers like Zuora, Authorise.net etc. come together?



## Answer 629

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-10-11
- score: 4

Here are the parts:

1. Authorize.NET and such are "payment processors."  They take credit card info and handle the authorization and fees with the card companies.
1. You also need something called a "merchant account."  This is the bank account where the processor deposits money.  You'd think they could just deposit it into your standard checking account, but they don't.
1. The credit card companies (Visa, Amex) talk to the processor so you don't have to do anything there.
1. Fraud and chargebacks are also handled by the processor.

That's it!

If you use PayPal, that's all-in-one.  They run the card and put in your PayPal account and you don't need the merchant account.


## Answer 743

- posted by: [Denis Hennessy](https://stackexchange.com/users/-1/311-denis-hennessy) on 2009-10-11
- score: 2

Jason covers the lower layers pretty well. However, for subscription payments there's frequently an additional service - a "subscription processor". Examples in this space are Zuora and Spreedly. 

Don't confuse some payment processors ability to do recurring payments with proper subscription processing - there are lots of edge cases around plan upgrades/downgrades, free trials, card changes, etc that the dedicated services do well.


## Answer 660

- posted by: [Puneet Gangal](https://stackexchange.com/users/-1/439-puneet-gangal) on 2009-10-11
- score: 1

Here are the "parts" in a payments system:
1. A payment gateway - like Authorize.net is one example. There are many others...
2. Merchant Account - This is where the payment processing occurs. 
3. Your normal checking account
When your customers enter their credit card information on your shopping cart, the payment gateway provides a mechanism to route that transaction (it depends on your implementation of the shopping cart, but there can be different ways to route - route directly, route through your server, etc.)
Your payment gateway will need to have your Merchant Account information, which is where they will route the information to. This tells your Merchant account provider, your payment processor to process the payment, i.e. charge the credit card of the customer and if approved settle it.. which means they deposit the money into your checking account. 

Some providers are a one stop-shop, like the leading banks - BofA, Chase Paymenttech, etc. or you can work with these provider individually. To streamline the process, you might want a single vendor, but the biggest thing to keep in mind more than the $$, is the integration and support. 

Hope this helps!


## Answer 1537

- posted by: [anthon](https://stackexchange.com/users/-1/238-anthon) on 2009-10-15
- score: 0

So does this sound like a subscription solution?

My application, interfacing through to Zuora/Aria to manage the subscriptions and then linking Zuora/Aria to Paypal who can then either provide the merchant account, or function as a gateway to a merchant account with a bank?


## Answer 1608

- posted by: [Paul O'Brien](https://stackexchange.com/users/-1/759-paul-o-brien) on 2009-10-15
- score: 0

Highly recommend PayPal; its easy to use and comprehensive.  Besides their new API is plugging in countless third party apps that make it even more valuable; we just plugged in to automate bookkeeping and accounting for businesses using PayPal.


## Answer 10765

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-30
- score: 0

Stay away from Zuora. It's not worth the headache. I tried the billing app, and it was just awful to integrate with our billing system.  They seem to think they have a great product, but it's just hype with a headache.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
