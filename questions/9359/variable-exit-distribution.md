## Variable exit distribution

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-03-18
- tagged: `seed-funding`
- score: 1

Is it possible to promise seed investor variable share of the exit. E.g, if the exit(or any liquidation event) is 10M I'm willing to give 5%, but if the exit is 50M, i'm willing to give 10%. 
My idea is that when the the absolute amount I may get as a founder grows, I'm willing to share early investors a relatively larger chunk of the pie. 
Does it make sense? and what is the technical way to do it?
Thanks.


## Answer 10073

- posted by: [WooYek](https://stackexchange.com/users/-1/3061-wooyek) on 2010-04-11
- score: 1

<p>IMO you can. In my country, legislation allows to put this in a terms of agreement founding a <a href="http://www.quicksprout.com/2010/03/31/beginners-guide-to-corporate-entities/" rel="nofollow">LLC</a> company, or just agreement between a company and and investor.</p>



## Answer 10080

- posted by: [Tall Jeff](https://stackexchange.com/users/-1/957-tall-jeff) on 2010-04-11
- score: 1

<p>There are several potential ways to create the effect you are looking for and it is generally done through defining a class of preferred stock called "<a href="http://en.wikipedia.org/wiki/Participating_preferred_stock" rel="nofollow">participating preferred stock</a>" and/or by structuring the investment into a debt instrument with what is called "<a href="http://en.wikipedia.org/wiki/Warrant_%28finance%29" rel="nofollow">detachable warrants</a>" (stock options). (This means that warrants go along with the note with a certain set of rules).</p>

<p>What is interesting about your question is that you are actually looking at increasing the percentage share of ownership for the investor as the exit size increases, while normally (in most cases) the objective would be to decrease the share of ownership as the payout gets larger. The reason for this in the "normal case" is to give the investor added leverage for smaller exits to try and guarantee a minimum return objective for them, however once getting them that money back "off the top", their overall take from the exit (as a percentage) goes down as the deal get bigger.</p>

<p>In any case, the most direct way to accomplish what you want to do is think of it as  offering stock options in addition to the "normal" shares in the company they get for their investment. (structurally this is usually done through the definition of a preferred stock class). The stock option piece is setup to have a "strike price" at the amount you want to have the added return start to kick in. To accomplish this exactly the way you describe makes the stock mathematics tricky, but it is possible to do.</p>

<p><em><strong>Crude Example</em></strong>: Let's assume 1M shares in the company on a fully diluted basis. At $10M exit, the share price is $10. At the $50M exit, the share price is $50. You can see to achieve your stated goal at the $10M exit, you want them to get $500,000 but at $50M you want them to get $5M. To set this up, you could issue them 50,000 direct shares and then also 75,000 options at a strike price of about $16.68 cents. This means that at any share price below $16.68, the options are worthless. However, at anything above that they start to create value. ie:</p>

<ul>
<li>$10/share: 50,000 shares is $500,000 (5% of total) and the options are worthless because they are under water.</li>
<li>$50/share: 50,000 shares is $2,500,000 and 75,000 options are worth $2,500,000 (which is 75,000 times ($50 - $16.68)) for a total value of $5,000,000 (10% of total).</li>
</ul>

<p>Note: I have ignored a few subtle pieces of the stock math here and how the exact stock price is affected by the exercise (or not) of the options, but hopefully this gives you an idea of how it would work. Again, the normal mechanism to actually do this is to setup a preferred stock class with a preference to take some money off the top and then after that redeeming the preferred stock by converting those shares into common shares to get another bite at the apple - this is the classic way of making a "participating preferred stock" work.</p>



## Answer 11620

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-05-29
- score: 0

Another way is to simply have an agreement where in the event of selling the company you agree to pay the investor according to a predefined schedule.

This means the money will be treated as ordinary income instead of long-term cap gains, but if this is in America it's highly likely the Bush tax cuts will be allowed to expire and the tax difference will become small.  This does waste a little money but is trivial to set up.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
