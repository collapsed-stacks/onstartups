## Annual Maintenance Payments

- posted by: [Cocowalla](https://stackexchange.com/users/-1/2832-cocowalla) on 2010-03-12
- tagged: `software`, `sales`, `subscriptions`
- score: 2

We are planning on introducing an annual maintenance fee for a new enterprise-level product we will soon be launching.

How do you handle _when_ the payments are to be made?

For example, let's say a custom purchases 10 licenses in January, 10 in February, 10 in July...etc

It doesn't seem sensible to send an invoice every month (or whatever) - is there a better or more 'normal' way to do this?

If it makes any difference, the first year's maintenance is included in the initial purchase.

Thanks! 


## Answer 9155

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-03-12
- score: 2

<p>We have a similar situation with our product <a href="http://www.gibraltarsoftware.com" rel="nofollow">Gibraltar.</a>  We thought through a range of options, got some feedback and what we ultimately settled on is that each time you purchase a new license it includes 12 months of maintenance - but we keep a common end date for a customer.  So for example <strong>if you purchase 10 new licenses, that gives you 10*365 license-days of maintenance</strong>.  We then look at how many licenses you already have and when their maintenance ends and come up with the new effective date. This way a customer always has a single renewal date and is always getting full credit for the maintenance they are purchasing - regardless of when they buy new licenses.  </p>

<p>Example:</p>

<ul>
<li>You purchased 10 licenses 6 months ago originally.  That means your maintenance is currently set to expire 6 months (180 days) from now.</li>
<li>You purchase 10 new licenses.  This gives you 10*365 license days of maintenance to add to your account, which currently has 1800 license-days of maintenance left for a total of 5450 license-days.</li>
<li>Since you have 20 licenses, you now go through 20 license-days of maintenance per day, so you end up with 273 days of maintenance left instead of the original 180.</li>
</ul>

<p>We send out notifications to people that their maintenance is coming due 90 days before it lapses, then again ever half interval, more or less (45 days, 30 days, 15 days, 2 days, 0).   We've gotten feedback that people like the earlier announcements even though they don't act on them because they can make sure the budget is there, etc.  Then they act on one of the last reminders - 15 or 2 typically.  We modeled this after the experience of two other companies that sell noncompeting products to our market and had a few years of track record for what works.</p>



## Answer 9181

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-03-13
- score: 2

<p>As an alternative strategy which we found works quite well in the enterprise space, you could consider <strong>Subscription Pricing</strong> (I've talked about it before in answers to <a href="http://answers.onstartups.com/questions/5406/launching-enterprise-software/6149#6149" rel="nofollow">this question</a> and <a href="http://answers.onstartups.com/questions/7456/what-is-your-upgrade-policy-for-a-new-release/7479#7479" rel="nofollow">this question</a>).</p>

<p>To recap, the idea is that instead of charging a big licence fee and then annual maintenance, you charge an annual subscription fee that includes everything, including the initial licence fee, maintenance and all major upgrades.  If you want you can set up a minimum subscription period, say three years.  (If you're feeling brave or very confident in your offering, then by all means give the client the option to cancel when they like, although I would avoid any structure which means having to repay the current year's fees).</p>

<p>Why is this interesting to enterprise buyers?  I would suggest the following:</p>

<ul>
<li><p>As the annual fee is going to be less than the up-front licence would have been, it's <strong>less immediate impact on this year's budget</strong>.  Next year's budget may be someone else's problem.</p></li>
<li><p>Enterprises like to be able to <strong>predict whole lifecycle costs</strong>.  Although they'll know what your annual maintenance will be, they won't know what you are going to charge them for major upgrades (this is an important revenue source for you, so you won't want to give them away).  Using subscription pricing means they know what they are going be paying you in year 1, year 2, year 3, etc.</p></li>
</ul>

<p>Accepting that there is a downside for you of less cash in the door up-front (not an insignificant issue for a start-up), why would you do go the subscription route?  </p>

<ul>
<li><p>The obvious main is recurring revenue.  Each year you're building on top of last year's sales (and all the preceding years), rather than starting from scratch.</p></li>
<li><p>I would also argue there is a <strong>customer intimacy</strong> argument too.  As customers are paying you the same amount of money each year (inflation adjusted if you like), then they are a little bit like new customers all the time.  Potentially this gives you more opportunity to keep close to them than if you're just shipping out maintenance invoices each year.</p></li>
<li><p>Probably the biggest justification for you (and the reason we adopted the approach) is that when you go to a customer in year 2 or 3 and start suggesting they pay you a load of money to upgrade (under a conventional licence model), then there's every chance they'll go back into the market to see whether they can get a better deal.  In other words, subscription pricing is a way of increasing your product's long-term <strong>stickiness</strong>.</p></li>
</ul>

<p>In terms of admin, then becomes simple - you agree one date with the customer that you are going to bill them up-front for that year's usage.  If they add additional subscriptions, you keep the date and pro-rata the subscription fee for the rest of the current period.</p>

<p>This approach isn't for everybody, particularly considering its up-front cashflow impact, but I would strongly recommend considering it for the long-term health of your business.</p>



## Answer 9229

- posted by: [Dane](https://stackexchange.com/users/-1/1441-dane) on 2010-03-15
- score: 2

What we do is ignore the problem on new sales but fix it on the maintenance renewal. For example if you purchase 10 licenses in Jan-2010 and 5 licenses in Jul-2010 then when we do the maintenance renewal for Jan-2011 for maintenance that covers all of 2011 we include 12 months for the 10 licenses and also include 6 months for the 5 licenses so then all licenses are covered for all of 2011.

If the customer complains that they are paying early for the batch of 5 licenses then we just split the payment date.  Then when we do 2012 maintenance we do all 15 licenses for 12 months.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
