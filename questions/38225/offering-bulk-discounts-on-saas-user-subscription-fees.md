## Offering bulk discounts on SaaS user subscription fees

- posted by: [Kosta Kontos](https://stackexchange.com/users/-1/16592-kosta-kontos) on 2012-04-16
- tagged: `pricing`, `saas`, `discounts`
- score: 8

Please note that I am specifically referring to SaaS providers that have adopted the traditional pricing model of charging per user per month, and have at some point considered offering pricing tiers for bulk users (ie: first 10 users are billed at $50 per user per month, then next 20 users at $45, the next 50 at $40, etc). In other words, I am not referring to offering discounts to customers who pay their monthly fees in advance for the year, as this has already been covered extensively on this forum [here][1] and [here][2].

The reason I ask is because I've recently read "Behind the Clouds" by SalesForce.com CEO Marc Benioff. Marc discusses how all their customers pay the same monthly user subscription fee, regardless of whether they have 5, 50 or 5000 users. To quote Marc:

> Many of our sales reps who came from the enterprise software
industry were accustomed to offering a discount. The discount
had become their closing strategy when they had to make their
targets. I didn’t think we needed that motivator, and I believed
that our service was fairly priced. Discounts, I thought, were tied
to perceived risk. Offering deals would compromise the service’s
value.

> Most important, by keeping the price the same for everyone,
we kept the costs low for everyone. It was the most democratic
way. Unlike the rest of the industry, we charged the same per
seat, whether someone wanted two licenses or two hundred.
Why should someone pay less just because his or her company
was bigger? That didn’t seem fair.

Furthermore, some companies take the tiered subscription fee model I described above, and extend it with an "unlimited" user / flat license fee for their largest customers. An interesting argument against this was put forward by Joel Spolsky in his article on [pricing software][3], where he explains that:

> I have certain competitors that do this: they charge small customers per-user but then there's a "unlimited" license at a fixed price. This is nutty, because you're giving the biggest price break precisely to the largest customers, the ones who would be willing to pay you the most money. Do you really want IBM to buy your software for their 400,000 employees and pay you $2000? Hmm?

> As soon as you have an "unlimited" price, you are instantly giving a gigantic gift of consumer surplus to the least price-sensitive customers who should have been the cash cows of your business.

It's interesting to hear the views of these industry giants.

What is your personal experience? Do you offer bulk user discounts for your SaaS solution?

If not, why not? And if so, why (and how)?


  [1]: http://answers.onstartups.com/questions/18925/monthly-or-annual-subscriptions-or-both
  [2]: http://answers.onstartups.com/questions/5803/is-it-proper-to-offer-discounts-upon-longer-subscription
  [3]: http://www.joelonsoftware.com/articles/CamelsandRubberDuckies.html


## Answer 38380

- posted by: [Joe Corkery](https://stackexchange.com/users/-1/4699-joe-corkery) on 2012-04-20
- score: 3

The point of offering an unlimited pricing in this context is to make the next lower tiers look attractive to potential buyers. Ideally, the unlimited price would be set so high that you wouldn't care if an IBM or another behemoth purchased that plan because it would be so prohibitively expensive if they didn't have that same user base. Clearly, this isn't the case that Joel is envisioning, because I'd never offer an unlimited license at a price so low.

In order to set an unlimited price, you need to know your potential market. Imagine your top 5 largest potential customers (and dream big here). Figure how many potential users might exist at the smallest of these companies and then set your unlimited pricing somewhere at or below what it would cost to get a license for every potential customer in that company. If you do that, an unlimited price becomes attractive to your largest customers, but only if they wanted to get a license for EVERYONE (which might not otherwise be the case) and not particularly attractive to the rest of the world. You want to give the biggest customers a reason to buy a license for everyone instead of just a subset of interested users.

You should have very few "unlimited" customers.




## Answer 48538

- posted by: [Ryan Elkins - IActionable](https://stackexchange.com/users/-1/2566-ryan-elkins-iactionable) on 2013-04-11
- score: 2

SalesForce.com (Marc Benioff's company) definitely does offer discounts to larger customers. They don't advertise it, and that may be the difference. I know plenty of companies that are paying FAR less than the advertised price. 

I don't think that's a bad way to go - advertise one price, let the big customers tell you there is no way in hell they are paying that price, and work from there. Most customers will try and negotiate the price regardless of what you list. For some it's simply less worthwhile to do so than for others.

Part of the reason is that there is some level of support and help you'll be providing for each customer. The amount of time a customer needs generally doesn't vary a whole lot based on size. I'm sure you'd much rather have 1 customer with 1,000 users paying X than 1,000 customers with 1 user paying X. Invoicing, account management, etc - is all easier with fewer customers. That's why it's worth discounting a big customer but not really worth it for a small one.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
