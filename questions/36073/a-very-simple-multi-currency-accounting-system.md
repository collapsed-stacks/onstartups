## A very simple multi-currency accounting system

- posted by: [lukeshek](https://stackexchange.com/users/-1/16193-lukeshek) on 2012-02-12
- tagged: `uk`, `ltd`, `accounting-method`, `currency`
- score: 3

I run a small limited company in the UK which requires very simple bookkeeping.

The company sales online services (internet apps) and the only costs the company have are:

- domain and hosting,
- transaction fees,
- director’s salary paid monthly.

I work from home and I made myself all the apps the company sales.
I keep a simple cash book and record every transaction.

![enter image description here][1]

However, the company operates all over the Europe and accepts payments in Euros and Zlotys.

In this example, let’s say all payments were taken in Zlotys (PLN).

![enter image description here][2]

As you can see from the table, the company had two customers and earned 100 PLN in total.

According to the law, all the received amounts must be converted into pounds (GBP).
I made a few simple changes to the cash book:

![enter image description here][3]

From this table you know that on my bank account there should be two transactions of 50 PLN each.

And now let’s say that 2012-02-12 is the last day of my accounting year.

I have 100 PLN at my disposal (on the bank account), which should equal to 19.59 GBP.
However, over the year the pound fluctuated and 100PLN is today worth 19.80 GBP.

This way the company earned 21 pence.

I have another cash book in which I record other incomes (for example bank interests).

![enter image description here][4]

And now the basic question – do I do it right?

Is this form acceptable?

How often should I record profits and losses if the currency fluctuates?

Should I do it every time the exchange rate changes or on the last day of my accounting year? (I would opt for the first one.)

Should I have one book for both sales in pounds and zlotys or keep the sales in separate books?

To anticipate your suggestions - yes, I'm going to contant an accountant, but first I would like to get the basics and make sure I understand what I'm doing.

In the meantime, I created another table.

![enter image description here][5]

This table shows transactions in both pounds and zlotys.
There is also a total amount received in GBP and ammout of assets in PLN.
Do you think this is clear to understand? I'm not sure whether this could look like if I had 29GBP and 100PLN on top of that. If so, how can I improve the table?

  [1]: http://i.stack.imgur.com/lFP6E.png
  [2]: http://i.stack.imgur.com/frqkN.png
  [3]: http://i.stack.imgur.com/k4wPo.png
  [4]: http://i.stack.imgur.com/RMqIb.png
  [5]: http://i.stack.imgur.com/oItue.png


## Answer 38626

- posted by: [Brad](https://stackexchange.com/users/-1/17731-brad) on 2012-04-29
- score: 1

If you maintain cash accounts in several currencies, you should maintain financial statements (P&L, BS, Cash flow statements, etc) in each currency.

As and when you undertake an FX transaction to move cash from one currency to another, at that point you should update each set of accounts accordingly, applying the FX rate at the time the transaction was made. This can be done as frequently or as rarely as you determine.

This approach gives you the mechanism of measuring P&L from a particular jurisdiction in the currency of that jurisdiction, and thus obviates the need for you to do anything specific in respect of FX risk at this level. 

However, the FX risk must still be managed. You should consider a separate mechanism for doing this, perhaps by converting your PLN P&L to GBP on a periodic basis (say monthly). This can become a complicated endeavour quite quickly, especially if you are sitting on large amounts of currency from different jurisdictions. In this case, it becomes a management (treasury) decision as to how frequently you undertake FX transactions to move money to your base reporting currency. This decision will need to be driven by your capital requirements in each region -- for example, do you need to pay Poles in PLN, if so, leave some PLN in place for that. 

If the FX risk gets severe, you may even need to consider hedging mechanisms (FX futures or options) to manage that risk.

You should of course bear in mind that FX rates change continually on a 24x7 basis, and not at discrete periods. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
