## Peer to peer marketplace payments

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-06
- tagged: `payments`, `market`, `credit-cards`, `bank`
- score: 2

I am in the process of setting up a peer to peer marketplace.  I would like to allow buyers to pay directly with credit card, and sellers to receive batch payments into their checking account directly without the use of a third party application.  I know I can use services such as paypal and I understand the advantages but for this project I would rather have payments go directly through by service.  Does anyone have any experience or advice on what I will need to setup.  From my understanding, I will need a payment gateway and merchant account.

Also, does anyone know anything about factoring?  How do marketplaces avoid factoring when applying a peer to peer marketplace?  Thanks


## Answer 13843

- posted by: [abenetis](https://stackexchange.com/users/-1/3397-abenetis) on 2010-09-02
- score: 3

From a Programming View this sounds complicated. However, as you like to use a Merchant Account and a Payment Gateway, you need to review the abilities they have and what they allow you to do. 

If you are allowed to make batch payments to the suppliers from your Merchant Account, you need to setup a Database which handles all Buyer and Seller Transaction Data to perform the Batch Payments.

Keep an eye on Security, if you have to handle Payment Transaction Data like Bank Account Numbers or Credit Cards Numbers. Better you don't need to handle them as this kind of Data needs superior Security, but you may have access to them through your Merchant Account.

Your System must be able to handle the Payment Status correctly, so if a payment is pending from the View of your Merchant Account Provider, you will not pass it through to the Seller until it turns to have the Status "settled" or what ever Status make it finally balance it into your Account.

Don't bother with Factoring, as you don't want to have the risks for not getting payments from either of the invloved parties of a transaction. If it is possible for you the Setup the aforesaid System, you don't need to bother with Factoring anyway.

Most importantly your System and your behavior must show that you and your System are trustworthy. This means, passing payments correctly and so on. If you fail to proof this, you might not get another chance with this kind of service.



## Answer 26040

- posted by: [Alex Cook](https://stackexchange.com/users/-1/6128-alex-cook) on 2011-06-08
- score: 1

I have no experiencing working with this company, but I stumbled upon it the other day: https://poundpay.com.

I'm also building a marketplace, and here's how we are doing it, roughly. Something like the above service might be good for an MVP, but we're beyond that point and have experience w/ payment gateways so we're doing it in house.

**Setup accounts**

 - Create a merchant account to accept credit card payments (there's a start-up out there I can't remember the name of that helps you find merchant account rates)
 - Create a separate ACH account through a company like http://www.paysimple.com (they might allow you setup both accounts through them).

**Here's a sample transaction:**

 1. Seller lists item for $100
 2. Buyer purchases item for $100 using Visa card
 3. Your merchant account processes the $100 payment.  Customer sees "Your Startup" on their credit card statement.
 4. After fees, you have $95 in your checking account.  It takes a few days for the amount to be deposited.
 5. You initiate an ACH transfer to the seller.  The funds are withdrawn from your checking account and direct deposited to the seller's account.  Typically the fee is a flat rate for ACH transfers (e.g. $0.55).

In the end, you process $100 and pay out $5.00+$0.55 to make it all happen.

**Additional considerations**

 1. When you use your merchant account, you're liable for chargebacks.
 2. When it comes to payments, there's a grey area on whether or not you need to become "pci compliant" (pay a 3rd party company to review your code/server setup to make sure it's secure).
 3. All of the events take time to process.  It's not instant.
 4. With ACH, depending on if you're withdrawing/depositing, you need to get the sellers to sign an ACH authorization form.  Depending on your number of sellers and the way you setup your flow, this isn't a huge deal.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
