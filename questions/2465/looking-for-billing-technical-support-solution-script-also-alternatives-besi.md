## looking for billing & technical support solution/script. also, alternatives beside Paypal?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-26
- tagged: `resources`
- score: 2

are there any open source solutions ? basically, these are the last functional features that needs to be finished. it's very generic, like generating invoice, billing users, sending support tickets, managing them and such.

so looking for (hopefully open source)

    billing system. 
    
    support ticket system.


Additionally, is it wise to use Paypal as the main payment processor ? Are there alternatives ?


## Answer 2466

- posted by: [Paul McMillan](https://stackexchange.com/users/-1/1126-paul-mcmillan) on 2009-10-26
- score: 1

The ticketing support system is going to depend on the scale of your application and how much customization you need. For general purpose use, you might check out OSTicket. I've also used hesk for low volume work.

http://osticket.com/

http://www.hesk.com/

Paypal is expensive, and has a history of arbitrary arbitration decisions, which may not be appealed. 

Recently we've started using [google checkout](http://checkout.google.com/) for our order processing. Their rates are comparable to the other major merchant processors, and without a monthly fee they come out on top. I can highly recommend them as a reliable alternative to paypal. As an added bonus, the arbitration procedures are more transparent and the documentation indicates that they are more likely to provide the merchant compensation in the event of a dispute.

http://checkout.google.com/

Both paypal and google checkout support recurring billing. There are fewer integration options with google checkout, but they are better documented. Paypal's API is poorly written. They both support recurring billing, buy-now buttons, and all the other features you'd expect.


## Answer 2476

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-26
- score: 0

<p>I haven't tried it, but an alternative to Paypal, besides Google, as Paul McMillan answered, is Amazon, <a href="http://aws.amazon.com/fps/" rel="nofollow">http://aws.amazon.com/fps/</a>.</p>



## Answer 2486

- posted by: [Jason Abate](https://stackexchange.com/users/-1/1135-jason-abate) on 2009-10-26
- score: 0

<p>From your question, I assume you're looking for something you can build into your application.  Depending on your platform, something like <a href="http://railskits.com/available-kits/" rel="nofollow">RailsKits</a> might work for you - they provide ticketing and billing/CRM functionality that is straightforward to integrate into your application code.</p>

<p>There are also several billing/provisioning systems such as WHMCS and ClientExec that might also be a good choice.  They've come out of the web hosting world and have a definite tilt toward hosting but have all the main support and billing building blocks.  You'd need to build some custom integration code to tie into your application, but they have pretty clean interfaces to work with.</p>

<p>In terms of payment collection, I think the choice of whether to go beyond just PayPal really depends on your target customer base - if it's just general consumers PayPal is probably file.  If you're targeting businesses, many companies aren't setup to handle PayPal payment.  In this case, adding direct credit card payments and/or check invoices is probably a must.</p>



## Answer 3593

- posted by: [Darius Dunlap](https://stackexchange.com/users/-1/1470-darius-dunlap) on 2009-11-13
- score: 0

Zendesk is worth checking out:

http://www.zendesk.com/

If your needs are more sophisticated (need to track product returns, for example) you may need something more sophisticated. 

Be sure to check out their "Extras" - other tools with which they integrate. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
