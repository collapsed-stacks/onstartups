## Online payment processor for items over $1000

- posted by: [Tim Kara](https://stackexchange.com/users/-1/2486-tim-kara) on 2010-04-19
- tagged: `payments`
- score: 1

I know this subject have been discussed in length here and elsewhere, but most of the people that ask what is the best online payment processor never mention the price tag.

My product's minimum order will be around $1000 and goes up after that based on the number of users.

Please tell me from personal experience what online payment processor should I use for such price tag item?

P.S.
Trying to stay away from Paypal.

Thanks in advanced

Tim



## Answer 10393

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-04-19
- score: 4

<p>The <a href="http://www.gibraltarsoftware.com/buy" rel="nofollow">cheapest product we sell is $495</a>, but our average transaction is significantly higher than that (for example <strong>our $2995 bundle is our most popular single offering</strong>) and we use <a href="http://www.fastspring.com" rel="nofollow">FastSpring</a>.  In our case, we handle most of the "shopping cart" aspects of the purchase and once we have a list of items for a customer hand it off to FastSpring to perform the actual purchase.  We have no merchant account, and FastSpring is handling all of the international currency conversion and tax issues, which is a significant thing for us because about 60% of our business is in Europe (and that is split between many countries).  They are also handling the fraud-detection and controlling our charge back risk.  It does cost more than being your own credit card processor, but not a lot more (talk with them about your situation).  At our current volume makes sense for us to simply not have to worry about it.</p>

<p>We do completely electronic fulfillment so one of our key requirements was that we could pass over a completed shopping cart and get back a web service-like hit when it was sold to complete issuing the licenses on our side.  We were able to get that working quickly with them.  </p>

<p>We also offer people the <strong>option of paying by purchase order</strong> if they are making a large enough purchase which makes some companies happy and means we don't have to worry about the FastSpring transaction fee on our larger purchases (which are usually over 5k to want a PO).  </p>



## Answer 10376

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-04-19
- score: 3

<p>It really has nothing to do with how much is your minimum purchase but what is your average volume of sales. If you have a sale once in a  while than PayPal may not be too bad of an option, however if you have a high volume, then you need some sort of payment processor that will be able to offer you a better % rate.</p>

<p>Please keep in mind, though, that most of other options will require additional setup and possibly involve setup fees. Here's a company that has been around for some time and mainly srves smal to mid-size businesses: <a href="http://www.authorize.net/" rel="nofollow">authorize.net</a>  </p>

<p>Some companies may wave their monthly fee if you have no transactions. I used to use <a href="http://echo-inc.com/" rel="nofollow">Echo</a> for that very same reason.</p>

<p>Payment processing is a mature market and you can certainly find a provider that will be able to meet your business needs and sometimes will bend backwards to get your business. Good luck.</p>



## Answer 10380

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-04-19
- score: 3

You should start by talking to **your** bank and asking what they offer in merchant accounts. Note that with an average ticket price of $1,000.00 or higher **any** merchant account is going to want to see a bank account that has had an average balance in the 10's of thousands of dollars for at **least** the last year. Chargebacks come straight from your bank account and no one is going to give you a merchant account where you can quickly take in thousands fo dollars without a way of getting it back if this is a scam.

Once you have a merchant account set up, be prepared to field phone calls from your merchant account provider about large dollar charges. They will call to see if this is correct and may delay payment to your account at first.








## Answer 10432

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-20
- score: 2

Gary, the rates aren't always that high when you use a full service e-commerce service.  In our case the rate for a high priced product is 5.9% plus $.95 per transaction, which is lower than the 9-15% mentioned.

The 1.5-2.5% figure you'd pay by having your own merchant account is a little low, because when you factor in amex, paypal, international, reward, and corporate card transactions the rate ends up blending out closer to 3.5-4%, especially when you account for the chargeback fees that get paid by the vendor if you have your own merchant account. 

Some more info on the advantages of outsourcing vs having your own merchant account is listed here:
http://tinyurl.com/c3t3qq

Hope that helps clarify things a little.

- Dan


## Answer 10433

- posted by: [Stefanos Tses](https://stackexchange.com/users/-1/3178-stefanos-tses) on 2010-04-20
- score: 0

Tim,

Your best bet is too start with a e-commerce provider like FastSpring or Plimus and when you have enough sales, and probably better office infrastructure, get you own merchant account. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
