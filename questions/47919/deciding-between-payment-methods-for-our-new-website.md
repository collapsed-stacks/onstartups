## Deciding between payment methods for our new website

- posted by: [Sam Kong](https://stackexchange.com/users/-1/25383-sam-kong) on 2013-03-08
- tagged: `bank`, `payment-gateway`, `paypal`
- score: 1

I am developing a website which will charge our customers monthly fee ($200/month) for membership.
So the payment will be recurring automatically.

My client (the website owner) wants to reduce the credit card transaction fee. So I am comparing credit card (through authorize.net), Paypal, and bank wire transfer.

I think bank wire transfer is the cheapest method. However, I don't have any experience with it. Can you shed some light on this? How can I decide what's best between these options?

I am in California. 


## Answer 47928

- posted by: [RichVel](https://stackexchange.com/users/-1/21890-richvel) on 2013-03-10
- score: 2

<p>Choosing a payment gateway and merchant account, and possibly a recurring billing system for subscriptions, is a complex technical + business decision, and you may well need all three.  If your requirements fit a specific 'modern' payment gateway such as Stripe or Braintree you might be able to get away without the recurring billing system.</p>

<p>First you need to do a <strong>lot</strong> of research, and think about your requirements.  As an example, here are some that I wrote recently as part of investigating this space for a UK SaaS startup:</p>

<ul>
<li>Payment gateway - possibly including merchant account</li>
<li>Multi-country - focus on US, and UK, with option for Canada, Aus, NZ. All with home currency billing.</li>
<li>SAQ-A PCI-DSS approval only</li>
<li>Recurring billing via a "vault" service provided by payment gateway (or separate recurring billing such as Recurly or Spreedly) 
<ul>
<li>including "updater" service for card info</li>
</ul></li>
<li>Ability to send reminder emails to users when cards about to expire - has big impact on churn, search for "patio11 card expiry churn" to see blog on this</li>
<li>Easy integration with your software - clean API</li>
<li>Reasonable fees - 2 to 3% or so (probably 3-4% once all cases included)</li>
<li>Simple fee structure!</li>
<li>No arbitrary freezes due to lack of earlier underwriting</li>
<li>Not Paypal (at least to start with) - there are many complaints about their support and occasional freezes on your account </li>
<li>Quick to get accepted (for merchant account) - one week if possible (tradeoff with underwriting) - can be 1-2 months</li>
<li>No charges for free users of your service</li>
<li>Option to create free subscription without credit card</li>
<li>Open door to migrate to another service:
<ul>
<li>Card data easily exportable to another service</li>
<li>Clear early termination fees on merchant account - can be significant</li>
<li>Minimal notice to quit contract</li>
</ul></li>
</ul>

<p>Don't have time to explain all those terms but simply knowing about them means you are thinking about the right things and Google will have info on them.</p>

<p>Important point: many people seem to base their decision purely on the percentage fee taken.  In my view this is a huge mistake - many other factors will be more important.</p>

<p>If you choose the wrong provider(s) and want to migrate elsewhere, it can be hard or impossible to get your customer card data out for transfer into another provider (card data portability is the term).  BrainTree and Recurly are good here, many others don't allow any portability.</p>

<p>If you want to expand to international markets outside US, you will need some abstraction of the payment gateway as the European market beyond UK is entirely different (far fewer credit cards, most people use direct bank payments aka SEPA direct debit).  Here you would need different gateways, e.g. GoCardless or WireCard.  See Spreedly's excellent blog for more on why this matters.</p>

<p>If you are going to build a recurring billing system, you can use Spreedly, otherwise consider Recurly etc.   Generally I would look at the market leading recurring billing systems (Recurly and Spreedly, though Spreedly are changing strategy to become more of a payment gateway abstraction layer) so you can avoid building your own billing system.</p>

<p>Building a billing system is much more complex than most people realise (pro-rating, refunds, credits, upgrades, downgrades, changes in pricing model, sales tax / VAT, etc), and a big distraction for most startups.  Just getting tax correct depends on geographical rules, and in Europe on whether the customer is VAT registered).</p>

<p>My shortlist, for what it's worth based on my requirements for a UK SaaS startup with US/Canada/Europe as key markets, was:</p>

<ul>
<li>1= Recurly + Braintree - good combination of features, can get started quickly</li>
<li>1= Recurly + Stripe (beta in UK) - non-underwriting model, </li>
<li>3 SaaSy - much higher fees but they do everything (chargebacks, billing system etc) and can get started really quickly.  Non-underwriting model.  No card data portability.</li>
</ul>

<p>"Non-underwriting model" means you don't need a trading history to get this service (<a href="http://answers.onstartups.com/questions/35597/suggestions-for-a-merchant-account-and-payment-gateway-for-a-uk-startup-using-re?rq=1">can be a challenge for startups</a>) because the merchant account is run by the service not by you (i.e. like Paypal classic accounts).  The tradeoff is that if you grow really fast or have unusual payment patterns (e.g. pre-orders) your account can be frozen.</p>

<p>PCI approval is a big issue - going for certain payment gateways (Stripe or Braintree) means you can use a 'transparent redirect' or a simple JavaScript embedded form, both of which mean you don't store or even transmit credit card numbers through your site.  This in turn means a much lower cost PCI approval (self assessment rather than a full-blown PCI evaluation) and means you can host on VPSs or cloud.  This factor alone could determine best approach for you, and save far more money than 0.5% on payment fees.</p>

<p>Some useful links from my rather long wiki page on this topic:</p>

<ul>
<li><a href="http://blog.spreedly.com/2013/01/25/startup-ceo-understanding-online-payments/" rel="nofollow">http://blog.spreedly.com/2013/01/25/startup-ceo-understanding-online-payments/</a> - start here, good intro to the main issues</li>
<li><a href="http://news.ycombinator.com/item?id=2444709" rel="nofollow">http://news.ycombinator.com/item?id=2444709</a> - useful thread on Hacker News</li>
</ul>

<p>Personally, I would try really, really hard to stay payment gateway independent if you plan to expand a lot - you can negotiate a better deal when you are larger, including switching gateway, and you can add other payment options such as bank wire transfer later.  Recurring billing systems may also make it simpler to do invoicing of clients, but that's getting into the realm of more complete billing/accounting systems.</p>

<p>Hope that helps!</p>



## Answer 47925

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-03-09
- score: 1

<p>Sounds like you need to do some research on the topic of payment systems. There are tons of little changes you need to concern yourself with when dealing with gateways, processors, and the like - much more than one can cover in this post.  And - if the API is poor, your developers will run for the hills.</p>

<p>You are correct about cost savings if you do a bank ach transfer vs. a credit card transaction - consider doing some reading on vendor sites like <a href="https://www.balancedpayments.com/#processing" rel="nofollow">balanced</a> to learn about whether that is something your implementation can use (<strong>note:</strong> many "ship product to customer" implementations can't use it - delay is too risky) </p>



## Answer 47968

- posted by: [Steven Wagner](https://stackexchange.com/users/-1/25442-steven-wagner) on 2013-03-12
- score: 1

Go with Stripe. 

They do not have the same merchant account requirements that Authorize.net or others have and they can integrate with Wufoo (not required) so you can have a simple payment form. They deposit the money in your account 7 DAYS after which is how they don't require all the merchant accounts. 

Traditional Payment Fees
* Merchant account
* Payment gateway
* Card fees
* Bank fees 
* Subscription service (Recurly, Chargify, etc.)

Stripe fees
* 2.9% +$.10/transaction
* Wufoo ($20/month)~optional

They charge 2.9% which on the surface seems high (plus the 7 days) but compared to some card fees, Amex 3.5+%, Mile or Reward cards in the 3.9% plus your others fees it is a better service. 

One drawback, THEY DO NOT HANDLE INTERNATIONAL commerce! 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
