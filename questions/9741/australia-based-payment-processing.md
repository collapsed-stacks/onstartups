## Australia based payment processing

- posted by: [Shabda](https://stackexchange.com/users/-1/2973-shabda) on 2010-03-30
- tagged: `payments`
- score: 4

Since Authorize.net is US/Canada only, I am wondering if there is a Austrlian counterpart to them providing service similar to them?

What are must have,

1. Recurring payments
2. One time payments.
3. Authorize and capture

NIce to have

Sane API. (Emphasis on sane, :) )




## Answer 9754

- posted by: [Daemin](https://stackexchange.com/users/-1/440-daemin) on 2010-03-30
- score: 3

<p>I'm in a similar situation to you since I'm working on a site that will be subscription based in Australia (for an international audience though). So far I haven't found anything decent for capturing and handling credit cards that work easily in Australia - maybe there's a (very small) market in there?</p>

<p>The current plan for my startup is to use a third party service like <a href="http://spreedly.com" rel="nofollow">Spreedly</a> connected to the payment gateway <a href="http://eway.com.au" rel="nofollow">EWay</a> (which is an Australian one) and then to an Australian bank (which I'm having most trouble with now).</p>

<p>Just a few words of warning though from what I've found so far. </p>

<ul>
<li>Spreedly (currently) only handles recurring payments (subscriptions) but it securely stores the credit card details. No details yet on single payments so you'll need to write something yourself for that.</li>
<li>The Australian banks are geared very much towards shopping cart sites in their merchant account offerings, therefore there will be more work involved for you.</li>
<li>To check off your three points you'll probably need to use a payment gateway like EWay and write a bunch of code yourself.</li>
</ul>



## Answer 27390

- posted by: [jkraybill](https://stackexchange.com/users/-1/11897-jkraybill) on 2011-07-11
- score: 1

I know this question is old, but in case it helps anyone, I just moved to Australia and am evaluating payment processing solutions. I can't vouch for them, having not integrated yet, but a trusted business colleague here says that Payment Express are full-featured and have been good to work with. They may not have recurring payments, but if not, that's pretty straightforward to implement yourself.


## Answer 43980

- posted by: [adnkhn](https://stackexchange.com/users/-1/10532-adnkhn) on 2012-10-31
- score: 1

There is http://pin.net.au where the amazing thing is you don't need an internet merchant account with a bank. They are in closed beta at the moment.


## Answer 28158

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-07-31
- score: 0

I am in Australia and have a software application that takes subscription payments.

I used NAB as the bank for the merchant account, their fees were the lowest when I checked (and for my predicted transaction volume).

I use Chargify for the subscription functionality, they recently added a very good GST module which makes them the best choice in Australia in my opinion.

I then use payment express for the payment gateway, as they are compatible with both NAB and Chargify.

Other than the delays waiting for the various approvals (particularly bank and payment gateway), it was fairly straight forward to set up, and the only coding required was to integrate with the Chargify API.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
