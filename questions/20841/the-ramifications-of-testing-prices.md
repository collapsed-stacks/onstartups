## The ramifications of testing prices

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-02-26
- tagged: `pricing`
- score: 9

I would like to test prices for a SAAS (software as a service) product. I know how to do A/B testing. My question has to do with the ramifications of such testing. If we sell to Customer A for $99 and then later we offer the same product for $49, what do we do when Customer A comes back to us and says they feel ripped off? Worse yet, what about the ones who don't say anything but are thinking it?


## Answer 20971

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-03-01
- score: 4

<p>When you are split testing prices, you must bear in mind that you may be varying the price and its representation.</p>

<p>So for instance, it's the case that</p>

<ul>
<li>$99/month</li>
<li>$100/month</li>
<li>$49/month</li>
<li><s>$99/month</s> $49/month</li>
<li>$49/month for the first three months [then $99/month - prominently]</li>
<li>$49/month for the first three months [then $99/month - not prominently]</li>
<li>$99/month Enter discount code: <strong><em>_</em>__<em>_</em>_</strong> [there are no evident discount codes]</li>
<li>$99/month Enter discount code: <strong><em>_</em>__<em>_</em>_</strong> [there are discount codes presented through the site]</li>
<li>$99/month Enter discount code: <strong><em>_</em>__<em>_</em>_</strong> [there are no discount codes easily Google-able]</li>
<li>$99/month (first month free)</li>
<li>Free for the first month ($99/month visible on the same page)</li>
<li>Free for the first month ($99/month visible elsewhere on the site)</li>
<li>Free for the first month (call for pricing)</li>
<li>$99/month [placed near to another value, e.g. your own $199/month premium service, or your competitor's $250/month service]</li>
</ul>

<p>are each distinct cases that may produce materially different outcomes. And we haven't remotely exhausted the possibilities!</p>

<p>If you are <em>only</em> varying price, then the end result is that you will select the most effective price for your purposes (which might be volume maximisation, revenue maximisation, profit maximisation or some other mode). In my view, in this case you should normally aim to standardise - which in the case of price reductions you can do next billing cycle, and in the case of price increases you will typically diarise for some months out. Whether on request you will part refund current and prior periods is a matter of judgement.</p>

<p>Many times, though, you are split testing price and product/package variants. For instance, if your SAAS offering has a unit called 'projects,' you may be trying to optimise </p>

<ul>
<li>The price and number of projects for an entry level proposition</li>
<li>The number of distinct propositions</li>
<li>The 'packaging' (for instance, is the entry proposition extensible - I can pay extra for more projects? or limited - to get more projects I need to upgrade to another proposition)</li>
</ul>

<p>Depending on the means you have of reaching prospective customers, the number of variants you want to test (which grows exponentially) may prove impractical, and you must either make arbitrary decisions about scope or precedence, or use some other tool.</p>

<p><a href="http://en.wikipedia.org/wiki/Conjoint_analysis_%28marketing%29" rel="nofollow">Conjoint design and analysis</a> is a good way of determining efficient split testing strategies that will resolve these multi-dimensional questions. Used with care, it's a great way of achieving better results more quickly than simple split testing - which is inevitably loaded with possibly unreliable intuitions and presuppositions about how customers will make buying decisions. I've had great results using conjoint techniques to solve for product specification and pricing together.</p>

<p>This type of experimentation does tend to leave you with a messier tidying up job! You don't just have customers on the 'wrong' pricing, you have customers for propositions that may no longer be on offer at all. In my experience, this entails somewhat more work than single variable testing, but has less anxiety - as customers for the orphan propositions can see that there's no simple mapping from the offering they have to your current general offer.</p>



## Answer 20930

- posted by: [burritoboy](https://stackexchange.com/users/-1/7868-burritoboy) on 2011-02-28
- score: 3

A few ideas:

- **Coupons.** Promote a lower price on the first month (or first 2 months, or first year) using a coupon so you can test against a cohort and compare adoption & retention to understand a few of the economics without having to adjust prices to your core customer base. You can prompt your existing customer base with a one-time non-transferable coupon so that you earn some goodwill. You might further test by having an opt-in for 14 days, and then auto-convert into the coupon after that. Make sure you flush the coupon codes out of your system after a period of time or they may end up on online coupon farms.

- **Reengage subscribers that leave.** Offer a lower price point to reengage left customers to see if you can win them back. This won't be a perfect a/b test on the entry price, but may give you some directional data. Dating sites,amongst others, have tried this with different levels of 'spammyness'.

- **Credits vs Refunds.** Depending on the size of your customer base, refunds may be pretty difficult to manage from a cash perspective in addition to tracking down all the customers that may have upgraded/downgraded, made payments on time, and the timing of those decisions. If you choose to go with a lower price point, consider crediting their account for future service to keep them as customers without having a potentially large cash outlay.


## Answer 20843

- posted by: [zippy](https://stackexchange.com/users/-1/7781-zippy) on 2011-02-27
- score: 2

You could consider refunding customers who paid the higher price if you end up settling on the lower price point. You could either do this automatically or only for customers who inquire or complain but the better policy would be to do it systematically. In any case, the lost revenue will be minimal compared to the value of figuring out which price works best and the goodwill you will generate with the customers who receive the refund.


## Answer 20859

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-02-27
- score: 2

When you launch a new saas product, its often easier to raise your pricing. ZenDesk recently did this.

Here is the benefit.  Lets say you got a SAAS product that you can afford to low ball at 12 per month.  DO it!.  It will allow you to get say 1000 customers.  That 12k can be used to sell your SAAS product then for its true value of 40 per month. 

Your early adopters will love you, and spread the word, because they are getting a good deal.  Once you have a good reputation your 40 price is justified.   In the long run you can wean off your early adopters by locking them into the product they have, but not giving them all the new bells and wistiles you create.

It takes come careful planning but dont show all your tricks with version one.  Like a good magician (or apple), always keep them wanting more. 

Also really helps to have multiple pricing plans.  Most my SAAS have free (ad supported) and pricing that ranges from 15 - 95 per month.  (Most pay $25).  Having the big number in your pricing for the Cadillac plan is important.  It gives the impression that the $25 plan is a great value.   Every once in a while we have a cadillac buyer!  :) 




## Answer 20846

- posted by: [David](https://stackexchange.com/users/-1/2684-david) on 2011-02-27
- score: 1

I know that this might affect the testing, but I would communicate very clearly to the customer getting the product for 49$ that he is getting it under a very very special price. If you can come up with a reason (whatever reason) for this price, then you can say to customer B that A got it under very special circumstances. For B2B product this is called a strategic price, since a customer was identified as a strategic customer...


## Answer 21114

- posted by: [Nicko](https://stackexchange.com/users/-1/7870-nicko) on 2011-03-03
- score: 1

The last poster makes a really good point about communicating that the price is "very, very, special." In the same scenario, we tried to code offers to special early adopter groups, and set an expiration time to the price.  Set it far enough in the future that they won't get worried that BOOM!, the price is going to spike in the very near future. But set an expiration date. We have a SaaS product, and I'd say that pricing is a constant, evolving  process. 


## Answer 21133

- posted by: [Marco Demaio](https://stackexchange.com/users/-1/3098-marco-demaio) on 2011-03-04
- score: 0

Price ramifications go both ways:



 - when you start with a cheap price and later you rise it
   up,

 - when you start with high price and later you lower it down.

In the 1st case your customers will be tempted to look at your competitor to see if they have a cheaper price

In the 2nd case your customers will fill really ripped off, they will hate you and think at you ad an unreliable company (at least this is what I felt when my phone company did this).

Since there is no way out I strongly recommend to go for the 1st way. Basically **start finding the lowest price you can afford to sell your service for and start with it (NOTE).** The reasons:

 1. If you start with the lowest price you can afford and nobody buys your service/product you can shut down your startup or completly revisit your business model because you are actually selling something nobody wants for that price, and you don't waste months playing with price (doing uselss A/B tests) to see if someone buys it.

 2. If you start with the lowest price you can afford (and it's lower than your competitors or as low as them) you will get good word of mouth both in real world and on the web (don't undervalue this). This will allow your startup to create a good number of customers (and money) and it will make you feel more self-confident.

 3. Rising the price is still better than lowering it down, people will still look at competitors for cheaper prices, but they won't think at your company as someone who screwed them up, think at the following scenes:

One of your customer Joe talking to his friend Bob (potential customer) and saying: `"oh, company A is a good service unfotunately they increased a bit the prices lately"`, Bob is probaly lazy enough to just buy Company A service anyway without looking for competitors. 

Now think at your customer Joe talking to his friend Bob (potential customer) and saying: `"oh, company A they are charlatans they screw me up making me pay a huge price, I won't buy anything from them anymore"`, Bob at this point woud not have other chance besides looking for your competitors.

----

(NOTE) When I mean the lowest price you can afford I mean exactly what I said, it's a price that you can not reduce more because you would start gaining nothing and you already reduced the costs to minimuM.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
