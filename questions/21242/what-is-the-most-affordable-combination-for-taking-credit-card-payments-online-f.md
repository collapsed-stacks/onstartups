## What is the most affordable combination for taking credit card payments online from around the world?

- posted by: [Nikolay Piryankov](https://stackexchange.com/users/-1/8046-nikolay-piryankov) on 2011-03-07
- tagged: `payments`, `ecommerce`, `credit-cards`, `uk`, `shopping-cart`
- score: 2

*I have looked at the **similar questions posted** and believe mine is different - please read the specifics of my question below:*

Assuming we do not want to use PayPal (or Google Checkout etc.), it seems to me that there are a couple of costs we need to think about for taking online payments.

I may be wrong but I believe we have identified the following costs:

1. **software cost** - the e-commerce systems charging you for each transaction.
2. **merchant account** - our bank charges us for taking credit card payments - a fixed fee and a % of the order value (it is significantly less for debit cards though).
3. **currency exchange** - we are selling globally and in various currencies.

Can anyone who has an e-commerce business and uses something other than PayPal (and similar) please suggest a service that creates an optimal mix of the above three, therefore minimising the cost of taking card payments.


## Answer 21246

- posted by: [Sean Harper](https://stackexchange.com/users/-1/8347-sean-harper) on 2011-03-07
- score: 3

The set of service providers between countries does not have very much overlap.  The reason for that is to accept visa and mastercard transactions you technically need to be a bank (or be sponsored by a bank, which is what all the non-bank processors do) and there aren't that many truly international banks. 

The fees involved in accepting cards are:

1. Merchant account fees -- the wholesale cost of accepting a credit card (basically what visa and mastercard charge) are called interchange - here are some benchmarks for averages in the US:
http://feefighters.com/blog/typical-interchange-rates-for-ecommerce-merchants/ and 

*Sometimes* the bank / merchant account provider will simply pass the wholesale rates on to yo with a small and well-disclosed markup (called interchange plus -- http://feefighters.com/blog/interchange-plus/).  More commonly they try to bundle the rates into various categories and play games with them in order to confuse you and make more money.

2. Gateway fees -- usually < $20 / month and another $0.05 or less per transaction.  Sometimes the merchant account provider will bundle the gateway in with the merchant account, but when they do that they usually build in extra fees somewhere (running a gateway isn't free).



As for currency exchange, if you have a merchant account that can accept international currencies you should not have to pay extra for the currency conversion since those fees are already built into the interchange rates.



## Answer 21243

- posted by: [Mike Scott](https://stackexchange.com/users/-1/6167-mike-scott) on 2011-03-07
- score: 2

<p>Your options in the UK include <a href="http://www.worldpay.com/" rel="nofollow">WorldPay</a> and <a href="http://www.sagepay.com/" rel="nofollow">SagePay</a>. But I'm not sure that you'll find them to be significantly cheaper or more fraud-proof than PayPal -- whoever you go with, you should be expecting to pay charges of 3%-4%, and be liable for chargebacks in the event of a dispute.</p>



## Answer 21244

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-03-07
- score: 2

Assuming you get your own **merchant account with a web based gateway**, you only have real two costs (possibly 3):

1) Merchant account fees. They **may** include a small fee per transaction, a **supposedly fixed percentage** of each transaction *(no matter what they say, this percentage actually varies depending on the type of charge card used),* and currency conversion fees. Note you need at **least** two separate merchant accounts, one for Visa/Master Card and a separate one for American Express. Merchant account fees are incredibly complicated and unless you have a specific contract from a specific firm and ask questions, there is no real way to generalize.

2) SSL certificate for your web site. You need an SSL certificate to get an https web address. This is a fixed fee per year (or multi-year).

3) For actual order processing you can write your own order processing page in php or a similar language, or buy shopping cart software.

Finally, when you have your own merchant account you have to pass a yearly compliance test with Visa/MasterCard and a monthly scan of your computer systems. *(This doesn't cost anything, but the yearly compliance test will waste a couple of hours of your time.)*

General US figures for your own merchant account run from 1.8% - 3% for V/MC transactions, 0.00 - $.15 per transaction, generally 1% extra for currency conversion. AmEx runs 2.5% - 3.5% for transactions plus the same 1% (or so) for currency conversion.



## Answer 21632

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-03-15
- score: 2

When it comes to billing software, CheddarGetter is often the cheapest. It also has its own gateway which is convenient, and the gateway works with virtually any merchant account. Internationally, CheddarGetter partners with PayVision, but will accept merchant accounts from other providers. CheddarGetter is also in the process of wrapping up an integration with PayPal, which will allow small or startup merchants who cannot get a merchant account (usually due to low volume) to charge their customers with out one. This way smaller merchants can build their volume making it easier to get a merchant account in the future. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
