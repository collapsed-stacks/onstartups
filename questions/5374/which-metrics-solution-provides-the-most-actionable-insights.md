## Which metrics solution provides the most actionable insights?

- posted by: [Nima](https://stackexchange.com/users/-1/2007-nima) on 2009-12-22
- tagged: `metrics`, `analytics`
- score: 2

I am considering incorporating better metrics software on my site. The three option I am most familiar are Google Analytics, KISSmetrics, and MixPanel. Any thoughts on the pros/cons of each would be useful. I need a solution that is relatively simple and provides actionable metrics. Thanks


## Answer 5472

- posted by: [Craig Daniel](https://stackexchange.com/users/-1/43-craig-daniel) on 2009-12-24
- score: 2

Google Analytics is good for traffic trends (pageviews) over time and compete with classic web site measurement suites like Omniture and WebTrends.  They have Events (rather clunky implementation) and Funnels, but they are most for histrorical reporting rather than actionable metrics that you can use to tune your online business.  Also, they are not real-time (~ 3 hours behind) and the API is not as open as it could be (i.e. no events in API).  The price is FREE, which is better than both of your other options.

Mixpanel is purely event based (with funnels) and pretty much swings the pendulum the other way from GA.  It is really easy to implement and has a transparent pricing strategy when you use more than 20k events/month.  It is also realtime, which is nice.  The downside is that is it is pretty new and I'd say the entire product is a "Minimum Viable Product".  There are a number of features that aren't implemented but it is pretty decent and workable if you are OK with purely event based metrics.

KissMetrics is the newest of the bunch and is definitely following the "LeanStartup" approach.  There are not a whole lot of features in their beta version, but they distinguish themselves by identifying real visitors instead of pageviews, and focus on a conversion funnel over traditional site stats.

In conclusion, I would definitely put GA on your site for basic traffic trends and analysis.  There are a number of advanced features that you can tap into when you get your head around it but remember it is best for trends, not actionable metrics.

In addition, I would try both Mixpanel and KissMetrics, but I think KissMetrics has a few things going for them in the long run:  

 - A larger infusion of cash than Mixpanel (Y-Combinator)
 - A rockstar team of employees, consultants, and advisors
 - "People as the basic unit of measurement" over pageviews (GA) and events (MixPanel).  At the end of the day people purchase software; pageviews or events don't purchase.

I've used all three...let me know if you have any more questions.




## Answer 13157

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-29
- score: 0

Craig, I saw your tweet about KissMetrics not offering startup pricing. Agree with you. Since I haven't used the product and you have, would you say that it truly offers better actionable metrics than Google Analytics? I am also looking at Mixpanel, and if you have any more insight now that you've used all of these platforms for several months since the question was originally asked, that would be great. Thanks, Josh


## Answer 13158

- posted by: [Jeff Epstein](https://stackexchange.com/users/-1/3666-jeff-epstein) on 2010-07-29
- score: 0

<p>Try <a href="http://getclicky.com" rel="nofollow">Clicky</a> it is better than Google and would compliment MixPanel / Kissmetrics.  It is likely you will want both an Analytics and Funnel Analysis software as they measure different metrics..</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
