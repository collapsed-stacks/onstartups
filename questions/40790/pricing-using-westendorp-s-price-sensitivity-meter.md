## Pricing using Westendorp's Price Sensitivity Meter

- posted by: [Johannes Rudolph](https://stackexchange.com/users/-1/11487-johannes-rudolph) on 2012-07-24
- tagged: `pricing`, `survey`
- score: 1

I have just read a [study (german)][1] that applied [Van Westendorp's Price Sensitivity Meter][2] to determine a reasonable price range for a SaaS offering. Specifically, the study tried to investigate the impact of usage-based vs. usage-independent pricing strategies. 

Put simply, Westendorp's meter works by asking 4 different price points from potential customers, at which they would consider a product to be too cheap, cheap, expensive and too expensive. The method seems extremely practical to me and it appears the required survey can be easily conducted with online survey tools. When customer contact information is retained or the customers are known, additional insights can be generated with personal post-survey interviews. 

Have you had success conducting such a study? Have you found it useful and were the results reasonable? 


  [1]: http://webdoc.gwdg.de/univerlag/2010/mkwi/01_management_und_methoden/software-industrie/05_preisgestaltung_fuer_software-as-a-service.pdf
  [2]: http://en.wikipedia.org/wiki/Van_Westendorp%27s_Price_Sensitivity_Meter


## Answer 40792

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2012-07-24
- score: 7

As someone with upwards of 20 years experience in pricing, I give very little credence to studies that ask customers how they *would* respond to a given offer, outside FMCG (fast moving consumer goods). See how they *do* respond - which in SaaS is easy and natural.

That's the first issue. The second is to poke at the underlying assumption. "I have this thing - what's it worth to you?" sounds like a reasonable question, but study evidence mainly points to human beings (which is mainly what you'll be selling to, I assume) anchoring their view of value in the price. "Here's what it costs, what do you expect of it?" is far more answerable. 

If you do want to (or need to) do something study-led, conjoint analysis does have some use. "Which would you rather have, A or B" still has a bunch of traps for the unwary, but can help you home in on value drivers.

I'm *not* saying that pricing studies of this type are innately flawed. There are a great many markets for which there isn't really any other alternative. But as a word to the wise, read the surrounding information carefully, and you'll find more often than not that there's a ton of context stuff you need to understand, a set of assumptions that may or not map into the space you're interested in, and a requirement for a relatively high level of statistical understanding called for to test and verify the work, never mind to replicate and interpret a similar new piece of work.

Good luck, have fun, and bear in mind that most of what you read on pricing - this included - must be taken with a large pinch of salt.


## Answer 40791

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-07-24
- score: 1

<p>Pricing is always a challenge.  Just a mention on the validity of freemium models could start a flame war. I have not used Van Westendorps approach, but there are always multiple ways to come to develop a pricing strategy. Here are two approaches to consider - hopefully they will be of use to you..</p>

<p>1) Understand your customer segments.  Each one has a pain threshold and an alternative way to address it (called by some a price anchor).  Segmenting these customers are important, otherwise you will get mixed messages and cloud the pricing exercise. Of course, you need to have a clear understanding of what your product is and what alternatives exist. Running Lean's Ash Maurya has a <a href="http://blog.spark59.com/2012/dont-ask-customers-what-theyll-pay-tell-them/" rel="nofollow">good post</a> on this. </p>

<p>As an example, <a href="http://www.sumologic.com/product/pricing" rel="nofollow">here</a> is a SaaS company using an anchor in their pricing page: They calculate the price of their solution and a on-premise solution for comparison. </p>

<p>2) If you already had the customer discussions and want to determine which model converts the best,  you can do automated a/b (<a href="http://en.wikipedia.org/wiki/Multi-armed_bandit#Semi-uniform_strategies" rel="nofollow">epsilon-greedy</a>, <a href="http://tdunning.blogspot.com/2012/02/bayesian-bandits.html" rel="nofollow">Bayesian Bandit</a>) testing to determine which pricing model converts the highest. Determining what the goal is, whether the population is statistically relevant, etc. is part of the test strategy you need to set. </p>



## Answer 41438

- posted by: [Reuben Swartz](https://stackexchange.com/users/-1/19294-reuben-swartz) on 2012-08-17
- score: 1

Van Westendorp works best when people understand the product really well (although Jeremey's caveat is important). For a SaaS offering, unless there is relatively little differentiation from a SaaS offering that your respondents are already using, you are unlikely to get good results. Beyond the limitations of the survey, small changes in the way you present the information will make a big difference.

Why not run a real life test with some AdWords and some test prices? (You can always move people who paid "more" down to the price you settle on.)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
