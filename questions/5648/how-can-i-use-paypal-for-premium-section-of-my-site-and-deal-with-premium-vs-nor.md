## how can i use Paypal for premium section of my site and deal with premium vs normal users?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-30
- tagged: `payments`, `user-interface`
- score: 1

I want to achieve something like this

http://depositfiles.com/en/gold/payment.php

I have normal users signed up. I want them to upgrade to premium user. Once a person pays, how do I know which user he was signed in ? How do i force the user to login first before being able to click the paypal button and make payment ? Otherwise, I would receive money, but wouldn't know which user to mark as "PAID" in my database.

when you click on the paypal button, it redirects you to the paypal page where you can login and pay.

I also want to accept Visa and Mastercards, is it doable through paypal using the same method ? If not, which gateway will allow me to easily sstart accepting credit cards without having to send business incorporation papers.



## Answer 5649

- posted by: [Dheer Gupta](https://stackexchange.com/users/-1/2052-dheer-gupta) on 2009-12-30
- score: 5

<p>From the sound of:</p>

<blockquote>
  <p>Once a person pays, how do I know
  which user he was signed in ? How do i
  force the user to login first before
  being able to click the paypal button
  and make payment ? Otherwise, I would
  receive money, but wouldn't know which
  user to mark as "PAID" in my database.</p>
</blockquote>

<p>it seems you need a programmer, frankly showing a link to members only is a very simple if loop. But you will need more than just that to make everything work seemlessly. I would recommend using a php/dev forum or something to figure this out. Perhaps you should head over to StackOverflow.</p>

<p>Alternatively, the simplest way to handle this is to integrate a script which is already designed to handle member areas, payments etc. A good script in this aspect is <a href="http://www.amember.com/p/" rel="nofollow">Amember</a>. There are other options too, just google "<a href="http://www.google.com/search?q=integrating+paypal+into+website&amp;btnG=Search" rel="nofollow">integrating paypal into website</a>" or use other more specific keywords.</p>



## Answer 5668

- posted by: [Nathan Kontny](https://stackexchange.com/users/-1/973-nathan-kontny) on 2009-12-30
- score: 2

<p>You could also look at things like <a href="http://spreedly.com" rel="nofollow">http://spreedly.com</a>.  They've got some good documentation on making plans like this and adding them to your site.  </p>



## Answer 5665

- posted by: [Chris Dansie](https://stackexchange.com/users/-1/2053-chris-dansie) on 2009-12-30
- score: 1

Depending on your programming ability one of these might be a good fit.

https://cheddargetter.com/

http://www.paysimple.com/products.html









## Answer 5670

- posted by: [Jason M](https://stackexchange.com/users/-1/2070-jason-m) on 2009-12-30
- score: 1

PayPal offers a couple of services.  Based on your comments, I assume you are using the PayPal payment option.  They also happen to offer a payment gateway -- the Payflow Gateway, which was purchased from VeriSign several years ago.  Payment gateways do not process payments.  Gateways provide the infrastructure to connect to a payment processor.  

Gateways abstract the connection infrastructure from the actual processing of the payment.  However, they typically charge a per-transaction fee on top of the cost of processing credit card payments (interchange).  If you want to avoid this fee, many payment processors offer direct connections to their solutions.  You will still need to pay the cost of processing the payment, but you can cut out the $0.02 - $0.25 per transaction that would be spent on a gateway.

The downside to this approach is that you will likely be building a connection to a proprietary solution.  It may be cheaper to process, but it isn't easy to switch processors without rebuilding some of the connection work that you have put in place.  

Big gateways:

 - PayPal's PayFlow Pro
 - Authorize.net

Big processors:

 - First Data 
 - Chase Paymentech
 - Global Payments
 - Merchant e-Solutions
 - TSYS
 - Elavon

As volume grows, you should always work to renegotiate your rates!  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
