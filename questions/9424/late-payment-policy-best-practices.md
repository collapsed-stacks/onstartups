## Late payment policy / best practices

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2010-03-20
- tagged: `payments`, `cash-flow`
- score: 7

I am considering instituting a formal late payment policy for our product.  Our terms have always been net 30 but it is something that we never consistently enforced.  As the company grows and matures, I think it is important to have a policy in place in order to treat all customers fairly and encourage prompt payment (which helps with cash flow).  

We sell B-to-B SaaS and all of our payments are currently received either via check, wire or ACH.  The bill varies month-to-month depending on usage / consulting fees somewhere between $600-$8000 dollars per customer.  

Here some options being considered:

1. Offer a discount for early or on-time payment.  
2. Introduce recurring credit card billing so that the customer is charged automatically each month.
3. Gracefully degrade the software as the customer gets late on payment.  For example.  (e.g. no administrative privileges or read-only mode after 45 days late payment).
4. Require an upfront deposit from customers that consistently pay late.
5. Charge late fees and/or interest on the outstanding balance.

Up until now I have avoided taking credit cards and PayPal due to the high fees these transactions entail.  I understand the tradeoff in terms of credit card cost vs our time cost to chase customers for payment but most pay on time and don't mind sending a check or wire.  The processing fees would be 3-5% of our gross revenue for 
every transaction ($18-$240 per payment per customer).   Likewise, to give a discount 
for early payment would mean at least another 5% off our current gross (another $30-$400 
per payment per customer).  We would almost certainly need to raise prices -- a tough
proposition in these times.  

Are there any other options I should consider?  What kind of late payment policies have you found work well for your business?  How do you handle customers that are consistently late?  How about delinquent customers?  At what point do you shut off the customer for non-payment and how long do you retain his data?



## Answer 9425

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-03-20
- score: 8

First, you need a formal written payment policy. Without that policy you have no legal options to enforce payment.

I can not figure out what the problem is with options 1) or 2) above. Acepting credit cards will cost you a minor amount of each transaction, but increase your cash flow and remove the entire process of chasing your customer down for payment. You build this percentage of "loss" into your product cost. Autobilling their credit card greatly simplifies your life! That is what we do for all our services. And if the customer's card is declined we have a frmal policy to follo. No payment in 15 days shuts off their account.

Billing your customers for money and chasing them down costs you just as much money as a credit card takes in percentage.

If you are billing a customer for payment by check this is essentially a purchase order. You should be asking the customer for a PO and specifying the terms for that PO. Purchase Orders are legal contracts in the US and can be bought or sold! Here are some standard terms we use for purchase orders.

 1. The smallest purchase order amount we can accept is $100.
 2. All purchase orders need to include contact information for a person at your organization. This contact information should include a person's name, phone number, and email address.
 3. There is a minimum $10.00 shipping and handling charge for processing a purchase order. This fee applies even for orders which specify electronic delivery. Additional charges and fees may apply based on your requirements.
 4. All products bought by purchase order must be shipped to a US destination.
 5. Payment terms are net 30. We do not accept POs with terms longer than this. All late payments on purchase orders are subject to a $25.00 per hundred dollars of value late fee.
 6. If payment is not received within 45 days, your license to use our software will be canceled. The fee to re-instate a software license, once canceled, is $150 per product.
 7. We can not accept purchase order numbers over the phone, or purchase requisition forms.
 8. We can not accept purchase orders from outside the United States. All international orders must be prepaid.
 9. We do not accept partial payment of purchase orders. An invoice, including all late fees and penalties, must be paid in full or your partial payment will be refused.
 10. By submitting a purchase order to us, you agree to meet all the terms listed here.
 11. The terms and conditions under which we accept purchase orders are subject to change without notice.



## Answer 9452

- posted by: [Traci D. Ellis](https://stackexchange.com/users/-1/2889-traci-d-ellis) on 2010-03-21
- score: 4

You've gotten some great advice here.  Gary's advice is right on target. As a business law attorney, I would only add the following suggestion:

Once your policy is in writing and has been communicated to the customer in your click wrap agreement, or however you communicate it, prior to automatically shutting off service, have a pop up advise them in advance (3-5 days) that service will be terminated/downgraded on [insert date] unless payment is received.

This type of last "grace period" warning goes a long way with judges in case you ever sue a client for collection.


## Answer 9429

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2010-03-21
- score: 2

1. $600-$8000 is the amount that can go on credit cards. $18-$240 should be a no-brain. If the monthly fee is large enough, have them pay for the first month to three months via credit card and then move them to the pre-pay via check. Bill them 30-days prior and turn them off 5 days after their overdue.
2. Quarterly, 6-month, 1-year, and longer terms should have a discount. Max discount we have given on 1 year of SaaS was 10%.
3. Net30 is something you EARN as a good customer. The only exceptions are publicly traded companies and even in that case you can get paid earlier.
4. I love SaaS business model, because you can pop up messages to the right people to aid the AR. But even when we dealt with the government (school districts, in our case) they could send any POs they wanted, unless there was a check, there was no service.
5. I am willing to bet your customers would prefer to pay via credit card. Easier to put it on the expense report than get a bill into accounting, get check issued, etc.
6. I always like instituting the "you sold it, you will have to collect it" policy. Keeps certain problem sales folks from selling to the wrong customers. It is amazing what happens to receivables, when the sales person has to call the customer after they are 14 days overdue.

That is at least what I like to do when I head business ops for companies or consult them on the best practices. 




## Answer 9433

- posted by: [tcolling](https://stackexchange.com/users/-1/2813-tcolling) on 2010-03-21
- score: 2

At my company, we provide a low-tech non-medical in-home caregiving service for Seniors.

We require a deposit in advance of service that is equal to one week's fees.  We hold that deposit until service ends and then we apply it back to the account as a refundable credit.  

We require that deposit even if the client is going to pay by credit card.

Requiring a deposit works for us because we bill weekly and the deposit amount is relatively small compared to the cost of service per month.  

We have to bill weekly for service from a cash flow standpoint because here in the People's Republik of Kalifornia we have to pay our caregivers weekly.  

People can decide to pay a deposit or they can go elsewhere to another company.  We hold the line on that because we have found that a prospective client's refusal to pay a deposit is a foreshadowing of collection problems down the road.  Most top-shelf companies in our industry require deposits.

If your SaaS service is a B2B product, it may be able to switch to a credit card approach if the clients are primarily small businesses.  If the clients are primarily large companies, I speculate that the clients will not want to use a credit card for payment.

Why not just bill in advance for your services, say, a month in advance?  That way, you're always working off what is basically a deposit.






## Answer 9455

- posted by: [Joe](https://stackexchange.com/users/-1/1081-joe) on 2010-03-22
- score: 1

Another perspective on the usage of credit cards.  Don't forget that aside from the benefits listed above, it does make things easier for the customer as well.  In my old company, the owner could slap down his CC for purchases and pay instantly.  If it required check or bank transfer, it had to go through Accounts Payable department first making it more difficult and time consuming.  Credit card will likely save them time and money, making them more likely to make purchases frequently.   


## Answer 20774

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-25
- score: 0

Acepting credit cards will cost you a minor amount of each transaction, but increase your cash flow and remove the entire process of chasing your customer down for payment.
<a href="http://www.au-laptop-battery.com/"laptop battery</a>



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
