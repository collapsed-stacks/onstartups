## Off-the-shelf paywall?

- posted by: [epall](https://stackexchange.com/users/-1/436-epall) on 2009-10-14
- tagged: `payments`, `web`, `subscriptions`
- score: 1

I'm in the process of building a subscription-based content service. Users pay a monthly fee for one of a number of levels of service, and in return get regular emails and website access corresponding to their level of service.

I tend to just write things myself, and it seems to me like ActiveMerchant plus a bit of custom Rails stuff should do the trick, but maybe I'm creating too much work for myself. Is there an off-the-shelf solution out there to create the kind of paywall I'm going for?


## Answer 1399

- posted by: [Doug Bright](https://stackexchange.com/users/-1/324-doug-bright) on 2009-10-14
- score: 5

I was in the same position myself about 6 months ago and wasn't super happy with the solutions I found. All of them took a little more work and a little more money than I wanted to put in so I did something that would get me laughed out of the room if I admitted it.

I punted on it.

I decided that I could deal with automating payment handling when people enough people started paying me that I could no longer do it manually.  I figured it'd be one of those good problems to have.

So when a user subscribed I basically did an INSERT with the payment info and sent myself an email alert that someone had signed up.  The system immediately started treating that person as a subscriber on the site. 

I would manually fetch the payment info out of the DB, delete the sensitive bits and then manually enter it into AMEX/Visa/MC merchant software as a recurring payment. Not exactly PCI compliant but it got the job done.

This of course isn't really the advice you were asking for but consider it if you are just starting up and looking for your first few paying customers. It's not for everyone, but for some of us this is one of those cans you can usually kick down the road a little bit. 


## Answer 1850

- posted by: [Nathan Kontny](https://stackexchange.com/users/-1/973-nathan-kontny) on 2009-10-18
- score: 2

<p>I like Doug's advice.  But there are some services out there that take the headache of doing this a lot less painful, and might be worth exploring a but.  <a href="http://spreedly.com" rel="nofollow">Spreedly</a> is a good one, I've used and would recommend.  Run by a seasoned Rails guy, Nathaniel Talbot, and has some helpful documentation.  And Chargify looks like it might be pretty good as well.</p>



## Answer 19792

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-04
- score: 2

<p>There are plenty of off-the-self paywall systems for WordPress, the ones with any sense hand the payment processing off to a 3rd party gateway (PayPal, Authorize.net, WorldPay) so they don't have to worry about handling the credit cards themselves (and therefore avoiding PCI compliance worries).</p>

<p>Obviously each has their own pros and cons (such as developer support, which payment gateways they support, support of things like "pay per post" etc) and obviously being a WordPress / PHP solution it means you can be up and running in no time and spend your time customizing it rather than writing it from the ground up. Generally they range from free to a free thousand dollars, but take the time to look into which one suits your needs as the more expensive ones aren't necessarily the best.</p>

<p>(ob. Disclaimer. I work for the developers of one such solution <a href="http://www.yourmembers.co.uk" rel="nofollow">www.yourmembers.co.uk</a> but I urge you to look into all the alternatives)</p>



## Answer 1885

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-19
- score: 0

Amember is PHP based, but provides enough integration points with payment processors and third party software like phpbb, and also an API for your own apps. For the money it's probably the cheapest way to get started, although it's not particularly pretty.


## Answer 1863

- posted by: [Rick Montgomery](https://stackexchange.com/users/-1/974-rick-montgomery) on 2009-10-18
- score: -1

Im sorry guys, I am a Merchant Services provider and if you ever get compromised in any way, via hacker or whatever it might be, Visa/MC/Disc/AMEX will put you out of business with fines and assessments and pull your ability to EVER take credit cards.Fines start for 1 offense at $50,000.00, you don't want to go there!!! There are MANY MANY systems that are available and PCI Compliant. We use eprocessing.com for online processing, its easy fast and very little labor involved. One of my biggest clients is processing $100,000.00 per day with about 10 minutes of labor.The fact is this is YOUR business and sometimes there are parts of it that aren't fun but must be done. Email me at rick.mccswi@yahoo.com I will help you with any questions or any advise you may want for free! Not out to sell you, just want you to be educated and informed and NOT compromising your livelyhood!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
