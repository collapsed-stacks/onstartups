## Should I give a discount when people pay with credit card

- posted by: [Philippe](https://stackexchange.com/users/-1/6113-philippe) on 2011-02-16
- tagged: `payments`, `credit-cards`
- score: 8

I have a software product (price around 700 USD). Some customers use PayPal, which is very low-touch and easy for us. Others want to do the whole procedure: RFQ / price quote / PO / invoice / wire transfer. Larger companies sometimes delay the payment for up to three months! Obviously PayPal is easy, POs are more troublesome. 

I have noticed that some companies accept *only* credit cards (like 37signals).

My questions: should I give a discount to incentivese people to use PayPal? What are the pro/cons of doing so? Do you have examples of other on-line companies that do this?
Could I get away with offering only PayPal (credit card) orders for the base product and offering PO processing for a premium version?


## Answer 20311

- posted by: [tbaums](https://stackexchange.com/users/-1/7624-tbaums) on 2011-02-16
- score: 12

Why not offer standard trade terms to your larger clients? 

The industry standard for physical goods is 2/10  net 30 (read: two ten net thirty). 

The way this works is that the buyer receives a 2% discount if the payment is made within ten days, but if the buyer declines to pay within 10 days, all of the payment must be made within 30 days.

The reason buyers almost always make payment within 10 days relates to the annualized interest rate of failing to do so. If the interest rate for (essentially) an extra 20 days of waiting is ~2%, then the annualized rate is huge (for a 360 day year...)! 

CFOs of purchasing companies pay hard attention to that. 

More on this from Wikipedia: http://en.wikipedia.org/wiki/Discounts_and_allowances

And in comparison to the amount that CCs charge, this is a reasonable discount to offer if payment will be made with a check or bank transfer.


## Answer 20317

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-02-16
- score: 10

While the cost of a PayPal transaction may **appear** to be low to your firm, you are also taking a **risk** on each PayPal transaction. The PayPal transaction might cost 1.5% - 2% of the total transaction in fees, but you also risk losing the entire $700 in a charge back. You need to consider that in your calculations!

In addition, many businesses do not have PayPal accounts, or have a negative image of PayPal, and thus will not use it to purchase. **Many** businesses only purchase things by Purchase Order. If you sell to businesses you typically have to accept Purchase Orders.

Note however, that it is **you** who set the terms for Purchase Order acceptance. Never let the purchasing department bully you. You are **loaning** them money and you set the terms of that loan. We have **never** lost a sale by telling the people sending out the POs that their terms were unacceptable.

**Rule 1:** Your terms should be net 30. Never accept any PO with terms longer than that.

**Rule 2:** Charge money to accept a PO. It costs you money to bill them, so make them pay for the privilege. (We charge an additional $10 for every PO, on top of normal shipping.)

**Rule 3:** Your web site needs to clearly state your PO terms and mention that changes to these terms can occur at any time. Our site specifies that if the PO is unpaid after 45 days, their software license will be terminated, the software will be deactivated, and re-activation costs an additional $150.00. We report all license terminations to the Software Business Alliance piracy site, and D&B.

**Rule 4:** Charge a major penalty for late payment. (We charge $25 per $100 of PO value for late payment and the penalty increases with each late notice.)

**Rule 5:** Never let purchase orders go untended- check all your unpaid po's at least once a week. Use standard form letters to send out a late notice at 30 days (with penalty fee), and a termination notice at 45 days (with more fees).

**Rule 6:** At 60 days, turn the whole thing over to a collection agency. You lose 18% - 25% but it rarely if ever comes to this point if you follow the rules above AND once you turn it over, your work is done. The collection agency duns the firm until they get the money or they go to court. When they go to court they always win. (And you pay no extra fees if it goes to court.)

**Rule 7:** Never accept partial payment for a PO. If you charged them a late fee and they finally paid just the original amount at 45 days- send the check back. Tell them to FedEx a check for the full amount, or lose the software.

If these rules seem to Draconian, remember they don't apply to anyone who pays on time. (Except for charging them for using a PO, which is **normal**).

Always remember, you are not dealing with the person using your software. You are dealing with a department whose whole purpose is to delay payment to those firms that let them get away with it. You are not a bank, offering unsecured loans.

**Finally**, your web site should be set up to supply offical price quotes for you product. That eliminates that problem.


## Answer 20377

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-17
- score: 0

you should keep all the ways to pay for your product. I mean the buyers should be able to pay with or without paypal because paypal is not supported to all over the world. There are many countries where paypal does not exist. If you give only one payment option by paypal then you may loose some buyers.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
