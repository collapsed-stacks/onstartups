## Payment Solution Nightmare

- posted by: [Josh](https://stackexchange.com/users/-1/28287-josh) on 2013-10-15
- tagged: `payment-gateway`, `paypal`
- score: 2

<p>I have a small problem - trying to figure out a way of doing the following:</p>

<ul>
<li>Accept payments without redirecting</li>
<li>Take staged payments (it's a subscription service)</li>
<li>When the payment is pulled on a periodic basis, take a cut and redistribute to sellers</li>
</ul>

<p>I know, individually, these are easy to implement using PayPal, but all together?</p>

<p>Any help/suggestions would be greatly appreciated.</p>



## Answer 51401

- posted by: [Arsham Mirshah](https://stackexchange.com/users/-1/28291-arsham-mirshah) on 2013-10-15
- score: 3

<p>Not sure if you're a developer .. or have development resources ..</p>

<p>You need either:</p>

<ul>
<li>Stripe (stripe.com)</li>
<li>Recurly (recurly.com)</li>
</ul>

<p>Either of those systems will allow you to pay commissions on each successfully collected payment.</p>

<p>Then, you'll need a developer who is familiar with the system you choose + jQuery &amp; AJAX to implement the non-redirect solutions you speak of.</p>

<p>If you don't have one, try odesk (odesk.com) or elance (elance.com) to find one.</p>

<p>Hope this helps :)</p>



## Answer 51398

- posted by: [jmadlena](https://stackexchange.com/users/-1/28290-jmadlena) on 2013-10-15
- score: 2

<p>Stripe Connect is your answer. I'm doing the exact same thing. With Stripe you can accept credits card directly on your site. Create various plans (charge $8 every month). Subscribe people to those plans, and take a percentage or dollar amount for each subscription.</p>

<p>It's an amazing service, with a reasonable 2.9% + $0.30 per charge fee.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
