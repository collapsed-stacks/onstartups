## Upgrades, Downgrades and Cancellations in Paypal recurring service

- posted by: [user3462](https://stackexchange.com/users/-1/3462-user3462) on 2011-01-14
- tagged: `subscriptions`, `payments`
- score: 5

I plan on using Paypal for a monthly subscription service and would like to know how to handle the Upgrade/Downgrade/Cancellation from users:

1. For cancellation, is it recommended to develop the site such that the cancellation is forwarded to an admin who manually cancels the service?
2. For upgrades, I'd think that the user will be happier if the upgrade happens instantaneously instead of waiting for an approval from an admin.

How do I handle these use cases? Thanks!


## Answer 19030

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-01-15
- score: 2

<p>The answer to this question is almost the same as <a href="http://answers.onstartups.com/questions/18948/how-to-let-customers-download-software-automatically-after-payment-through-a-webs/18966#18966">my answer to the "How to let customers download software automatically after payment through a website?" question</a>. Namely, you should use <a href="https://www.paypal.com/ipn" rel="nofollow"><strong>PayPal IPN</strong></a>. Specifically, see the <a href="https://www.paypal.com/cgi-bin/webscr?cmd=p/acc/ipn-subscriptions-outside" rel="nofollow">"subscr_cancel", "subscr_modify", and "subscr_eot"</a> "txn_type" values coming from IPN.</p>

<blockquote>
  <p>For cancellation, is it recommended to develop the site such that the cancellation is forwarded to an admin who manually cancels the service?</p>
</blockquote>

<p>If a user cancels they should be immediately downgraded or removed by your system (or however you handle cancellation). You could always do this manually, but why would you? If you receive a "subscr_cancel" from PayPal's IPN you can use a bit of code to cancel their account.</p>

<blockquote>
  <p>For upgrades, I'd think that the user will be happier if the upgrade happens instantaneously instead of waiting for an approval from an admin.</p>
</blockquote>

<p>Yep. In this case use the "subscr_modify" transaction type from PayPal IPN.</p>



## Answer 19795

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-02-04
- score: 2

Worth mentioning PayPal have lots of options:

PayPal Standard Payments, which is what most people consider "PayPal" has a very basic subscription system, where either party can cancel the subscription but neither party can modify it. Also it is quite complicated to programmatically cancel the Subscription.

PayPal Express checkout is similar to above but has some basic API allowing software to automatically cancel payments for example. 

PayPal Adaptive Payments which is a newer set of APIs allows PreApproval billing this is probably PayPal most flexible system, it will allow you to specify dates/periods to bill and users can be asked to accept new billing agreements etc.

Finally their is PayPal pro which is much more akin to a normal payment gateway. 

Which one you choose to use has a massive difference to what you can and can't do, obviously the more flexibility of Adaptive for example comes at the cost of requiring a developer to help implement it correctly. For more information (especially if you are a developer check out x.com its PayPal developer network) as it's not just a case of listening to an IPN as has been suggested, at least not if you want to trigger the IPN in the first place.


## Answer 19233

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-01-21
- score: 0

<p>You may want to consider using a service like <a href="http://blog.recurly.com/2010/08/top-ten-reasons-to-use-recurly-vs-paypal-for-recurring-billing/" rel="nofollow">recurly.com</a> (they have a good explanation of Recurly vs. using the Paypal API at that link), cheddargetter.com, chargify.com, or spreedly.com.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
