## Is there a service like chargify that will do recurring billing, but allows variable monthly charges?

- posted by: [Jack](https://stackexchange.com/users/-1/4925-jack) on 2010-10-21
- tagged: `ecommerce`
- score: 3

This is a hypothetical question, but say I run an email hosting service and I want to charge my customer a fee per month for each email account that he has set up.  Let's say that the email accounts are $1 per month each and when he first signs up he had 5 email accounts, but gradually adds more each month.  Is there a recurring billing service that would allow me to add and subtract from the total recurring charge instead of just setting the fee during the initial account setup?

I'm also a bit confused about the need for a payment gateway and a merchant account.  I'd really like the payment and all of the legal requirements that go with that to be offloaded to this service if possible.


## Answer 15433

- posted by: [kurt.heinrich](https://stackexchange.com/users/-1/4659-kurt-heinrich) on 2010-10-22
- score: 2

Have you seen Chargify's component pricing? http://chargify.com/blog/new-feature-quantity-based-components/

And Chargify does not replace a merchant account and gateway. It's just a billing system. You'll still need to get a merchant account and gateway to accept credit cards.


## Answer 15453

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-22
- score: 2

What you're looking for is typically called metered billing. Recurly does support this, and you can read more about it at http://docs.recurly.com/subscription-plans/metered-billing.

You could also easily accomplish this by updating the quantity of the subscription as the user adds or subtracts more emails. 

A payment gateway is the company that actually processes credit card transactions, while a merchant account is your bank. Some companies (like PayPal or Intuit) offer both in one. At Recurly, we are PCI compliant, so you don't need to worry about the additional fees and security associated with accepting and storing credit card data.

If you have any other questions, feel free to give me a shout at rachel(at)recurly(dot)com. Sounds like we'd be a good match for you!

Rachel
Recurly Support


## Answer 27022

- posted by: [Jessica](https://stackexchange.com/users/-1/11639-jessica) on 2011-07-01
- score: 1

I know that CheddarGetter is set up to add tracking information to all your billing plans; so, in your case, you would be able to set up an automatic piece of code that would see when someone increased or decreased their emails, and CheddarGetter would change their plan accordingly.  We use CheddarGetter for a SaaS we're about to release, and we have it set up in a similar way.  It was very easy to implement!

Also, we're using CheddarGetter for both the billing management software and the billing gateway.  All we had to do on the side was get the Merchant Account, which made it a lot less of a hassle than if we had to get all three.



## Answer 15431

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2010-10-22
- score: 0

<p>Have you looked at <a href="http://www.freshbooks.com" rel="nofollow">Freshbooks</a>? They may be able to help you. You can also do this kind of thing with programs like Quickbooks as well.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
