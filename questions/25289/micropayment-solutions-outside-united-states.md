## Micropayment solutions outside United States?

- posted by: [Raymond Ho](https://stackexchange.com/users/-1/10685-raymond-ho) on 2011-05-22
- tagged: `payments`, `shopping-cart`, `micro-payment`
- score: 5

I have a small project that sells legal music online, per transaction is less than a dollar so the traditional payment solutions are not my option because they charge too much fee.
I found out that [Paypal][1] have a Micropayment solution but it is only available for US companies. Then I checked [Amazon][2], they also have a flexible payment solution, but it is also only available for organizations in United States.
So I got no option left, I need to have a payment solution that accepts business that are outside United States(I'm in Philippines), and charge low fees for microtransactions.


  [1]: https://www.paypalobjects.com/IntegrationCenter/ic_micropayments.html
  [2]: https://payments.amazon.com/sdui/sdui/business/asp/standard#pricing


## Answer 25291

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2011-05-22
- score: 1

If you have repeat purchasers, consider a "points purchase" solution - used by companies such as iStockPhoto.com, Nintendo Wii (console purchases) etc.

The user buys (say) $10 worth of points which can then be spent on anything over the next year. (Accountants will want an expiry date on unused points because otherwise they will show up as an indefinite liability on the books, but the expiry date can be years rather than days). This makes the minimum transaction worthy of PayPal / credit card processing.

If you can get this to work there is a second advantage: according to behavioral economists people spend points more easily than they spend the equivalent amount of money.

Of course, this assumes that somebody looking at your website will happily say: "I can easily spend 100 points here over the next year". If they can't easily say that, a points system won't work.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
