## Any experience with StartSSL class 2 certs?

- posted by: [Jewelthief](https://stackexchange.com/users/-1/4547-jewelthief) on 2011-05-05
- tagged: `ecommerce`
- score: 7

I am interested in buying a cert to sign my binaries as well as web server cert. [https://www.startssl.com/?app=2][1] seems to provide it at decent price, but I am not sure if this is a reliable company.

They are looking for passport/company registration information before they can issue cert.  Their website looks crappy and their help email bounces..reducing my confidence.

Has anyone in this forum dealt with them for class 2 certs?

What are other reliable cheap alternatives?


  [1]: https://www.startssl.com/?app=2


## Answer 24455

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-05-05
- score: 8

<p><strong>Googling StartSSL together with common hot words for trouble</strong> -- like "scam", "fraud", "review", "security" -- doesn't seem to bring up anything too onerous. But don't take my word for it, do your own background check.</p>

<p>That said, the big suppliers of SSL certificates are pretty much guaranteed to be pre-installed in all browsers, including the mobile ones. The same can't quite be said for smaller certificate authorities. So it might make sense to hunt around for <strong>Comodo, Thawte &amp; GeoTrust certificates (no special ordering)</strong> on the cheap. Here is a little secret for you, it is often possible to find the brand-name certificates for cheap from other resellers.</p>

<p>Here are some resellers:</p>

<ul>
<li><a href="http://www.trustico.com/">http://www.trustico.com/</a></li>
<li><a href="http://www.namecheap.com/ssl-certificates/comodo.aspx?pricefor=ssl">http://www.namecheap.com/</a></li>
<li><a href="https://secure.ksoftware.net/ssl_certs.html">https://secure.ksoftware.net/</a></li>
</ul>

<p>Feel free to google around for reviews of the above resellers, and for alternatives -- f.x. google "cheap Comodo certificates" or something like that. Also look at your hosting provider, quite often the web hosting provider has special bundle deals available.</p>

<p><strong>One good tip:</strong> When you are done, I would recommend you to use the online test tool at <a href="https://www.ssllabs.com">Qualys SSL Labs</a>. It can connect to your site, and tell you quite a lot about how the SSL is set up, including the certificate chain of trust and revocation state -- which is very handy as a troubleshooting &amp; test tool.</p>



## Answer 39344

- posted by: [Bas](https://stackexchange.com/users/-1/18083-bas) on 2012-05-24
- score: 2

I don't think StartCom / StartSSL is worthy of your trust. My reasoning:

For validation they require a scanned passport and drivers license. Information like this is very sensitive as it can easily be used for identity theft, for instance to acquire a loan in your name.

As a principle, I watermark these documents with the name of the company I supplied them to. They are still perfectly legible but this way, they can no longer be used for identity theft.

Startcom is unwilling to process these watermarked documents because they 'could be forged' (not because they were unreadable or anything like that). Imagine that. Any digital image I send 'could be forged', of course. Adding or not adding a watermark changes little on that account.

And where is the business case on their end? Why do they need (or even want) documents that can be used for Identity Theft? And why won't they process documents that are clearly suited for their purpose of identification?

The only reasons I can think of is that they are either very naive in their security thinking or worse, that they have plans for your documents where the watermark would get in the way. Makes me wonder...

Also please take note that they have been hacked in the past (and admitted to that) so why trust them with you identity in this way?
http://www.theregister.co.uk/2011/06/21/startssl_security_breach/

Bas


## Answer 24461

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2011-05-05
- score: 1

<p>As per Jesper's answer, I had a very good experience with <strong>K Software</strong> (<a href="http://ksoftware.net/" rel="nofollow">http://ksoftware.net/</a>) - they are reseller for Comodo and seem to offer a good level of discount.  In fact, most of my dealing after paying were with Comodo directly - <strong>expect to have to jump through a load of hoops to get any such cert</strong> because it basically says that you are who you say you are, and the issuing company is in some sense vouching for you.</p>

<p>HTH.</p>



## Answer 24472

- posted by: [Joshua](https://stackexchange.com/users/-1/10254-joshua) on 2011-05-05
- score: 1

We use StartSSL at a medium sized university. All staff and students who log in to our Portal (which all students have to do) use the cert. So far, we have had zero issues. Customer service has been excellent. Do be prepared to actually validate. Who you claim to be to qualify for class 2.


## Answer 32426

- posted by: [Max.T](https://stackexchange.com/users/-1/14334-max-t) on 2011-11-09
- score: 1

Basically in order to get StartSSL Organization verification (and certificates) you have to go through personal verification (and pay US$ 59.90) and only then you are allowed to proceed with Organization verification.
But personal verification payment is "non-refundable" and they can delay Org. verification for as long as they like to and with any reason whatsoever till you will go elsewhere for your certificate.
In my case they selected one of the lawyers on documents Apostille (on even on the main corp. documents) and "we trying to call him" for more than a week. Right now I have to go back to Comodo (was using it for 4 years before) for the real certificate and cancel my payment with the bank - waste of time and money!
If you are looking for this kind of "entertainment" - try it yourself.


## Answer 42143

- posted by: [Greg](https://stackexchange.com/users/-1/19790-greg) on 2012-09-21
- score: 1

By far the WORST SSL provided I have ever dealt with. They require way more information then is presented on thier ordering page. Repeatedly asked me for additional CONFIDENTIAL information. Poor english spoken. Difficult to deal with. RUDE RUDE RUDE employees. STAY AWAY - You can find better service somewhere else. 


## Answer 24466

- posted by: [Rob Hall](https://stackexchange.com/users/-1/10253-rob-hall) on 2011-05-05
- score: 0

We use them for all our certificates. Perfect pricing, very helpful company, now a root CA with all the major browsers and their support is second to none. It is common enough for a company to ask for personal as well as corporate identity before issuing certificates so there is nothing unusual there. Hope that helps.


## Answer 24498

- posted by: [Mike](https://stackexchange.com/users/-1/10265-mike) on 2011-05-05
- score: 0

Used them for class 2 for two years now, I havE always had excellent service from them, and the support is superb. 


## Answer 51806

- posted by: [StartSSL Awful](https://stackexchange.com/users/-1/29738-startssl-awful) on 2013-11-20
- score: -3

<p>Have to agree with StartSSL being rude and seems almost like a scam for the class 2 certificate.  I advise using someone else that has decent customer service.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
