## question about credit card charge

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-06
- tagged: `payments`
- score: 1

We are working on building an e-commerce website. And will only accept payment on line via credit card or paypal. But now the problem is, 99% payment is like $1, $2, $5. Very some amount per transaction. We found the credit card company will charge 2%-3% of the amount plus 25 cents - 35 cents per-transaction. That means up to 50% income will go to the credit card company.

Any suggestion?
Thanka a lot.


## Answer 18672

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-01-07
- score: 3

Do you expect most customers to be frequent, repeat customers? 

The Apple iTunes Music Store has an algorithm where it tries to accumulate multiple purchases over several days and then charges your credit card all at once. If you buy something for $1, it might wait a week and then charge you, just to see if you'll buy something else so that it can put them together on the credit card charge.

Your algorithm could be arbitrarily sophisticated to strike the perfect balance between how soon you get paid, how confused your customers will be (if you wait 3 months to charge them they will not remember the charge), and what kind of customer it is. For example, you might decide to charge very frequent purchasers on a monthly basis, but charge a newbie, one-time purchaser immediately.


## Answer 18637

- posted by: [3sixteenweb](https://stackexchange.com/users/-1/6407-3sixteenweb) on 2011-01-06
- score: 1

Questions:

Will the average payment increase?

What sort of volume will you be doing?

How is your credit?  

There are other companies out their with less expensive fees. If your average sale is small, say $1-3, you may need to set up a minimum dollar amount until the volume gets to a point that you have some negotiating clout. 

Google Checkout isn't much better on the fees. I have always seen a decrease in fees with volume and age of business.  

Hope this helps. Look forward to your reply.  Good luck.




## Answer 18646

- posted by: [Giles Thomas](https://stackexchange.com/users/-1/1547-giles-thomas) on 2011-01-07
- score: 1

<p>This is a long-known problem and there are surprisingly few solutions.  If you follow links from <a href="http://en.wikipedia.org/wiki/Micropayment" rel="nofollow">Wikipedia's article on micropayments</a> you might find something useful, though TBH I couldn't in the quick check I just made.</p>



## Answer 18712

- posted by: [Paul](https://stackexchange.com/users/-1/5003-paul) on 2011-01-08
- score: 1

what is the product, if I can ask?  If it's something you expect a person to frequently get more of (or buy more from other places on the site, etc) you could do like iStockPhoto and have them buy buckets of "credits" on the site that they can spend over time.


## Answer 18749

- posted by: [Ben R](https://stackexchange.com/users/-1/6356-ben-r) on 2011-01-10
- score: 0

Not ideal because it can complicate things but you could take the credit approach. Your customers can purchase 10/20/30 credits at a time with each credit worth $1 (so they pay you $10/$20/$30). You then price your products in credits and when they make a purchase you remove credits from their balance. This only really works in cases when your customers are expecting to be making repeat purchases.

Another option is to lower your per transaction fee. We pay 1.5-3% + <b>5 cents</b> per transaction. Maybe the <a href="http://feefighters.com/">Fee Fighters</a> can help you get a better rate on your merchant account.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
