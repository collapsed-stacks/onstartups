## What's the best way to deal with a proforma invoice?

- posted by: [Tim Long](https://stackexchange.com/users/-1/11009-tim-long) on 2012-12-07
- tagged: `accounting`, `business-process`, `invoice`
- score: 0

I have a supplier that sends me invoices in advance, with so many days to pay. I want to enter these invoices into my accounting software as soon as they arrive, so I know what my commitment is for the upcoming month. When I pay the invoice (online) the invoice number changes, so it no longer matches what I have in my accounting software.

I found this very confusing and difficult to deal with. I asked the company about it and they said that the unpaid invoice was a 'proforma' and when it gets paid, then it becomes an invoice and the number changes, because its a new document.

To my mind, that's an odd way of doing things - but they are unlikely to change it and I need to work out how best to deal with it.

I use Office Accounting 2009 - which is actually a really nice bit of software but regrettably no longer available. OA doesn't support proforma invoices directly. If I wanted to issue a proforma myself, then I would create it as a sales order, then print it out using the proforma template - but internally it is a sales order document.

But I'm not issuing the proforma, I'm receiving it. Inferring from the reverse process, it seems likely that one way to model this would be to enter a purchase order to represent the received proforma, then convert it to an invoice when the bill is paid. Unfortunately that then means there has to be an intermediate step of a Goods Received Note (GRN) which is wierd (there are no goods, its a service) and it makes the whole process very tedious.

So, lets get to the questions.

 1. What is the validity of what this supplier is doing? Is it normal to issue a proforma? Why wouldn't they just issue an invoice.

 2. How would you deal with this situation in your own books or accounting software?

Thanks.


## Answer 44856

- posted by: [mojsilo](https://stackexchange.com/users/-1/1826-mojsilo) on 2012-12-07
- score: 1

 1. Yes it is normal. In many countries if you issue an invoice you must pay tax on it (VAT etc) even if client never pays. That can be quite a problem in cash flow as you can imagine. That's why they issue a pro-forma invoice so you know what to pay and once you pay, they convert that pro-forma document into an invoice. Totally legit.
 2. In your accounting program you might have an option to create an invoice from a supplier where you can mark it as pro-forma or not verified but still be able to see the due date or you can create separate entries for payments and connect it with invoice when you get it etc. It's easier if your supplier have an Origin field on their invoice where they will put the document number of the document that this invoice originated from (pro-forma). It sucks, but it is what it is.


## Answer 44888

- posted by: [LLM](https://stackexchange.com/users/-1/21992-llm) on 2012-12-09
- score: 1

Pro-forma invoice from an abroad company is akin to a sales estimate here in the United States.  Given that it sounds as though your vendor won't issue you an actual invoice - and if you are on accrual accounting, and if you plan on paying an invoice in X days, then just book the pro-forma invoice in to your accounts payable when you receive it.  Then pay it later, as you normally would.  This will cause the expense to be booked on your income statement and the accounts payable on your balance sheet to increase.  When you pay, the accounts payable will reduce and your cash will reduce.  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
