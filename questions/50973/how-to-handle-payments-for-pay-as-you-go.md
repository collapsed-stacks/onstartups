## How to handle payments for pay-as-you-go?

- posted by: [steve](https://stackexchange.com/users/-1/27226-steve) on 2013-09-16
- tagged: `payments`, `customers`, `risk`
- score: 1

My startup is a marketplace for compute time (a crowd-sourced alternative to Amazon EC2/Web Services), where buyers can rent computer time via the internet by the hour.

Ideally I'd like to aggregate the billing amounts at the end of month, because:

 - It reduces the payment processing fees (PayPal to start with) considerably
 - It simplifies the billing process

Is there any way to mitigate the risk that the buyer disappears, and I never get paid?

e.g. Is it acceptable/possible to ask for a deposit up-front? If so, how would I return any unused balance? (e.g. would I have to pay additional fees to the payments provider to refund any unused amount)?

Are there any other ways to handle this?

[EDIT - I should clarify that I'm based outside the US, so a US-specific product/service is unlikely to be applicable to firms like mine]


## Answer 50994

- posted by: [Adam C](https://stackexchange.com/users/-1/27921-adam-c) on 2013-09-17
- score: 1

<p>With PayPal, I don't think its possible to charge customers automatically at the end of the month. It will require the customer to make the payment, this means you will have to get into the business of chasing invoices for payments if they don't pay. You should factor this into your cost vs getting some form of payment up front. </p>

<p>I've been trying for a long time to get a continuous authority merchant account which might be a solution for you but I'm not sure (I will charge a minimum monthly fee + any extra usage). The requirements for this are complex and the paperwork is heavy.</p>

<p>If I was in your situation, I would swallow the extra charges and charge people upfront a small amount for a number of hours (£10, for 10 hours example) and then have them top it up when required. This would provide you an opportunity to give people intensives and extra's (£10 gets you 15 hours rather than the normal 10 etc). </p>

<p>For returning money, on PayPal, if you perform a partial refund, the transaction fee is recalculated and adjusted to the amount of money not refunded. So if you refund 30% of the charge, PayPal will adjust the transaction based on the remaining 70% of the balance. If you refund after 60 days however, nothing is credited. </p>

<blockquote>
  <p>If you issue a refund within 60 days, PayPal credits the original
  transaction fee for receiving the payment to your account. For partial
  refunds, PayPal credits a percentage of the original transaction fee
  based on the refunded amount. When you issue a refund after 60 days,
  your original transaction fee for receiving the payment is not
  credited to your account.</p>
</blockquote>

<p><a href="https://cms.paypal.com/uk/cgi-bin/?cmd=_render-content&amp;content_ID=developer/howto_admin_refunds" rel="nofollow">Details here</a> </p>

<p>Once you have proof and accounts to show you have a working business model, the banks are more willing to provide more flexible billing services but until then the options are pretty limited based on my experience. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
