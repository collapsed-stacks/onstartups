## Third-party subscription payment processing like Recurly?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2010-12-03
- tagged: `payments`, `subscriptions`, `payment-gateway`
- score: 7

Does anyone have any experience with third-party subscription payment processing services like [Recurly][1]?

What else is there?


  [1]: http://recurly.com/


## Answer 17396

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-05
- score: 4

CheddarGetter has the best pricing of all of these products.  But most of these products are not viable if you are a programmer or can program your own recurring payments.

We looked at all of the above for a new startup and decided to AGAIN code our own recurring billing.  What were deal breakers for us were:

1. FREE Accounts - All the systems above charge you for the free accounts, otherwise you have to use some trickery and separate your free and subscription customers, making conversions tough. 

2. None support affiliate payments.  One of the most powerful things you can do as a SAAS is to offer affiliates recurring affiliate payments upon billing.  Using the systems above you still have to code that yourself.

3. Unnecessary transaction fees, adding a few cents to every transaction adds up.  That is money better spent of development or marketing.

4. Intergrated metrics.  If you keep billing your own DB, you can intergrate closer with other metrics and analytics.  Over time it becomes a pain to corolate spikes in subscriptions with your marketing efforts.

5. Pro-rated billing.  We pro-rate every transaction. This is important because it lets us handle our billing early in the month.  It allows us to take care of our payrolls, ad costs and more without being a month behind on accounting.  Also lets us schedule our customer retention efforts, and handle declined transactions on a schedule.  If you dont prorate- you will be billing customers throughout the month.  That is expensive investment of your time, considering you could be calling clients 30 days a month to retain their accounts or offer promos.

Look at the systems above for ideas, but you will learn that you could build a very similar system in little time.  If you are worried about storing card data, look at tokenization through your gateway.  Authorize.net makes tokenization very simple. 






## Answer 17372

- posted by: [Kyle West](https://stackexchange.com/users/-1/4267-kyle-west) on 2010-12-04
- score: 3

<p><a href="http://chargify.com" rel="nofollow">Chargify</a> is good. Spreedly and zuora are others.</p>



## Answer 17373

- posted by: [Jeff Epstein](https://stackexchange.com/users/-1/3666-jeff-epstein) on 2010-12-04
- score: 2

<p>You can also check out <a href="http://cheddargetter.com" rel="nofollow">CheddarGetter</a>.</p>



## Answer 17397

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-05
- score: 2

<p>We use <a href="http://spreedly.com" rel="nofollow">Spreedly</a> at Argyle Social.  Very inexpensive and easy to implement.</p>



## Answer 32354

- posted by: [ClayNichols](https://stackexchange.com/users/-1/3534-claynichols) on 2011-11-07
- score: 0

Another is Spreedly.com
They are in our top 2 choices (at least partially b/c they support Quickbooks Merchant Services as the payment processor).




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
