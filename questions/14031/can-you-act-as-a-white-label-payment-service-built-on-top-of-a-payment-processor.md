## Can you act as a white-label payment service built on top of a payment processor?

- posted by: [Javid Jamae](https://stackexchange.com/users/-1/4142-javid-jamae) on 2010-09-12
- tagged: `credit-cards`, `payments`, `saas`, `charging`
- score: 1

Can a company who has a merchant account act as a white-label "middle-man" between another merchant and a payment processing company like Paypal? For example, a white-label company offers an API into which a customer-facing businesses can integrate. The customer-facing business then uses the API to manage and charge credit-card transactions made by their customers. 

I've heard that this might be against the policies of Mastercard/Visa because they want the person with the merchant services account to be the actual merchant that the end user is facing. 

I've looked into Chargify.com (a SaaS offering that manages recurring payments) to see how they operate and they don't act as a merchant. Rather, they allow you (the customer-facing site) to provide your own merchant account information to them, which they use to run the transactions for you. I wonder if a restriction of some sort is the reason they went with this model instead of using their own merchant account.

I'll probably call Paypal and a few other payment processors next week to ask them directly, but I was curious if anybody on here knew or had any experience in this area.


## Answer 14049

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-12
- score: 3

VISA and MasterCard both forbid this "payment aggregation" as part of their merchant agreements.  They want to know that the merchant tied to the merchant account is responsible for the delivery of goods, fulfillment of service, etc.

VISA and MasterCard put their trust in the merchant to fulfill their end of the bargain, and risk users charging back more funds than VISA and MasterCard have currently held for your account.  For this reason, they refuse to process transactions for merchants that are unknown to them.

Now, when you're as big as PayPal, you can negotiate some terms which allow non-merchants to charge credit cards.  But that likely takes a whole lot of insurance, money, and negotiations.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
