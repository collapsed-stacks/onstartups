## How do startups sell online, manage customer relationships and support their products?

- posted by: [SomethingBetter](https://stackexchange.com/users/-1/7125-somethingbetter) on 2013-01-13
- tagged: `ecommerce`, `customer-support`, `crm`
- score: 2

We want to setup an online shop for our (physical) products. When a customer registers to order a product, we want this information to be registered to a CRM automatically so we can track our future deals with the customer. Also, we want this information to be registered with a customer support portal (which should include a help desk ticketing system, a user-to-user forum and a download area which can be used to download software/firmware/drivers etc associated with the product) automatically. We want the user to be able to use the same credentials that he/she used during online ordering to login to the support forum / help desk / download area.

It seems to me that these are very common business problems for most start-ups.

Since my search for an integrated solution failed, I would like to hear how other start-ups handle these seemingly standard business problems. I am looking for ideas which can be considered as "best-practices". (For example, maybe it is NOT a good idea to link the web-store and CRM?).


## Answer 45613

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2013-01-13
- score: 3

It's pretty typical for a web application to do one or two tasks really well. But most products don't try to tackle the entire business operation.

Example:

 - Magento: Great at eCommerce but using it as a CRM would not be ideal
 - Desk.com: Great for help desk / tickets - but no commerce or other features
 - Freshbooks.com: Great for invoicing/billing but doesn't do true "accounting"
 - Mailchimp.com: Great for doing client newsletters and mass mailers

The most common approach is to find what products you want to use for what major components you need.  Systems like Desk.com and many other Saas services have very rich web services / API's. You then do "system integration" where you outline a way to pass critical bits of information between your systems using their programmable interfaces.  This would require a web developer to write the integration code to string your systems together and set it up for a single sign on strategy.

This is a very typical approach for many businesses and it IS a good idea to do this type of automation that's why these companies publish API documents.

http://dev.desk.com/
http://developers.freshbooks.com/
http://apidocs.mailchimp.com/
etc.

Find the systems that do what they do best and how you need them to work. Then integrate them.  


## Answer 46633

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2013-01-14
- score: 3

While there are a few full integrations around [InfusionSoft](http://www.infusionsoft.com/), [BrightPearl](http://www.brightpearl.com/) they tend to be very much jack of all trades master at none. I.E suck at everything but in a consistent way. The second issue with all in one systems is they are a single point of failure, if they are down then your entire business is offline.

In the other camp and certainly not best practice most companies simply do not join up their CRM, accounting and fulfilment solution at all or rely on adhoc transfer of spreadsheets. Their are several reasons for this many don't realise they could integrate the various components, several believe its more cost effective to employ an office admin and have this type of data inputting part of their job. Given this is the norm any attempts at an integration will be an improvement on many of your competition.

The 3rd way is to look to integrate where possible specialist software and services.

When looking at specialist software regardless of what role it will fulfil it's worth looking at:

 - Does it have a way to integrate with 3rd party software (normally this would be referred to as a webservice or API) that you can build on?
 - Does it have a pre-existing integration with software you use?
 - Does it support data portability i.e can you get your data out or is it a closed system?

Using one of our clients here is how they are setup:

 - E-Commerce solution: Magento
 - CRM: [CapsuleCRM](http://capsulecrm.com/)
 - Accounts Package: QuickBooks Online
 - Email: MailChimp
 - Fulfilment: Amazon
 - Affiliates: [HasOffers](http://www.hasoffers.com)

In their case Magento is the master record it's regularly backed up, when an order is placed, paid, shipped etc Magento passes this information via the various integrations, several of which are custom built to the specialist solutions. So when a customer is created the information is passed to MailChimp and CapsuleCRM. When a sale is made the information is passed to all of the above barring Amazon. When the item is ready to be dispatched Amazon is notified along with QuickBooks.

In addition to this, CapsuleCRM and MailChimp are linked up, so non registered Magento customers and opportunities can still be sync'd likewise when an email is cleaned in MailChimp the record is updated in CapsuleCRM.

So this means CapsuleCRM holds the information about the person and their experience (using cases for ticketing support, opportunity for presales)

QuickBooks maintains the ledger and accounting information

Magento has all the sales data.

If a member of the sales team wishes to look up a user they do so in CapsuleCRM
If a member of the sales team wishes to look at an order they do so in Magento
If a member of management wants to see profit/loss sheet they go to QuickBooks

This style system is very effective but relies on the individual integrations however if one of the services doesn't meet expectation or fails for some reason you still have all your data and can push it across as all the services have some data portability.

The biggest hurdle is building or finding existing integrations, most popular solutions will integrate with other popular solutions. Even if you are not a developer you can use existing solutions and then services Such as [Zappier](https://zapier.com/) which provide a drag and drop solution to link systems together. Of course in an ideal world you would work with a developer to build an integration that closely matches your needs.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
