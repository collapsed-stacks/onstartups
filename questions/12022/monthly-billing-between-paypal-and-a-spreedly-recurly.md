## Monthly billing between PayPal and a spreedly, recurly

- posted by: [user3635](https://stackexchange.com/users/-1/3635-user3635) on 2010-06-11
- tagged: `charging`, `monetization`, `webdev`
- score: 1

Paypal's simplest integration is an IPN and is super simple, but we all know the risks, and how badly they handle monthly billing. But it takes an hour to set up and is $.30 + 3% or something.

It seems like the next step is authorize.net ($99 + $20/mo), a 3rd party app like spreedly or recurly ($20/mo), and an SSL certificate ($300?). 

Am I missing a middle step? Is there's something for $20/month and that's it?


## Answer 16594

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-11-17
- score: 2

Yup.
Authorize.net and other Gateways still need a merchant account which has fees close to .30+3% or something.  You usually end up paying more if you have few transactions, and less if your have more if you go with  you own gateway.

My advice, plan big, and get a real merchant account with the authorize.net gateway.



## Answer 29319

- posted by: [Quang](https://stackexchange.com/users/-1/12982-quang) on 2011-08-27
- score: 0

I believe for SSL you can get a Geotrust RapidSSL from NameCheap.com for $11/year

Not sure if it'll work for you, but possibly.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
