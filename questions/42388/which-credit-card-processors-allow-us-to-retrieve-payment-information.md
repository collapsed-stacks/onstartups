## Which Credit card processors allow us to retrieve payment information?

- posted by: [simplyme](https://stackexchange.com/users/-1/11458-simplyme) on 2012-10-03
- tagged: `payments`, `credit-cards`
- score: 1

Which credit card processor allow us to retrieve payment information from their server in case if we need the payment information?

I believe my question isn't clear enough and I decided to write a detailed scenario.

We are building a new web project which allow hostel owner to list their hostel at our website.
We will charge 10% as a deposit for the booking and if the guest doesn't show up, the hostel owner can look at the guest's credit card information (login into their control panel from backend) to charge the credit card with their own credit card terminal.

So now I am looking for a credit card payment processor which allow us to charge the 10% deposit, store the credit card information on their server and in case of no-show, we can retrieve the credit card information which the hostel owner will need it to charge for the no show fee.

Thank guys. Any answer is much appreciated 


## Answer 42402

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-10-03
- score: 2

Payment processors (at least for credit cards) are **prohibited** from giving you more information than you supplied to them. You may be able to retrieve the information you supplied to them, but nothing additional. The only extra information you can get from them is a code that may **or may not** indicate the billing address or security code you supplied was incorrect. These reference codes tend to be unreliable.

Our merchant account does **not** allow you to see the expiration date, CVS, or complete credit card number for settled batches. 


## Answer 42404

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2012-10-03
- score: 0

If I understand your question correctly, here is what I suggest:

1. If you need to re-use credit card information to bill customer for additional products and/or services, 1st you need permission to retain such information. You have to ask and have verifiable YES from them. All it takes is one or two of your customers getting pissed off and complaining. You will lose your merchant account and can get blacklisted.
2. Authorize.net (which is used by huge number of processors) has a feature where this information can be retained for recurring charges. I've looked at it and at the time it was cheaper for me to retain that info (encrypted) in my CRM, but I had to put in place a lot of processes to make sure I am PCI compliant. Not doing so will result in loss of merchant account and possibly getting blacklisted.

Whatever you do, do not cut corners! I had to deal with cancelled merchant account before - it is not fun, it is really painful, and not worth the shortcuts.


## Answer 42440

- posted by: [Randy E](https://stackexchange.com/users/-1/19553-randy-e) on 2012-10-05
- score: 0

Why aren't you taking the entire payment upfront? Most booking services I've used require 100% payment upfront. 

One thing you need to keep in mind, if you keep sending noshows to hostels, they're going to stop listing on your site.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
