## Accept credit card payment within your site?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-20
- tagged: `payments`
- score: 3

Right now we use Paypal Website payment standard.  

Ie- customers pay using Credit Card or Paypal on Paypals site (redirected from and back to our site).

We'd like to keep customer on our site for credit card payments.

How can we accept credit card payment directly within our site ?

- Is Website Payments Pro easy to integrate with?
- Does it allow recurring subscription as well? 
- Can you remember credit card and then able to auto-bill people as part of a "top up" function?

Would appreciate any advice..
Simon


## Answer 12904

- posted by: [dalenkruse](https://stackexchange.com/users/-1/282-dalenkruse) on 2010-07-20
- score: 4

We've used Authorize.net on 2 e-commerce sites for almost 3 years. We've had absolutely no problems with them at all. They have two options for integration: simple and advanced. The simple integration method requires a redirection to their site. The advanced integration method allows you to make API calls with your own code so you can retain the look & feel of your site.

Disclaimer: I'm not affiliated with them, just a happy customer!


## Answer 16486

- posted by: [Dustin Boswell](https://stackexchange.com/users/-1/5295-dustin-boswell) on 2010-11-14
- score: 1

<p>I've been researching this lately too, and two services I'm considering are:</p>

<ul>
<li><a href="http://www.braintreepaymentsolutions.com/" rel="nofollow">BrainTree</a></li>
<li><a href="http://chargify.com" rel="nofollow">Chargify</a></li>
</ul>

<p>Both of these specialize in recurring billing, and have an API so you can embed in your site (programming required of course).  These are both shiny "web2.0" companies, so their interfaces are nicer, and their APIs cleaner.</p>

<p>I currently use Paypal (standard) too, and looked into Paypal (PRO) - apparently it does support recurring billing (<a href="https://www.paypal.com/us/cgi-bin/webscr?cmd=xpt/Marketing/general/RecurringPaymentFAQs-outside" rel="nofollow">paypal</a>). As a developer, I personally find the Paypal site annoying (their website is outdated, their documentation is confusing), so I'm looking elsewhere.</p>

<p>As for remembering customer's credit cards, all of these services do this for you. As far as I can tell, there's no need for an online company to store credit card info themselves anymore.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
