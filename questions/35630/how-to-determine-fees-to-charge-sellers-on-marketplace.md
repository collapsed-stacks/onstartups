## How to determine fees to charge sellers on marketplace?

- posted by: [sk24iam](https://stackexchange.com/users/-1/4660-sk24iam) on 2012-02-02
- tagged: `market`, `fees`
- score: 0

I'm working on building a fee structure for a website marketplace that allows buyers to purchase frrom third party sellers.  Similar to ebay...  So I must charge sellers a fee for their final value sales.

I'm looking for some advice on how to determine this fee structure and what to consider.

So far I am considering how much the merchant account charges me per transaction, the monthly server costs, and the average sale amount, competitors fees.

What makes it tricky is that it's hard to determine a fee structure that would be appropriate for the first year and also when the busienss has scaled and volume has increased.  Some websites charge a flat fee while others are based on brackets for the sale price.

Any advice would be greatly appreciated.
Thanks


## Answer 35638

- posted by: [Sid](https://stackexchange.com/users/-1/13800-sid) on 2012-02-02
- score: 1

First, do something about your user profile's accept rate on this site itself :)

Back to the point, you threw in a myriad of possibilities, most of which are fair to think about. I'd address them as:

  1. **Differentiation**: What is going to keep you different from eBay? Your product offering, your targeted market - or price? I hope it's not price but if it is, eBay is your benchmark. Just wanted to get this out of the way first ...
  2. **Per transaction cost**: I'd talk directly to the merchant account sales person or support telling them you have this issue. See if you can get a discount if you can batch process them for a lower effective per transaction cost. Microtransactions use the same principle to reduce their overheads.
  3. **Smarter payment routing**: This depend on the mix of your product sales, but perhaps it's best to have not one but TWO routes for processing sales - one for large items and another for smaller items to drop the effective per transaction costs.
  4. **Hedge profit margins for volume risk**: It looks like it's too early for you to know
  * number of transactions (volume)
  * size of each transaction or composition of transactions (eg 30% under $10, 70% over $10)

  In this case I'd suggest that your hedge by picking a processing plan that keeps your fixed cost at a minimum. So you'd focus on keeping being profitable on the variable costs/in every transaction. Sure, this means you may *less* profitable on each transaction but at least you won't hit losses (due to fixed costs) if you miscalculate the volume. Of course, I'm assuming there is some margin to play with here. Once you have some history of volume, you can always renegotiate/change your payment routes to optimize it for those volumes by modeling this excel. (eg: You may find that paying $500/month fixed cost to shave 1% off the variable cost is actually more meaningful given volume X @ transaction price $Y).

Good luck!

Sid



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
