## Sending money to users

- posted by: [Codebeef](https://stackexchange.com/users/-1/1594-codebeef) on 2010-03-26
- tagged: `accounting`, `payments`, `legal`
- score: 3

I'm considering building a system that allows our users to purchase points, trade them between themselves, then cash them in for real currency.

The system will work like this:

* User A buys points - say 100 for £10
* User A buys something from User B for 50 points
* When UserB accumulates >= 100 points, they can sell them back at a rate of £9 / 100

For now, I'm thinking of using PayPal to facilitate the process, but I'm unsure as to the accounting and legal issues I need to take care of. Does anyone have any specific advice or pointers to the areas I need to cover?

We're based in the UK.

Cheers!


## Answer 9627

- posted by: [Greg Belote](https://stackexchange.com/users/-1/837-greg-belote) on 2010-03-27
- score: 1

I toyed with an idea for an IOU management system a while back, that allowed you to pay friends with a credit card later. Here are a few of the ways we brainstormed getting money back to users:

- **PayPal**. Expensive charges, they take a lot off the top but they're easy and familiar.
- **Gift cards**. Seems like you should be able to buy Amazon gift cards and email them to your users. Instant and there may not be any transaction fees, but not as flexible as cash money.
- **Mailing checks to users**. Send them a check in the mail. It's not fast or super-easy, but OK for some users and the only transaction fee is the postage and someone's time.
- **Mailing checks to the user's bank**. Some banks allow money transfers this way. It's non-instant and requires you knowing the bank address (and maybe account number?) but cheap and simple.


## Answer 9661

- posted by: [Joe](https://stackexchange.com/users/-1/1572-joe) on 2010-03-28
- score: 1

<p>On the points -> money side, credit card companies offer something called a <a href="http://en.wikipedia.org/wiki/Stored-value_card" rel="nofollow">stored value card</a>.  It's sort of like a debit card backed by a small account.  At a previous company, we used these to pay customers an incentive bonus.</p>

<p>Worked great; we used a fulfillment company, who took care of everything.  Just upload an order file to them periodically and they would send the cards, handle returns, etc.</p>

<p>On average, people don't use the full value of the card.  So they end up costing you somewhat less than face value.  For people who do use the card, it's very convenient -- accepted anyplace that accepts Visa/Mastercard.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
