## Barriers to truly global payment processing?

- posted by: [anthon](https://stackexchange.com/users/-1/238-anthon) on 2009-10-11
- tagged: `ideas`, `payments`, `credit-cards`
- score: 6

As a startup in Australia, one of the problems commonly faced here is getting a suitable payment service that customers world wide can use.

It seems that since the implementation of global AML/KYC legislation, payment providers are hesitant to offer a service that is too flexible to ensure compliance with the aforementioned legislation.

In your experience as startups and those that require payments, what do you see as being the biggest barriers to making providers like Authorise.net offer a flexible service? Or is this something that most startups in North America/Europe don't need to worry about, given the great majority of your customers are based in your regions.

What would you recommend for an Australia based provider? Should we incorporate overseas to overcome this or is there a service out there I haven't found?

 


## Answer 994

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2009-10-12
- score: 1

Even the big players, eBay, Google, Microsoft don't have global processing privileges for their users. Here are my suggestions -

 - PayPal can help you cover many countries including Australia.
 - You can try services like this - http://www.kagi.com/kagisolutions/index.php?page=wwpay
 - Then you can geo-target users and show payment options relevant to them.


## Answer 1495

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-15
- score: 1

<p><a href="http://www.nab.com.au/wps/wcm/connect/nab/nab/home/business%5Fsolutions/1/3/4" rel="nofollow">NAB Multi Currency Acquiring</a> might be worth a look. In addition to AUD, this lets you accept payments in "US Dollars, Canadian Dollars, Euros, Pounds Sterling, Japanese Yen, New Zealand Dollars, Singapore Dollars, Hong Kong Dollars. Other currency transactions are settled in Australian Dollars."</p>

<p>I have no real world experience of this product so this is not a recommendation, just something that I'm aware of and that you may wish to consider. I'd expect that you'd be paying a premium in merchant fees, forex fees etc. for this service, and I am not sure what to do about other currencies (I'd like Indonesian Rupiah but that's a tough ask).</p>



## Answer 1553

- posted by: [Daemin](https://stackexchange.com/users/-1/440-daemin) on 2009-10-15
- score: 1

<p>I've been looking into this as well recently - as I'm in a similar boat to you, global startup in Australia. I've found that most banks have about two classes of merchant setups that deal with Internet payments. Either by using their service which allows you to redirect to a form they host for the purchaser to enter their credit card information in, or by creating a merchant account and using some other 3rd party payment processor.</p>

<p><a href="http://www.eway.com.au" rel="nofollow">eWay</a> seems to be a popular payment processor, and is supported by some US based subscription management systems, notably <a href="http://spreedly.com" rel="nofollow">Spreedly</a>. (These are the providers that I'm using for my startup, so the appropriate disclaimers apply.) There are other payment gateways out there so check with your bank as to which ones they support. </p>

<p>If you want to go with a USA based payment gateway then from what I've been told you need to get a US based bank account, as well as a Federal Tax ID (or something equivalent with a different name). So far I haven't been able to get a quote out of these US based payment gateways so I don't know if doing the paperwork is worth it.</p>



## Answer 20985

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-03-01
- score: 1

I use Moneybookers, this is actually quite an international approach they have also suited for all size of merchants: http://www.moneybookers.com/ads/merchant-account/


## Answer 989

- posted by: [user574](https://stackexchange.com/users/-1/574-user574) on 2009-10-12
- score: 0

I can't speak about Australia, but here in the States we have the same issue. Finding and implementing a global payment system is tricky. My last startup used CyberSource which, at the time, was only able to accept USD payments. Once we launched in Europe and Asia this was an issue.

Once we picked a new back-end, CyberSource was able to accept other currencies. The issue though, was that we needed bank accounts in every country in which we wanted to collect funds. As a small company, this proved impossible.

I have since started a new company and need to find a global solution as well. I look forward to hearing from other people on this topic.

Rick




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
