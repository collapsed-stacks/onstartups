## How do you choose the base currency for online and mostly international sales?

- posted by: [morpheous](https://stackexchange.com/users/-1/3365-morpheous) on 2010-05-16
- tagged: `accounting`, `saas`, `pricing`, `payments`
- score: 3

We are about to launch a website offering products. My "gut" feeling is that a good proportion of our customers will be based in the US. We are currently based in the UK, though that is likely to change in the near future.

We are trying to determine which currency to use as our base currency. To clarify, people can purchase in their own currency (but a conversion will be made if their currency is different from our base currency)

The choices we have are:

1. Pound Sterling

  - Pro: Local currency (for now)
  - Cons: Currently beleaguered, near to mid term outlook not rosy
      There may be some 'reluctance' to purchase products denominated in sterling? 
      Products may appear relatively expensive to US and Eurozone customers


2. Euro
  - Pro: The new kid on the block, widely seen as the defacto replacement for the USD
  - Cons: Short term, reeling from the Greek crises, though future not in doubt, questions remain
      Products may appear relatively expensive to US customers


3. USD
  - Pro: Needs no introduction. Even used in some emerging countries alongside their local currency
  - Cons: Although heavily sold already, it may go lower still


To complicate matters still, although we are currently based in the UK, we are likely to be relocating to sunnier climes (South of France/Mediterranean or the Caribbean) in which case, either the Euro or the USD will become our local currency.

I am assuming that it would be fairly disastrous to launch with products denominated in one currency, and then switch later on to another currency - thats why I want to make sure that I make the "right" choice - or at least, the "least bad" choice.

Can anyone add some further insight to help make the decision as to which currency to select as a base currency?




## Answer 11222

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2010-05-16
- score: 3

I would choose Euros since you are based in Europe. Even if you have US customers, the conversion would be simple to do at checkout and you would not have to worry about price changes as much.

The Pound is a pain and if you are already thinking of moving, the Euro is the better way to go. Most US customers will get the Euro but be befuddled by the Pound.


## Answer 11236

- posted by: [Dario Solera](https://stackexchange.com/users/-1/1539-dario-solera) on 2010-05-17
- score: 3

<p>I have asked a <a href="http://answers.onstartups.com/questions/10934/multiple-currency-management-for-saas-payments" rel="nofollow">similar question</a>, and the general answer is that Americans prefer USD prices.</p>

<p>We'll have prices both in USD and EUR, and keep this in mind: there's no reason why the USD and EUR prices need to be connected.</p>



## Answer 11323

- posted by: [Giles Thomas](https://stackexchange.com/users/-1/1547-giles-thomas) on 2010-05-19
- score: 3

To a large degree, I think it depends on who your customers will be.  In general, consumers will be less happy with prices in currencies that are not their own than businesses.  More generally, the more web-savvy the customer, the less likely they are to be put off by foreign currencies.

Beyond that -- in my industry, with primarily business customers, I think, but don't have numbers to back up, that Americans tend to avoid products with no dollar price, Euro-zoners are reasonably comfortable with dollars but significantly prefer euros, and Brits aren't terribly bothered but rather like the option of paying in pounds.  Because our sales are split 50% US/25% Euro/15% UK, we price in dollars and adjust the euro and pound prices to the nearest round equivalent every month or so.  We're UK-based, so this strategy makes our sales vary against our expenses when the currency markets move, but the movement is random in the short term -- and if a long-term change makes our prices unprofitable, we can always change them.


## Answer 11219

- posted by: [Griftastic](https://stackexchange.com/users/-1/3446-griftastic) on 2010-05-16
- score: 2

Well, the Euro is strong compared to the Dollar, but you have to consider whether your customers will be comfortable dealing with those currencies.  I'd say to include both pounds and dollars if you are pretty sure that's where most of your customers will come from.

Being a US native, when I got o a foreign site and see:  $5/€3.93/£3.38, I just assume they are equal.  If I just see pounds, I do the quick math of £x1.5 and buy.

Since you are moving anyway, that seems to narrow it to euros and dollars.  If you're really, truly, 100% sure that most of your customers will be from the US, then go with the dollar.  

The only real negative in having both prices is that they need to be updated fairly often.


## Answer 11359

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2010-05-20
- score: 2

If most of your potential customers are based in the US you should price in USD. You will lose US customers otherwise. You will also lose UK customers if you don't price in GBP and eurozone customers if you don't price in EUR. Choose the market that matters most.

If possible, adopt @Dario Solera 's recommendation: provide currency options for your major markets. These don't need to be exact conversions: you can price discriminate (a little) between currencies. What is important for the buyer is *what-you-see-is-what-you-pay*. If you quote 500 yen then the amount charged to the credit card must be 500 yen, not some approximation of the amount. You will also need to be able to do refunds in the same currency to avoid problems with changes in exchange rates. Otherwise you will get unhappy customers and charge-backs.

 


## Answer 11325

- posted by: [J. Pablo Fernández](https://stackexchange.com/users/-1/751-j-pablo-fern-ndez) on 2010-05-19
- score: 0

Currencies are not like other units. If you were doing a weight tracker, you could pick kilos, pounds or stones and always store the same thing, then do conversions for every user. You can do that because those are stable units.

Currencies are not stable. Currencies fluctuate between each other. If you start to get really deep into it, it gets really weird. You have two prices: buying and selling and the gap between these two prices can be wider or narrower. I think you could even have cases where A > B > C > A. The whole Forex industry is based on this.

If someone payes you one dollar, and you say, this is 0.8EUR, you cannot say that the person payed you 0.8EUR, because when you analyze the information a month from now, the value of the dollar changed and 0.8EUR now is wrong. You have to record 1.0USD.

Multinational companies work in lot's of currencies, a MacBook Pro costs something different in the UK than in the US, but it's not only a matter of currency conversion. It's a matter of market and local costs.

If your costs are in pounds, you better keep your prices (at least internally) in pounds, because otherwise you may find yourself in a case where you keep selling the same amount, but your revenue goes down and you don't have enough to cover the costs. But also be aware that you can't just do a money conversion to sell abroad. It would be really nasty for your clients if your prices change every hour. You'll probably need to set up a price you feel comfortable with in the local currency or use your internal currency.

Moving could be tricky. I suppose it would be the equivalent of opening a remote branch, with prices and costs in a different currency and then closing the original branch.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
