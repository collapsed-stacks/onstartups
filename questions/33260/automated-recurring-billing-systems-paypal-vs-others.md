## Automated recurring billing systems Paypal vs others

- posted by: [Jewelthief](https://stackexchange.com/users/-1/4547-jewelthief) on 2011-12-02
- tagged: `payments`, `ecommerce`, `payment-gateway`
- score: 6

We have today paypal integration, which was very simple, one time purchase.

Now we want to into recurring payment model and charge users on monthly or yearly basis. We would also allow users to buy addons by paying one time fees.

Should i consider Paypal recurring service or should consider services like Chargify, recurly or similar services?

What are some major pros and cons of using both sets of systems


## Answer 33297

- posted by: [SimonF](https://stackexchange.com/users/-1/14817-simonf) on 2011-12-04
- score: 2

<p>I assume that you are using Paypal because you don't have/want to deal with the "full stack" required for credit card processing (i.e. bank account, merchant account, payment gateway, etc.).  If this is the case and you want similar convenience for processing recurring payments, I would take a look at <a href="http://www.saasy.com" rel="nofollow">Saasy</a> or <a href="http://www.stripe.com" rel="nofollow">Stripe</a>.  They provide a full service and, from all accounts, are easier to integrate and more reliable than PayPal for recurring billing scenarios.  I have experience with Saasy and have been very happy with it to date.</p>

<p>There are pros and cons to each, or course.  </p>

<p>Saasy is a product from FastSpring and is well established, works with companies pretty much anywhere in the world and has great support for developers but takes a fairly large chunk of the sale (around 9%).  Stripe is newer, so less proven, and only works with companies in the US at the moment, but takes a smaller cut of sales (around 3%).</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
