## How can you reduce the number of credit card chargebacks for a website selling high value products that are vulnerable to fraud?

- posted by: [Nikolay Piryankov](https://stackexchange.com/users/-1/8046-nikolay-piryankov) on 2011-03-08
- tagged: `payments`, `credit-cards`, `shopping-cart`, `fraud`
- score: 5

From this question on [Merchant Account Chargeback Ratios][1], one answer suggested that websites selling high value items will have higher charge backs because more criminals will attempt to purchase products using fraudulent credit cards.

How can we:

1. **Reduce the cost of chargebacks** if we anticipate we might have a lot?
2. **Prevent fraudulent payments** from going through?


  [1]: http://answers.onstartups.com/questions/21249/merchant-account-charge-back-ratios


## Answer 21270

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-03-08
- score: 7

<p>There are two separate approaches to reducing credit card fraud. The first approach requires the collection of credit card and purchaser data, and then a review of that data. Your order pages should <strong>always</strong> require the customer CVV code, collect their IP address, and their phone number and billing address. While your credit card processor might accept a charge with a bad CVV, or a bad AVS respones (AVS doesn't work in all countries) <strong>you</strong> don't have to accept it.</p>

<p>We hand review <strong>all</strong> high value orders for products that have a high incidence of fraud. The hand review takes less than a minute per order- well worth it for the fraud protection. The reviewer looks at the order in total- does it use a free email address? Does the email address match the purchaser's name? Does the physical address sound reasonable? <em>(This can all be done in less than 10 seconds!)</em> Next, trace the IP address with a service like <a href="http://www.ip2location.com/free.asp">IP 2 Location</a> and make sure it matches the billing address. Finally, <strong>call</strong> the phone number provided on the order form. You can also use Google maps and their satelite view to verify an address exists and that it is a residential or business address.</p>

<p>The second approach to fraud prevention is to protect the actual product you deliver. If they are downloading software- can you issue a temporary key to the software that only works for a fixed period of time? If it is a web service make sure they have limited access until you are sure of their payment.</p>

<p>If you are shipping a physical product to the customer <strong>always</strong> use tracking on the package. You can fight many charge backs (but not all) by showing the merchant card providers proof of of delivery.</p>



## Answer 21265

- posted by: [Michael Pryor](https://stackexchange.com/users/-1/130-michael-pryor) on 2011-03-08
- score: 4

<p>To reduce chargebacks, you should add additional checks during the purchasing process:</p>

<ol>
<li>Require the <a href="http://en.wikipedia.org/wiki/Card_security_code" rel="nofollow">CVV code</a> from the credit card. This should not be optional.</li>
<li>Use the <a href="http://www.maxmind.com/app/ip-location" rel="nofollow">MaxMind GeoIP</a> service to get a 'fraud score'.  Essentially this will tell you if the user with the card is too far in physical space from the bank where the card is from.  This is extremely useful and almost always points out fraud.</li>
<li>Use a tool such as <a href="http://phoneify.com/" rel="nofollow">Phoneify</a> to verify a physical phone number for your purchases.</li>
</ol>

<p>If a purchase fails any of these, you should have your system set it aside for manual review.  If you can't tell whether an order is fraudulent or not after review, just leave it sit.  If it is legitimate, the person will contact you.</p>

<p>Note that having a low chargeback rate will NOT get you better credit card rates.  For each chargeback, you'll just have to pay a fee and you'll be responsible for the loss on any merchandise shipped out, but the credit card company doesn't care about how many chargebacks you have - UNTIL a certain point.   At that point, they will just close you down.  So getting a low chargeback rate is just for your own protection, and won't get you cheaper merchant fees on normal transactions.</p>



## Answer 35729

- posted by: [Dan Grossman](https://stackexchange.com/users/-1/6897-dan-grossman) on 2012-02-05
- score: 1

My business used to have a major chargeback program, so I built a system to call high-fraud-risk customers during the ordering process before charging their credit cards. That weeded out 99% of the fraud... the people with stolen credit cards would not provide their real phone number, or their real phone number would give away the fraud (US billing address, Russian phone).

I built http://www.dialshield.com to offer the same system to others.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
