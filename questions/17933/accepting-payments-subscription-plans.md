## Accepting payments... subscription plans

- posted by: [Igorek](https://stackexchange.com/users/-1/4395-igorek) on 2010-12-17
- tagged: `credit-cards`, `payments`, `charging`, `billing`
- score: 7

So, I am a total newbie when it comes to payment processing, acceptance of payments, subscription plans, etc.  
I've recently built out the SaaS offering and will be in beta with it through the end of the year.  The service however has stabilized and I am ready for the payment part.

Before I ask my detailed questions, here is how I would like the payment processing to look like:

 - All users will be charged a monthly fee, from $0/month through  $550/month, depending on the plan they chose.  I suspect majority of users will be on a $40/mo plan. There are 5 plans total.

 - In addition to flat monthly plan cost, all users can be charged extra for over-usage if they go over the limits of their monthly plan. This fee will be calculated at runtime on a monthly basis 

 - Consequently, there maybe other additional features in the future that I would to add charges for

 - My software is in .NET and runs in the cloud (Windows Azure) 

 - I /need/ to bill on a monthly calendar basis (1st through 31st).  This is because over-usage is being tracked on a calendar monthly basis 

 - I would like to accept payments from customers from all over the world and not be tied only to US.  (Why would someone not do this from the get-go?)

 - I would like to NOT keep any CC/payment information myself and outsource all the processing to a 3rd party

 - Users register on my site, pick a plan and I will use  my API when they register for service.  They will get a free trial.  I would like them to enter their CC information sometime after they registered for an account and tried the product for a while.  





I'm really interested in learning about two things if I can:

 - Having never dealt with online payments & processing, where should I go to LEARN about the payment architecture for such a requirement as mine?  What are the do's and don'ts?  What are the gotchas?  I'd prefer to not have 1000 URL's to browse through but 1-2 sites that contain all the basics.

 - Any recommendations for a 3rd party vendor that would suit my particular requirements the best?

Thank you kindly


## Answer 17969

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-18
- score: 7

You can use a service such as CheddarGetter.com to simplify your transactions for subscriptions, but you will quickly learn that its best to build your own subscription system.  It's easy, it gives you ultimate control, and worthwhile doing versus services that exists.

you will need:
1. Merchant account
2. Gateway ( I highly recommend Authorize.net)
3. A way to store customer cards (not on your server)

For a merchant account, contact Kirk Mcworther at flash ship merchant services.  It will cost you around $40 per month, but you will get great rates, and in the long run could get interchange plus pricing. 

The gateway gives you access to an API to process transactions.  Authorize.net is very easy to code in C# with plenty of code examples.  Authorize.net also offers you a credit card vault, where you dont store credit cards in your DB, and therefore dont have to worry about PCI compliance and extra security risks.  They do this by tokenization, what it essentially does is send you back a token for each credit card you store in the vault, your system can then reference a stored credit card by token, rather than the card details.


Last, if you have a monthly service, serisously consider pro-rated billing.
Here is a scheme that I find works VERY well in B2B apps.

1. Offer a trial, without a credit card required.  We do this very similar to rackspace email apps, where we offer 14 days free trial.  Since we built our own payment systems, we allow the customer to convert the trial to a real subscription at any point, but keep the remaining free days.  You cannot do something like that with the subscription services that exist.

2. We offer upgrades and downgrades, this is next to impossible to do with Paypal subscriptions (they limit the % of increase you can do), and with services for subscription billing its a hassle to code. 

3. Pro rate where you have your customers billed on the 1st of the month.  For your 500 plan, if someone signed up today, they would be billed for only 14 days out of 31 days remaining in December (45% x 500), then full $00 on the first of the month.
The reason pro-rated billing is great is it allows you to focus on your collection efforts early in the month, freeing up the rest of your time for marketing, building features, and retaining customers who let their cards expire, or cancelled.  If you bill on a daily basis, its hard to focus on your other goals while random transactions appear.  Also pro-rated billing helps you get a way better grasp of how your business is doing on a monthly basis.


Coding your own solution takes a few weeks worth of work, but its the best option for handling overages, late charges, etc.  Plus the few cents you might spend per transaction using a 3rd party service add an unnecessary layer of overhead, and risk that if that service fails your income pipe is down. 


Best of luck on your Azure app.  I really think its a great idea, and would like very much to see it be a great success.

FB


## Answer 17935

- posted by: [John Sjölander](https://stackexchange.com/users/-1/5866-john-sj-lander) on 2010-12-17
- score: 3

<p>If you like a tighter integration with your site and service I highly recommend using</p>

<ul>
<li><a href="http://www.freshbooks.com/" rel="nofollow">Freshbooks.com</a></li>
</ul>

<p>They provide an Invocing API that works really well, and a multiple of external addons for everything from payments to CMS integration. It's really excellent. </p>

<p>Arpit's answer is also good, if you want to rely more on an external supplier, and are not customizing much.</p>



## Answer 17951

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2010-12-17
- score: 3

I don't know of a place that offers comprehensive explanations for this. 
jumpstartcc.com will give you an overview of what's involved in credit card processing. 

Basically, there are three parts to it:

 - merchant account (you could get that at your bank)
 - payment processor (e.g. Authorize.net, they will store CC details for you)
 - subscription management service (Recurly, Spreedly, Chargify etc.)

I think there are services that provide all of this for you (e.g. BrainTree Payment Solutions). 

All your requirements other than charging for over-usage seem straightforward, so you'll just need to understand which providers allow dynamic charges. Accepting payments from outside the US shouldn't be a problem as far as I know. 


## Answer 17934

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2010-12-17
- score: 2

Go through these providers and as you gain more and more customers, you'll need to switch to other providers depending on your experience and needs.

 - PayPal.com
 - Kagi.com
 - FastSpring.com

I guess information offered on these websites will be sufficient to understand online payments and processing.


## Answer 17982

- posted by: [Jeff Epstein](https://stackexchange.com/users/-1/3666-jeff-epstein) on 2010-12-18
- score: 1

<p>Other 3rd Party Billing Applications include:</p>

<ol>
<li><a href="http://chargify.com" rel="nofollow">Chargify</a></li>
<li><a href="http://recurly.com" rel="nofollow">Recurly</a></li>
<li><a href="http://spreedly.com" rel="nofollow">Spreedly</a></li>
<li><a href="http://cheddargetter.com" rel="nofollow">CheddarGetter</a></li>
</ol>

<p>They are all pretty comparable.  Chargify and Recurly probably have the most backing.</p>



## Answer 17940

- posted by: [AAA](https://stackexchange.com/users/-1/6037-aaa) on 2010-12-17
- score: 0

One good subscription site is zuora.com


## Answer 18127

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-22
- score: 0

<a href="http://www.ariasystems.com">Aria Systems</a> provides exactly the type of Billing & Subscription Management you're looking for. We offer two products for startups like yours. First is the Aria Billing Platform, which allows you to manage the entire subscription process, from Customer Acquisition to Billing/Invoicing to Reporting & Analytics. This is not just our core competency of billing & invoicing, we're designed to help with the entire customer lifecycle. Secondly, we offer Aria SubscriptionsPlus, which is Aria Subscription Billing with our partner PayPal - it's at a great price point for startups & small business. 

To answer one of your questions, in this space, you'll see geographic limitations with the third party payment gateways/payment processors - some are US only, while others are global.


  [1]: http://www.ariasystems.com
  [2]: http://paypal.com/subscriptionsplus


## Answer 19064

- posted by: [Daemin](https://stackexchange.com/users/-1/440-daemin) on 2011-01-17
- score: 0

Just to answer one part of your question: 

> I would like to accept payments from customers from all over the world and not be tied only to US. (Why would someone not do this from the get-go?)

I too was looking to accept payments from customers all over the world (and am in a similar situation to yourself). This really depends on what you mean by accepting payments from all over the world. This can mean accepting payments:

* from customers that reside in any country in the world, or
* in different currencies used by your customers.

Now in the first situation this is handled by just accepting one of the common currencies (which I would put to being US Dollars, British Pounds, or Euro's) and letting the credit card networks automatically take the payment and convert it for you. This will cost a small extra percentage amount of the transaction, charged to either the customer or you, although it seems to be most often on the customer side. I'm unaware if the merchant also gets charged this, although it wouldn't surprise me.

As far as the second situation goes you'll need to put in a lot more extra effort as the whole payment processing pipeline will need to be done for each currency, and you'll need a merchant bank account that can handle all of the different currencies. These do exist, and it is possible to set this up, but it's a whole lot of extra work for a startup to do, and the accounts themselves are quite expensive - fee wise.

Now you might think that doing the second option - charging in different currencies - would be nicer on the end user, and to some extent it is. But speaking as someone from outside of the US, it doesn't matter that much, and it would matter a whole lot less for businesses. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
