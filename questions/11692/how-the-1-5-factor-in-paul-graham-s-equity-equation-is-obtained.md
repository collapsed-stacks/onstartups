## How the 1.5 factor in Paul Graham's equity equation is obtained?

- posted by: [xavi](https://stackexchange.com/users/-1/3567-xavi) on 2010-06-02
- tagged: `equity`
- score: 4

In "The Equity Equation" essay

http://www.paulgraham.com/equity.html

Paul Graham says...
"If your valuation grows 3x a year, the total cost in stock of a new hire's salary and overhead is 1.5 years' cost at the present valuation."

Can please someone provide more details on how the 1.5 factor is obtained?


## Answer 11727

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2010-06-04
- score: 2

This 1.5 factor is independent of the 3x per year number. His point is that in order to calculate the expense of a new hire, you need to multiply their base salary by 1.5x. This gives you salary + overhead number that you can then use to calculate how much that person costs. Once you have the cost of that person, you can then use that to calculate the return on that person and how much "equity" you give up (since you are burning through cash to pay someone and you would have to raise that much more).

He does run through an example (reproduced below):

"Let's run through an example. Suppose the company wants to make a "profit" of 50% on the new hire mentioned above. So subtract a third from 16.7% and we have 11.1% as his "retail" price. Suppose further that he's going to cost $60k a year in salary and overhead, x 1.5 = $90k total. If the company's valuation is $2 million, $90k is 4.5%. 11.1% - 4.5% = an offer of 6.6%."

In the example above, the stock % for the new hire is worth 11.1%. The salary cost is another 4.5%. When you subtract that, you get 6.6%, which is the amount of the company you give away in equity, at that evaluation, to make a stock "profit" of 50%.






## Answer 40115

- posted by: [Ben McCann](https://stackexchange.com/users/-1/18507-ben-mccann) on 2012-06-22
- score: 0

    1 + 1/3 + 1/3^2 + 1/3^3 ... = 1.5

This is an infinite geometric series so you can see that it's 1.5 by plugging 1/3 into the formula for such series:  1/(1-1/3) = 3/2

pg said earlier in the article "to translate salary and overhead into stock you should multiply the annual rate by about 1.5".  It can be a bit misleading that he used 1.5 as an example number for two different parameters to consider, but they are completely separate and unrelated.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
