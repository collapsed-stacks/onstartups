## Low price merchant friendly payment gateway

- posted by: [Iam](https://stackexchange.com/users/-1/15609-iam) on 2012-01-14
- tagged: `payments`
- score: 1

Without getting into too much detail, we need to lot of transfer of large amounts upto $1000. However that's not our revenue.

We need a payment gateway which offers low fees ACH transfers, preferable below $0.50 per transactions. Do you have any recommendations?


## Answer 36172

- posted by: [Dan](https://stackexchange.com/users/-1/16275-dan) on 2012-02-14
- score: 1

<p>Have you looked at Braintree Payments?</p>

<p>Maybe <a href="http://www.feefighters.com" rel="nofollow">Fee Fighters</a> can find something for you.</p>



## Answer 34810

- posted by: [Rick Button](https://stackexchange.com/users/-1/14549-rick-button) on 2012-01-14
- score: 0

<p>If you don't have a merchant account or are OK with dumping your current one, you can go with <a href="http://stripe.com" rel="nofollow">Stripe</a>. They integrate the gateway and the merchant account into one and essentially just expose it with an API. I use it for a product and it is really good. Their pricing is pretty good,(no flat rate, 2.9% of volume + $0.30 per transaction if I remember correctly).<strong>I don't know how they handle large transfers, however.</strong></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
