## Experience with payment gateway for ecommerce site?

- posted by: [Scott Blanc](https://stackexchange.com/users/-1/2137-scott-blanc) on 2010-03-30
- tagged: `finance`, `payments`
- score: 2

Anyone have experience with ANY of the below payment gateways (some do merchant services as well) that you can comment on:

1. Payjunction
2. Authorize.net
3. Braintree

Looking at these three gateways.  Biggest decision criteria in order of priority:

1.  Look and feel of integration into site (do not want redirect)
2.  Cost (we are membership based company looking to scale from 0-10,000 members in yr1).  Recurring payment fees seem to scale UP and it can get scary.
3.  PCI compliance (overall security) - we are hosting application in the cloud and want to make sure C.C. information doesn't touch our servers (advanced API integration without redirect)
4.  Service - response times and overall service level

Also, anyone who has experience with strong merchants that would take on "high risk" industries, such as Online Dating.. your comments would be much appreciated.

Thank you everyone.

Scott


## Answer 9751

- posted by: [dalenkruse](https://stackexchange.com/users/-1/282-dalenkruse) on 2010-03-30
- score: 6

We've used Authorize.net on 2 e-commerce sites for almost 3 years.  We've had absolutely no problems with them at all.  They have two options for integration: simple and advanced.  The simple integration method requires a redirection to their site.  The advanced integration method allows you to make API calls with your own code so you can retain the look & feel of your site.


## Answer 9752

- posted by: [Dan](https://stackexchange.com/users/-1/2100-dan) on 2010-03-30
- score: 3

Most we know who have worked with Authorize.net seem to be happy with them.  They have a larger feature set than some of their competitors, and they get online txns better than most.  You're right to care about PCI compliance and where CC #s are stored, you don't want to be storing any CC #'s.

- Dan from FastSpring E-Commerce


## Answer 9755

- posted by: [user1377](https://stackexchange.com/users/-1/1377-user1377) on 2010-03-30
- score: 2

PayPal is awful.  Their APIs are in continual flux, their documentation is terrible, their support is abysmal, and their sales staff will outright lie to you ("No, you can't do recurring payments at that level, you'll have to upgrade").

Worse still, their offering isn't fully baked.  As of 4/30/2010 they don't support taxes for recurring payments, so you'll have to do all the accounting yourself and include the tax in your price.  Their test infrastructure requires that you set up recurring payments and then wait for them to fire -- a day later -- to figure out what the actual structure of the messages are.

If you start using them, you'll end up burning a lot of time and making getting away from them a priority.  Stay away.



## Answer 9769

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2010-03-31
- score: 1

We switched to Authorize.net about 18 moths or so ago. We're saving significant money over are old processor and much more happy with the service. So far it's been great.


## Answer 9834

- posted by: [Matt O](https://stackexchange.com/users/-1/2997-matt-o) on 2010-04-03
- score: 1

If you're selling subscriptions or re-occurring payments on your site, Recurly sound very interesting. This is their entire business model, so it's in their interests to get the whole integration as streamlined as possible. I'm hoping to be testing them out in a couple of months.


## Answer 10370

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-19
- score: 0

Integration with Authorize.net or BrainTree is straightforward. BrainTree is extremely fast platform however their built is recurring payment is sub standard. Pure play recurring billing solutions like ipapplications, zuora, vindicia, IMHO are ripoffs with  substantial monthly commits and a percentage of your revenue [ as exotic they might claim, they will eat into your margins]. Another major factor to consider is data portability. That was a big issue for us to allow our data to be transferred to another gateway/provider if needed. In my evaluation I narrowed down the selection to authorize.net, BrainTree and Paysimple. All three had decent offering [ few positives and few negatives ]. In the end we ended up developing our own solution for our unique needs. One of the packages that I evaluated was a product called dotnetinvoice which had much better capabilities than most online providers and integrated with some of the major gateways including paypal, authorize.net etc.


## Answer 10371

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-19
- score: 0

We have integrated Authorized.net payment services for a number of our clients and found Authorize.net to be stable and reliable. I am sure you won't go wrong using them. 

P.S: We are NOT in any way associated with Authorize.net


## Answer 12862

- posted by: [WWonka](https://stackexchange.com/users/-1/3857-wwonka) on 2010-07-19
- score: 0

Have used Authorize.net for the last 4 years, no issues.  Had issues opening an account with Braintree, as any business dealing with anything related to finance or investing it seems, gets more scrutiny.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
