## Payment processing questions for yet another SaaS model

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-22
- tagged: `credit-cards`, `payments`
- score: 2

We are working on building an e-commerce solution and offer it as a SaaS. Our service is limited in customer base, as in, we are only willing to provide this to a certain niche [handmade gifts and paintings shops] and we have 12 customers so far and we are not expecting to get more than 30 customers. We would like to be small and service our customers effectively.

One of our services is to host a website along with an online store on behalf of our customers on our SaaS framework. We have decided on various pricing levels based on different "tiers" of service we plan to offer.

Initially we plan to invoice and charge our customers manually to avoid unnecessary fees by employing credit card companies and I am ok with that.

As I mentioned, one of our services would be to have online stores on behalf of our customers where regular shoppers can browse and place orders. 

I have looked into web credit card payment and I think initially, we would like to go with Paypal Pro where the shoppers can pay with any credit card/check/paypal on our site.

How would this set up work? Sorry if I am being too stupid but I cant seem to wrap my head around this concept.

Would you suggest that each of our customers have a paypal account and the shoppers to that store would deal with the customer directly?

Or should there be a master paypal account which keeps track of all the purchases and refunds and monthly or biweekly we settle the accounts?

Estimated cost of purchases placed by shoppers at each of the store will be around $100-$250

Again, I am interested in how to handle the shopper purchases at each of the websites I am hosting on behalf of my customers when I am going with Paypal.

I am looking for any help, guidance, suggestions in this area.

Thank you for this wonderful community and invaluable resources you guys provide.


## Answer 10509

- posted by: [Steve Montgomery](https://stackexchange.com/users/-1/3203-steve-montgomery) on 2010-04-22
- score: 1

I am not a Paypal fanboy or critic, but I can say that I chose not to use them after researching payment methods for a technology licensing business I started several years back.  I don't remember the exact issues, but you can google "paypal sucks" and look at what I read for yourself.

Google has an option that we ended up chosing called Google Checkout.  It is really an e-commerce solution in and of itself, but we used it only as a backend payment processing solution.  We used our own e-commerce suite (built into Joomla) for all of the front end stuff.

The rates are good and, if I remember right, they throw you free adwords advertising based on the amount of monthly transactions you do.

You can always use a real payment gateway and CC processing company, but I can tell you it is a major pain to do that.  For a business your size with the limited number of transactions you will do, using a service like Google Checkout or Paypal is the better deal, I think.


## Answer 18633

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-06
- score: 0

You might want to take a look at FastSpring's subscription service to see if the beta program is a fit for your needs.  PayPal and the other major payment methods are part of the payment options offered.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
