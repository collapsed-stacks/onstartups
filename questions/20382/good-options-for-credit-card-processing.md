## Good options for credit card processing

- posted by: [James](https://stackexchange.com/users/-1/7272-james) on 2011-02-17
- tagged: `payments`, `credit-cards`, `micro-startup`
- score: 4

I'm bootstrapping a micro-startup hosting service with very, very little capital.
 
All of my customers will have recurring billing with a possible trial period. Initially I integrated with [CheddarGetter](http://cheddargetter.com) however I found out that it would be impossible for me to get a gateway account for the first few months since my expected revenue would be so low.

I've looked into PayPal and Amazon's payment services. Both look good, except I don't like the idea of having to break the customer out of my site, but for no monthly fee I can't complain too much.

Which would be the better option? PayPal seems to have clout and acceptance, but I'm already heavily leveraged on the Amazon web services platform and have their branding across my site. 

Are there other payment processing services out there that cater to businesses with limited credit/capital/revenue?


## Answer 20398

- posted by: [Justin C](https://stackexchange.com/users/-1/6947-justin-c) on 2011-02-17
- score: 4

PayPal and Amazon are some of the best ones if you have no budget.

If you get to the point that you have a small budget you can move to a higher service level with PayPal and integrate a payment form into your website. This takes a little programming knowledge so you either need to be a techy, know a techy, or be ok reading lots of articles.

So I would pick PayPal simply because you can continue to grow within their system as your number of payments grows. They also have decent name recognition so while you have to redirect your clients for the time being they are at least being redirected to a vendor that they most likely recognize.


## Answer 20395

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-02-17
- score: 2

You should get your own real merchant account.  For Startups i recommend Kirk McWorther at flagship merchant services... They know the business, and will hold your hand as you grow.  When you process a lot, they can get you interchange plus pricing which will save you a ton compared to paypal or amazon.

As for billing, it depends on your applicaiton.  Cheddar getter falls short, not allowing for pro-rated invoices, and the development overhead is about the same as if you build on top of your own gateway.

For my apps, I use different merchant accounts (all from FlagShip Merchant Services), and all the the Authorize.net gateway.   Auth.net can be programmed in almost any language, and they have a CC vault offering tokenization that makes your app a lot more secure, and avoids a lot of PCI compliance non-sense that is expensive (money and time) to deal with while you are small.




## Answer 20428

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2011-02-18
- score: 2

<p>Transaction size and monthly volume are the true decision drivers here.</p>

<p>Here's a good cost evaluator for deciding between paypal vs merchant.</p>

<p><a href="http://feefighters.com/paypal-calculator" rel="nofollow">http://feefighters.com/paypal-calculator</a> </p>

<p>So, likely your volume will always tip towards paypal.</p>

<p>Luckily cheddargetter is working on <a href="http://support.cheddargetter.com/kb/getting-started-19/how-to-get-a-merchant-account" rel="nofollow">a paypal integration</a> with a target march '11 release date - why not give them a call and see if you can be on their beta?</p>



## Answer 27785

- posted by: [Ian Cooper](https://stackexchange.com/users/-1/11919-ian-cooper) on 2011-07-21
- score: 0

Google Checkout is also a good solution.  Fees are similar to PayPal and they decrease significantly with volume.


## Answer 27812

- posted by: [Bryan Marble](https://stackexchange.com/users/-1/4228-bryan-marble) on 2011-07-21
- score: 0

<p>I think the "next big thing" in integrated CC processing will come out of a company called <a href="http://stripe.com" rel="nofollow">Stripe</a>.  They're in private beta right now and I believe they were founded by a former PayPal founder, but they make CC processing dead simple.  No applications, no merchant account, just a clean API and flat per-purchase rate.  Recently the turnaround time on invites has been pretty low too, so it's worth giving it a shot.</p>



## Answer 34827

- posted by: [Neil Kelty](https://stackexchange.com/users/-1/13978-neil-kelty) on 2012-01-15
- score: 0

<p>One you ought to look into is <a href="http://www.stripe.com" rel="nofollow">Stripe.com</a> The fee is a little bit higher at 2.9% + 30 cents, but the integration is a breeze and it handles all the recurring billing.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
