## Reports needed for ecommerce and advertising

- posted by: [user3741](https://stackexchange.com/users/-1/3741-user3741) on 2010-07-03
- tagged: `ecommerce`, `advertising`, `recommendations`, `reports`
- score: 1

I'm planning to have a develop build a CMS (in Ruby on Rails) with blogging, advertising and ecommerce integration. 

Many types of reports/charts would seem necessary in such a system: Unique viewers, page views, overall sales, average sales, sales using coupon, sales by location, ad impressions, ad click-through, sales by location, top referring links in, top exit links and order issues -- just for staters.

What other types of reports or charts would you recommend including in the system?


## Answer 12477

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-07-04
- score: 3

I would recommend you find 10 people who desperately want to use your new (as yet incomplete) system and ask them.  Alternately, 10 people who already attempt to solve this problem today with a mixture of different tools and holes in their knowledge and work with them to determine something that would convince them to switch to you.

That is, phrases like "would seem necessary" are a sure sign you haven't determined what your target customers actually want; then the question would be unnecessary.

I recommend answering this question with your customers instead of inventing more permutations of potential metrics.


## Answer 12482

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-07-04
- score: 1

Since you're showing ads, I'm assuming you're going to have some freemium model (I'd hate to pay for a service and be annoyed with ads.). If so, you'll want to keep track of the conversion percentage. 

It's not a marketing metric, but you need the cost per client. Then you can figure out if the ads plus the paying client revenue indicates a high enough conversion rate.

@Jason has a great point. You should start there and maybe some of this reporting will be useful when you're up and running, but be prepared to adapt to the changes.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
