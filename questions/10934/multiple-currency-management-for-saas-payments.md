## Multiple Currency Management for SaaS Payments

- posted by: [Dario Solera](https://stackexchange.com/users/-1/1539-dario-solera) on 2010-05-07
- tagged: `saas`, `pricing`, `payments`
- score: 1

We'll soon exit the beta stage and start charging for our SaaS solution.

We're based in Italy so we work in Euros. We think we should also offer the solution in US Dollars, however we find it hard to come up with a decent solution that:

 1. keeps our operative margin under control (as we pay our bills in Euros)
 2. keeps USD prices steady enough not to scare existing customers.

In our case, customers top-up their account every once in a while and we charge them for their daily resource usage (like Google AdWords). 

Would it be too bad to only offer a EUR pricing in your opinion? It would simplify things a lot, however it would (probably) turn down quite many US potential customers. On the other hand, we would have to update pricing frequently (especially these days), so it doesn't make that much of a difference to US customers on the final price.

A possible solution is to update the USD prices every three months, but how to handle existing balance? In the end, we would have to change prices so that with the same resource usage, one day we charge you X, the next day we charge you Y. Basically, the price change would be applies to the existing balance too. It's a bit of a mess.

On the other hand, if we cast our USD price in stone, we would take an enormous exchange rate risk.

Any suggestion on how to handle all of this?


## Answer 10962

- posted by: [Denis Hennessy](https://stackexchange.com/users/-1/311-denis-hennessy) on 2010-05-08
- score: 2

I've gone through this recently with a SaaS offering as well. In the end it comes down to this:

**Don't make a product choices that makes your accounting easier at the expense of your market size!**

If you're selling to a global market then the de-facto global currency is USD (I say this as a non-US resident). People are comfortable paying for online services in USD. If you choose to charge in EU, then it may not reduce your European customers but it will certainly reduce your US customers (who will somewhat distrust it). If you put a value on this, it's certainly greater than the minor cost of accounting for the currency exchange.

And another thing - don't try to charge variable-tax based on the location of your customer - it confuses them and impedes sales. Work it all out _after_ you get the sale.


## Answer 10948

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-05-08
- score: 1

Dario - I think it depends on your target market.  I run a small business and we use a variery of SaaS type products that are priced in USD, GBP and EUR.  It doesn't bother me that we're paying a varying amount each month for USD subscriptions because **the amounts are reasonably small**.  If you have a great product and its pricing is below some sort of pain threshold, your customers may not care, as long as they don't have to do the foreign exchange themselves.  (I think this works fine for credit card and direct debit billing, but it's no good for regular standing order payments as these expect to be a fixed amount.)

Of course, I am to some extent giving the European viewpoint; because we're used to dealing in many currencies (historically) and we often buy stuff from the US in Dollars, we're perhaps more tolerant - it would be interesting to get a US perspective.  It's possible that Americans will be put off your service because they perceive it to be a foreign operation and perhaps less trustworthy - here offering USD pricing might improve adoption rates in the US.  Perhaps other, US-based readers could comment?

One final point: hedging is of course an option to manage your exchange rate risk, but as it's effectively a form of insurance, there is a cost attached to that too.  I think it all depends on the sums involved.

Hope this helps.


## Answer 10936

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-05-07
- score: 0

Get financial advice. Depending on your size you may be able to:

* Adjust your USD Priices like every 3-6 months.
* Hedge your risk for that timeframe using financial instrument (Futures, Forex, CFD.

Basically - you need to have a good estimate of your income for the time period. Then you "speculate" against the price. If for example you get more EUR for the USD you earn, the speculative account will have a loss similar to the gain you have in the currency. OTOH, if you "loose" money because you get less for the USD your customers pay you, the hedging account will have a complementary income. There is some more gains with interest differences, but at the end it is some pretty standard math for hedging.

You can easily hedge up to about 12 months out, though the capital requirements. Every futures broker in the US may be able to help you (you are not a "high income" but a "steady small income" customer for them).

This is basically how large companies hedge stuff - like deliveries for airplanes etc. You can sell of the exchange risk against the possible exchange gain.

If you want you can contact me by email and we can set up a phone call so I can explain that in more detail - I do financial software and some trading and once upon a time did learn all that for a job in another profession (broker, series 3 and 7).

This is basically as good as it gets if you want to offer USD Prices without exchange risk - OTOH, naturally, you can not sustain a hedge indefinitely. Note: there is NO speculation in hedging.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
