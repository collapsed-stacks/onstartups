## Paypal automated pay/receive and success notice with business account? (what if I don't have a business?)

- posted by: [Totty](https://stackexchange.com/users/-1/5231-totty) on 2011-12-10
- tagged: `payments`
- score: 1

I would like to know if is possible to create a system that pay/receive automatically based on what is happening in the site.
I would like to know after a payment that it has succeeded or not in order to activate the service.



I don't have a business so what is my best choice? (country: Portugal)
thanks

Example of what I would like is 99design.com (not exactly how it happens):

 - Users pay to open a new contest
 - Website somehow is noticed by the success of that payment and opens the contest
 - There is a winner and the money are sent to that user and a little commission to the Website


UPDATE:

What I Really NEED:

 - Available in Portugal;
 - API to know if the payment has been done
 - Low fees, I prefer no monthly fees
 - What about if I don't have a business, but just the site
 - Business name instead of my Name when someone receive/pay


## Answer 33575

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-12-11
- score: 2

<p>This is actually some what of a technical question not really a 'start up' question.  </p>

<p>I'm not sure what countries PayPal works in, but whether you have PayPal standard or Pro you can achieve what you are looking to do.</p>

<p>With PayPal Standard there is a concept called <a href="https://www.paypal.com/ipn" rel="nofollow">IPN</a> Instant Payment Notification. You can essentially call a web service or page back on the originating website once they finish the transaction on PayPal. Once IPN calls back to your website you would need to have custom code/logic to mark in your database that the contest has been paid for.</p>

<p>If you were able to upgrade to PayPal Pro in your country you can do a lot of this without the user ever having to go over to the actual PayPal website.  </p>

<p>You would essentially pay commissions out to people by sending them money via PayPal to their email address. </p>

<p>There are probably content management systems or e-commerce systems that may be a good fit for you to automate some of this. It's possible that Drupal 7 and Drupal 7 commerce could achieve this without much programming. (But I'm just guessing).  </p>

<p>Typically this stuff is custom coded for a specific need.</p>

<p>Regarding your update:</p>

<ul>
<li>Available in Portugal ('I think' PayPal is)</li>
<li>API exists for PayPal Standard. See this link for <a href="https://www.x.com/developers/paypal/products/express-checkout" rel="nofollow">Express Checkout</a>, has API docs</li>
<li>PayPal charges a transaction fee under a dollar and a percentage typically 2.5 - 3.3%</li>
<li>PayPal standard has no monthly fee</li>
<li>In the US you don't have to have an actual registered business to do business. There are benefits to incorporating but you can just claim any income on your personal income taxes.  Not sure if it's the same in Portugal.</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
