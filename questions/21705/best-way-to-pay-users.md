## Best way to pay users

- posted by: [nami](https://stackexchange.com/users/-1/8684-nami) on 2011-03-16
- tagged: `payments`, `ecommerce`, `finance`
- score: 2

Lets say I make the next google ads service (hypothetically speaking), how can I pay my users in more or less real time? with minimal or no additional cost to the company.


## Answer 21707

- posted by: [Brian Karas](https://stackexchange.com/users/-1/8465-brian-karas) on 2011-03-16
- score: 2

You can't.  Not both in real-time and for (near) free.

Distributing payments always has a cost.  This is part of the reason why micropayments still aren't doing much (the processing costs as much as the payment) and why there is a billion dollar merchant services industry.




## Answer 21708

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-03-16
- score: 2

The most common approach is for you to keep account of your users earnings in a DB.  Once those amounts are high enough, then you could do a Paypal to Paypal transfer.  This can be done via API, and costs you very little, (just a transaction amount).

For countries where they cannot "withdraw to local bank" then your options are payment debit cards such as payoneer. 

If your users are just in the US, then I would avoid payoneer because their rates are expensive.  in that Scenario you could still offer debit card payments.  I think the pricing is $5 per card, flat (thats the best i have found).  You still would have an expense of loading the cards, this is done through ACH, and costs again only for the transaction amount.

Make sure that you require 1099 from those getting paid. 




## Answer 21754

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-03-17
- score: 1

I think fees will be the least of your worries. Fraud is what will cost you. If you pay in real time, fraudsters will work you over before you realize you have been taken. A grace period gives you a little time to weed out the ne'er-do-wells.


## Answer 21744

- posted by: [Mat Banik](https://stackexchange.com/users/-1/6605-mat-banik) on 2011-03-17
- score: 0

<p>The lowest fees are for ACH (Automated Clearing House) credit (meaning from your biz account to clients account) transactions. Also you can have service where the payment processing company will tear paper checks for your for monthly fee. </p>

<p><strong><a href="https://www.paymentsgateway.net/" rel="nofollow">paymentsgateway.net</a></strong> - is one of the ACH credit processors. Check out their fees page.</p>

<p><strong>Amazon Payments</strong> allows sending money but not via API yet. They have a lot lower fees than PayPal.</p>

<p>BTW, you would need to hire developer to integrate API for the ACH on your site.
Also PayPals new Adaptive API allows for specification of who will pay the fees. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
