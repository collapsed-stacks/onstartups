## Traction for seed funding: free or paying users?

- posted by: [Seven Dials](https://stackexchange.com/users/-1/28370-seven-dials) on 2013-10-22
- tagged: `seed-funding`, `freemium`, `fundraising`
- score: 4

<p>This topic was touched on in a fairly general abstract way in another post, but I'd like to put the question based on these specifics.</p>

<p>Here is the business:</p>

<ul>
<li>Consumer internet web app</li>
<li>Freemium business model - stripped down version is free, the premium features version will be a few bucks a month.</li>
<li>We are pre-launch but about to put the prototype into private beta shortly.</li>
</ul>

<p>The question has been asked by an angel investor I am currently negotiating with: What kind of traction are we targeting - or rather, do we need - to get to a Seed round of $300k-$500k. Is it acquisition of free users, or positive demonstration that some of them will convert into paying users.</p>

<p>The context for his question is that the prototype / MVP we have built is the free version only. The intention is to add the premium / paying features, and start charging, after Seed funding. What he is getting at is, is acquisition of free users itself going to be enough, because if not, then our capital need at this stage is going to be greater to build and ship the paying version.</p>

<p>Obviously I get that paying users are the best form of traction. But I'd like to know specifically if proving demand in the product category via free user acquisition (plus, any positive press, if we got that) could be enough to take to seed funders (eg on Angel List). Any thoughts and examples much appreciated.</p>



## Answer 51471

- posted by: [user60812](https://stackexchange.com/users/-1/19115-user60812) on 2013-10-22
- score: 1

<p>Well I don't think what he is asking you can have a Right or Wrong<br>
He wants to see what you would like to go for, and what's the reasoning behind it.<br>
If you tell him you want free users to jump start demand, build brand loyalty, etc I'm sure that's exactly what he's looking for (of course paid users would be better), you can try something along these lines:</p>

<ol>
<li>By 100k free users we feel that we would have enough traction to offer paid features</li>
<li>By 200k we feel we would be able to optimize our pricing models to cature more paid users</li>
<li>We expect to go out to VCs once we have 1m free users, with at least 10% conversion</li>
</ol>



## Answer 51502

- posted by: [OnTheShelf](https://stackexchange.com/users/-1/17699-ontheshelf) on 2013-10-24
- score: 0

<p>I read the investor’s question as “what is the point” of getting the money. It is not an unusual question when looking at business concepts based on the freemium model. Let’s take a quick look at some of what they may be looking for in an answer.</p>

<p><strong>Someone has to pay for the basic costs:</strong></p>

<p>In a Freemium model generally a small percentage of users (let’s say 3%) pay for all the costs of the free users (97%).</p>

<p>Depending on other lines of revenue (I will presume there are none), the small percentage of paid users also needs to cover the general operating expenses (OpEx) of things like an office, payroll, legal, advertising, etc.</p>

<p>I would suggest you start with some <strong>basic unit cost</strong> information, and a budget forecast for your ongoing operating expenses.  Remember, beyond just attracting the users, you have to support the product going forward.  Be thinking of having a “live-site” staff who will need to deal with service going off line (usually at the least convenient time), as well as someone to answer customer questions on a blog or customer forum, all in addition to the devs/pm/UX folks creating the software.</p>

<p><strong>Basic Units / BUC:</strong></p>

<p>Calculate exactly how much each <strong>free</strong> user costs per month (the FREE-BUC “basic unit cost”).  This might be things like 1/500th of a sever providing some REST API, etc.</p>

<p>Calculate how much each <strong>paid</strong> user costs per month ( the PAID-BUC).  Remember they are getting more in services, so they should have a higher BUC.</p>

<p>Calculate how much your total <strong>OpEx (operating expenses)</strong> will be each month.</p>

<p><strong>You cannot lose money on each one, and then make it up in volume:</strong></p>

<p>Obvious as that sounds, most freemium proposals get this one wrong.  Let’s take a look based on the example data.</p>

<p>FREE-BUC = $ .03 /month</p>

<p>PAID-BUC = $ .29 / month</p>

<p>CONVERSION RATE =  3% (for every 100 free users, 3 will pay)</p>

<p>OPEX-MONTH = $100,000  (Do a detailed budget and you will be surprised how fast 100K per month becomes a low estimate)</p>

<p>REVENUE-PER-USER/MONTH-FREE = $0</p>

<p>REVENUE-PER-USER/MONTH-PAID = $1  (I will presume you are charging them $12 / year / user)
(Note: This ignores the ~ 30% the publishing and transaction fees the APPL/MSFT/GOOG platform will charge)</p>

<p>$1 – $ .29  = $ .71 (1 x PAID-BUC);</p>

<p>$ .71 – $ .99 = &lt;- $ .28><br>
(33 x $ .03 FREE-BUC – as every 3 PAID uses must pay for 100 free) </p>

<p>Notice that there is a <strong>28 cent LOSS for each paid sale</strong>, even at a 3% conversion rate. This is NOT even counting operating expense.</p>

<p>If the conversion rate is lower than the 3% the loss gets worse, as all FREE users cost the FREE-BUC starting on day one.
With this example, more users mean you lose more money per month. Scaling up is a non-starter.</p>

<p><strong>Don’t forget the OpEx:</strong></p>

<p>Let us instead presume that each paid user is profitable by $ .25 per month, even after paying for the free users.</p>

<p>The operating costs are $100,000 per month.</p>

<p>At the per-paid “profit” of $ .25, the total PAID users needed to cover the monthly operating expense is 400,000.</p>

<p>Given a 3% conversion rate, there needs to be 13,200,000 users.  (Thirteen million users is possible, but a high hurdle in the first several years at best)</p>

<p>Presume you do fantastically and generate 13MM users, but it takes 20 months.  You now need to figure out how to pay for the Operating Expenses for those 20 months.
OpEx/Month = $100,000 x 20 =  $ 2,000,000 needed to keep the business running while you get those (“active”) users. Not surprisingly, you will need to have the profit to pay that back with a return on their investment.</p>

<p><strong>Traction question:</strong></p>

<p>If I were your potential investor, I would expect for you to be able to answer all of the basic-unit-cost, estimated OpEx and the conversation rate questions to determine if you will EVER make money. </p>

<p>I hope this helps with your planning!</p>

<p><em>As always these ideas were free, and possibly worth no more than what you paid for them.</em></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
