## Bookkeeping practices for a website using electronic payments (e.g. Paypal)

- posted by: [morpheous](https://stackexchange.com/users/-1/14583-morpheous) on 2011-12-08
- tagged: `payments`, `ecommerce`, `accounting`, `bookkeeping`
- score: 1

I am in the process of setting up an accounting "system" (well set of procedures etc). For most businesses, the books of original entry include:

- Sales Day Book
- Sales Return Day Book

As I understand it, these day books are required in order to keep track of which customer owes money etc. In other words, they are only relevant if you offer credit terms to your customers. In the case of my website (selling fairly low ticket items), no credit terms are offered, and the customer pays for the product there and then, using paypal to transfer funds to my Paypal account.

I will then periodically (say end of the day) check if there have been any transactions for the day, and transfer the funds to my bank account (incidentally, is there a way to automate this, or does it have to be done manually?).

My main questions then is:

Do I still need to create a Sales day book or do I simply enter the transfered amount(s) into my Cash book?

I can see a side benefit of having sales day book and personal ledgers as it would help me keep track of the individual customer spending patterns etc.

Suppose I have the following transactions:

    Date        Customer     Description    Quantity  Amount
    2011-12-1   A. Other     Product 1      4         $120
    2011-12-2   I. Someone   Product 2      1         $30
    2011-12-4   N.O. Body    Product 5      1         $10

Which day books (journals) and nominal ledgers will I record these sales - and Paypal fees into. For the sake of simplicity, lets assume Paypal fees are $1 fixed per transation.



## Answer 35086

- posted by: [Michael](https://stackexchange.com/users/-1/15880-michael) on 2012-01-22
- score: 1

For simple Book-keeping purpose, 

Create - Paypal Account under Bank category. Then you record your daily, weekly , monthly or quartely as your choice in there. Do not post individual transaction but use summary of your desire frequency. 

**1) When you record your sales from paypal**

 - Debit - Paypal Account 
 - Credit - Sales

**2) When you record your paypal charges**

 - Debit - Bank charges 
 - Credit - Paypal Account

**3) Whenever you transfer money from paypal to business account,** 

 - Credit - Paypal Account
 - Debit  - Suspense or Transfer account 

(You need this intermedia account to trace your transfer since paypal takes few days to reach money in to the account and thus the date of transfer and money received in the account will differ).


**4) When you record bank transactions for the paypal transfer;**

 - Debit - Bank
 - Credit - Suspense / Transfer Account.


-----

Since customers are paying you straight away, nominal ledger is waste of time. But if you have debtors then they will useful to track who are outstanding.

Sales account can be use as sales daybook. 

Please remember to keep all the records. Download paypal transactions as CSV format which is the best format for reconcilaiton. 

----
Book-keeping Notes 

 - Debit - Increase (+)
 - Credit - Decrease  (-)


## Answer 33708

- posted by: [Vasiliy](https://stackexchange.com/users/-1/14038-vasiliy) on 2011-12-14
- score: 0

I couldn't find an answer to this question, so I will start with it: Do you have a set (limited) number of customers who pay you multiple times or do you have a new customer each time a payment is made?

In the first case (same customers) you may want to keep track of sales for each customer in your records, mostly for tracking purposes. However, I would assume the limited number of customers in your situation is not the case. So, to the second option.

If you have a lot of new customers and they pay you via PayPal, you probably don't need to track each payment individually. What I do (a lot of customers because every payment is basically a new customer) is sum up total payments from customers for a month and record that as my sales. I don't use paper, I use QuickBooks, so the entry will be to increase cash and increase revenues. I then record PayPal fees as a deduction from sales and cash, but PayPal fees are recorded in an account different from sales: increase PayPal fees/expense and decrease cash. This way I know how much gross revenue I earned and how much I spent on PayPal fees. The difference is my net cash inflow.

I am not sure why you will need to create daily sales books. One option I see why you may need that is if you need to collect sales taxes (USA). However, in either case PayPal has nice reports on their website for merchants which will show you sales, returns, etc. by day for a month. You can just download that report every month and use it for your records.

Also, not sure about the need to transfer cash from PayPal to your bank account daily. Why not just do that at the end of a month?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
