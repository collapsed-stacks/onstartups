## Verisign vs. Thawte? Looking for advice

- posted by: [Chris](https://stackexchange.com/users/-1/412-chris) on 2010-10-05
- tagged: `security`
- score: 7

Our SSL certificate with Thawte is about to expire and I was wondering if this is still the best route.

Any recommendations?


## Answer 14809

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-10-06
- score: 8

<p>This question is an old one. Here is <a href="http://serverfault.com/questions/62999/choosing-the-right-ssl-certifcate">one little contribution</a>, also look at the SSL tags at ServerFault. <strong>I see no reason to focus on Verisign and Thawte, unless you strongly believe that their site seals improve your conversion rate. And if that is the case, then go the whole way, and get a Verisign Extended Validation certificate.</strong></p>

<p><strong>My take, in short form, is that your choices are:</strong></p>

<ol>
<li>A name-brand SSL certificate with clear root chain, but purchased from one of the cheap resellers at &lt; 50USD. By name-brand, I mean a certificate with the same signing root as the big players use -- Comodo from a cheap reseller, RapidSSL (cheaper GeoTrust), InstantSSL (cheaper Comodo), et cetera.</li>
<li>A name-brand SSL certificate with a nice logo / "trustmark" to put on your shopping cart ("Secure by ..."), purchased directly from the issuer (I like DigiCert).</li>
<li>A name-brand <a href="http://en.wikipedia.org/wiki/Extended_Validation_Certificate">Extended Validation certificate</a>. So far, you need to work directly with the issuer to get approved for these, there is a fair amount of paperwork required to prove identity, and the prices are high often > 250 USD/year.</li>
</ol>

<p>I would personally <strong>either</strong> get a cheap Comodo or similar certificate from:</p>

<ul>
<li><a href="http://www.ksoftware.net/ssl_certs.html">Here, ~50 USD</a></li>
<li><a href="http://www.namecheap.com/learn/other-services/ssl-certificate-pricing.asp?pricefor=ssl">Here, less than 100 USD</a></li>
<li><a href="http://www.trustico.com/">Here, GeoTrust and Verisign too.</a></li>
</ul>

<p><strong>OR, I would get an Extended validation certificate.</strong> (In other words, of my options 1, 2 &amp; 3, I personally think that 1 &amp; 3 are the good choices.)</p>

<p>I'm still on the fence with regards to <a href="http://en.wikipedia.org/wiki/Extended_Validation_Certificate">Extended Validation</a>. What they're trying to do is a good thing, and the extra consumer confidence they can provide is a good thing, possibly lowering abandonment rate. All the big names (Microsoft etc) use EV certs now. On the other hand, I have not seen a definitive usability study showing that the really work, that end users really grok the difference.</p>

<p><strong>The more expensive non-Extended Validation certificates are a bit of a scam, really.</strong> They don't add any authentication or encryption beyond what the really cheap ones provide. Don't overbuy, i.e. don't think that the 200 USD non-EV certificate is necessarily better than the 50 USD non-EV cert with the same root.</p>

<p><strong>Last bit of advice:</strong> If you take the cheap route, then look at your current domain registrar, DNS host, and web hosts. Sometimes they can sell you a cheap certificate with the same trust root as everyone else, and a streamlined buying process because they already have your domain information.</p>



## Answer 14798

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-10-06
- score: 4

You would do well to compare the prices of the exact same certificate from Verisign, Thawte, and Comodo. They all offer virtually the exact same service. But their prices vary rather dramatically.

Every current version of Windows (XP, Vista, Win 7, etc) comes with equal built in recognition for certificates from all three provders.



## Answer 14818

- posted by: [sk24iam](https://stackexchange.com/users/-1/4660-sk24iam) on 2010-10-06
- score: 2

I plan on buying a Godaddy certificate.  Not nearly as expensive and the name is there.  


## Answer 14816

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2010-10-06
- score: 1

+1 for taking a look at Comodo certificates. We've been using them for years.


## Answer 16951

- posted by: [AviD](https://stackexchange.com/users/-1/2018-avid) on 2010-11-25
- score: 0

<p>Most of the other answers here deal mainly with the price.  </p>

<p>Another aspect is the security the certificate provides - see <a href="http://security.stackexchange.com/q/90/33">this question</a> on ITSecurity for a discussion on that.<br>
Though the bottom line is pretty much "any of the well-known CAs can do the job well enough" (though in some situations there might be some benefit to some).</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
