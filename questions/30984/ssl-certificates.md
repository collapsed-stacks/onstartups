## SSL Certificates

- posted by: [DMoore](https://stackexchange.com/users/-1/13608-dmoore) on 2011-10-03
- tagged: `website`, `security`
- score: 4

For an e-commerce site accepting payment information, I am being told I need to get an SSL Certificate.  My hosting provider offers it for $99/year plus $25 initiation.  Prices vary greatly -- e.g. verisign is much more expensive.  

Does it matter which SSL I choose?  Is there a difference in quality or reputation or is that the same thing in this context? Is there any reason why renting through my host gives an advantage?

Obviously I don't want to waste money paying extra for nothing.  Appreciate any thoughts on how to make the decision.

Not sure if this is the right place to add this but -- from everything I have seen, the two disticntions between SSL certificates is the impact/value to the customer of seeing a particular SSL badge and possibly the quality of customer service, though frankly I am not sure what I will need their help for once the certificate is issued.

Anyway, I guess the ultimate question is, how much does the consumer care whether it is Verisign (expensive) or Commodo (cheaper) who is managing the SSL process? Does the customer care whether it is an EV certificate or not? If the customer is more likely to transact based on a particular seal, maybe it makes sense to pay more?  


## Answer 30987

- posted by: [romaninsh](https://stackexchange.com/users/-1/13659-romaninsh) on 2011-10-03
- score: 4

The cheapest one would do fine. You can even find a free HTTPS certificate, try http://cert.startcom.org/

Sometimes you need certificate for things where trust is important. For instance if you building a Domain Registrar star-up you would need to purchase SSL cert worth around $1k to communicate with Verisign API. More expensive certificates means there is more authority behind them and some companies would simply require you to have them.

Your hosting company's offer seems fair. Cheapest paid certs on godaddy is 69/y but your hosted might request you to pay extra for using 3rd party cert.


## Answer 31025

- posted by: [José Ceale](https://stackexchange.com/users/-1/13673-jos-ceale) on 2011-10-04
- score: 1

You can have a Comodo SSL certificate for only 35 euro/year:
https://www.sslcertificaten.nl/SSLCertificaat



## Answer 31086

- posted by: [Rob R](https://stackexchange.com/users/-1/13692-rob-r) on 2011-10-05
- score: 1

The SSL certificate you will want, will simply depend on need. As others have stated, if there are no other requirements, other then the simple need to have your site secured by SSL, any will really do and there is no need to over spend.

However, be aware, that are some differences in "types" of SSL's. Such as, a wildcard SSL, which will cover all subdomain names. Ex: www.domain.com, sub.domain.com, another.domain.com, etc. There is also an extended validation certificate as well. This certificate requires a higher level of verification in signup, however, will provide extra browser information to your users as well. Depending on the browser, it could mean a full green address bar, drop down with full SSL information, etc.

Also, realize, that sometimes the SSL you choose, will relate to customer assurance. If people are buying stuff from you, they want to feel their data is safe.


## Answer 31082

- posted by: [dpac](https://stackexchange.com/users/-1/10195-dpac) on 2011-10-05
- score: 0

yea, customers wouldn't care that much about the brand name of ssl. But they definitely look for ssl in the site. I usually get it from clickssl.com, they have good deals and comparison for different kind of ssl certificates.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
