## e-commerce provider for an EU based startup

- posted by: [Branko](https://stackexchange.com/users/-1/670-branko) on 2009-12-31
- tagged: `ecommerce`
- score: 0

I am starting a software company located in the European Union. I wrote a B2B product that is in beta test at the moment. Based on my market research and analysis I expect to make 50% of sales in USA, 30% in EU and the rest in other parts of the world.

Which e-commerce provider would you suggest for me? Is it better if I use an EU based provider like ShareIt or is the location of the e-commerce provider not important?

Thanks,  
Branko


## Answer 5755

- posted by: [Denis Hennessy](https://stackexchange.com/users/-1/311-denis-hennessy) on 2009-12-31
- score: 3

<p>It's not clear whether you're looking for a provider to just process payments for you, or whether you're also looking for someone to handle registration and fulfilment. It's worth considering them separately:</p>

<p>I'm assuming you are going to accept credit cards directly (i.e. not via a paypal account or one of the other proxy channels). This means you have to follow these steps:</p>

<ol>
<li>Apply for a credit card Merchant Account (either with your current bank or another in your country). It's typically difficult to get one from a different country.</li>
<li>Find a Payment Processor and supports the bank of your merchant account (authorize.net are the big one in the US, realexpayments and sagepay are two I know in Europe).</li>
</ol>

<p>Then, you need a storefront solution that supports your payment processor (there are lots to choose from, examples are shopify and oxcommerce).</p>

<p>Finally, you may need a solution to handle license key generation and user registrations. I'd recommend looking at Shine because it's free (<a href="http://clickontyler.com/blog/2009/08/shine-an-indie-mac-dashboard/" rel="nofollow">http://clickontyler.com/blog/2009/08/shine-an-indie-mac-dashboard/</a>) although I haven't tried it myself.</p>

<p>My hunch is that it's best to keep away from the all-in-one solutions like ShareIt - they look pretty pricey to me and it'll be hard to move later.</p>



## Answer 5776

- posted by: [Dan](https://stackexchange.com/users/-1/2100-dan) on 2009-12-31
- score: 1

You may want to take a look at FastSpring E-Commerce.  There is support for multi-currency transactions, foreign language order pages, global tax collection, wiring vendor funds overseas, etc.  

Hope that helps.


## Answer 5799

- posted by: [Dmitry Leskov](https://stackexchange.com/users/-1/2093-dmitry-leskov) on 2010-01-01
- score: 1

Stay away from any and all services that Digital River owns. We had been mostly happy with element 5 (which also owned share-it!), but in a couple of years after the DR acquisition the quality of their service has degraded so substantially that we had to start looking for alternatives.

FastSpring is good, but IMHO not B2B ready yet. As of today (Jan 01, 2010), they don't accept wire transfers and have no written quote request automation in place. They promised to have those features available soon, so I sincerely hope this paragraph will be outdated.

Of the newcomers, <a href="http://www.cleverbridge.com/">cleverbridge</a> also looks interesting, but I am so allergic to .NET that I am yet to give my demo account a shot (their control panel is a .NET desktop app, and they say many of its features are absent in the Web admin interface.)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
