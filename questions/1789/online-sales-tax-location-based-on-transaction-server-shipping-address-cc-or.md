## Online Sales Tax: location based on transaction server, shipping address, CC, or location of purchaser?

- posted by: [user960](https://stackexchange.com/users/-1/960-user960) on 2009-10-17
- tagged: `sales`, `tax`
- score: 7

Online sales tax seems overly complicated. From what I've read, it seems like most states collect sales tax if your company has a physical presence; however, location on both ends is badly defined:

On the company side,

- If your company is registered in a state (say Delaware), but have no physical presence, does this count this state apply?
- If you rent servers or colo servers, does this count as physical presence?

On the purchase side,

- What does the purchase location entail? Is this the state of the server which made the transaction, the final shipping location, the location that the credit card was issued, or the current location of the purchaser?

Also, is there a chart somewhere that has the updated tax information by state?

Thanks!


## Answer 1839

- posted by: [Mark Beadles](https://stackexchange.com/users/-1/296-mark-beadles) on 2009-10-18
- score: 7

What you're asking about is something called "nexus". Nexus is the minimum level of commercial activity within a jurisdiction that is enough to cause a business to fall under the jurisdiction's tax regulations, such as collection and payment of sales tax.

Some business activities clearly fall under the definition of nexus, such as operating an office in a jurisdiction.  The complication is each state has a different definition of nexus, and nexus can be defined very loosely. It does not even require a permanent physical presence in the state in some cases. So, in short, it's complex, and you may not want to tackle it yourself.

In addition, sales tax rates vary by state and locality in the US; for example, you may have a state tax, a county tax, and a city tax. You might even have two different sales tax rates within the same zip code (I remember running into that one time). And of course rates change all the time due to local levies, new state laws, etc. The chart you're asking for has to be dynamic. 

The above are complexities that are not core to your business (whatever it is), so you might not want to waste your energy doing it yourself. When I've had to deal with this in the past, what we did is outsource the tax calculations to a third party that specializes in that function. 

ADP has this kind of service, and there are some others such as Avalara and Sabrix in this business as well.

Good luck!


## Answer 1797

- posted by: [Chris W. Rea](https://stackexchange.com/users/-1/953-chris-w-rea) on 2009-10-17
- score: 2

<p>I'll let somebody who knows more about sales tax answer the first part of your question.  </p>

<p>But, I can point you to this Wikipedia article on that last point:  <a href="http://en.wikipedia.org/wiki/Sales%5Ftaxes%5Fin%5Fthe%5FUnited%5FStates" rel="nofollow">Sales taxes in the United States</a>.  It's very detailed information on each state's sales taxes.</p>

<p>Here's another reference in table format: <a href="http://www.taxadmin.org/FTA/rate/sales.html" rel="nofollow">State Sales Tax Rates</a>, from the Federation of Tax Administrators.</p>



## Answer 2596

- posted by: [Paul O'Brien](https://stackexchange.com/users/-1/759-paul-o-brien) on 2009-10-28
- score: 0

Track everything
The concept of nexus and the chart BasicallyMoney.com provided, I suspect, answer your question generally.   Bottom line, what do you do about it now?  Track everything.  Legislation will pass requiring tax collection in each state regardless of where you reside (or distribute).  

Big marketplaces involved (eBay, Etsy, Amazon, Commission Junction) are following this issue closely and should do something about it.  (I can't speak for them but essentially they'll enable HUGE headaches for their sellers/merchants if they don't simplify sales tax across state lines).  But for independent or direct sellers, you'd be wise to keep records of what was sold, when, and to/from where.  Use an online service to track everything.  We're working on this very challenge and automate the record keeping now; sales tax to come when it's an issue.  Good luck!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
