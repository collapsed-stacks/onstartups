## Are there any benchmarks for hosting/infrastructure/licensing costs for a SaaS provider?

- posted by: [BoomTownTech](https://stackexchange.com/users/-1/13332-boomtowntech) on 2011-09-14
- tagged: `saas`, `hosting`, `costs`
- score: 0

Does anyone know of benchmarks or comparisons for hosting/software/infrastucture costs for a SaaS startup?

We are running at about 3.2% of Gross Revenue and 11% of net revenue.  We feel like we are doing a good job keeping our server costs down but don't have any idea how to benchmark that.


## Answer 30086

- posted by: [JonDiPietro](https://stackexchange.com/users/-1/11642-jondipietro) on 2011-09-14
- score: 2

OPEX Engine publishes an annual SAAS benchmarking report: http://www.opexengine.com/software-benchmarking/


## Answer 30128

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-09-15
- score: 0

Hello user13332 (please change your name..),

I would say that the benchmark needs to take into account your growth strategy. If you are running with no investment for future growth, your costs seem very reasonable to me, but if you are comparing yourself with companies that do invest heavily in future growth then it won't be accurate. 

So just be careful who you are comparing yourself to, put that in perspective of the stage of the company you are looking at.

Also remember that investment in infrastructure is often time in stairs shape. Big investment all at once (you are at over capacity), then nothing until you run out of capacity, big investment again, etc.. You will see those kind of investment made after a round of funding for example.

I know I'm not giving you a straight answer but putting a bit of context around your assessment. Hope this helps.


## Answer 30135

- posted by: [TXBirder](https://stackexchange.com/users/-1/13351-txbirder) on 2011-09-15
- score: 0

Your analysis should also take into account the type of application you are providing and your expected user base. The key factor is the number of simultaneous users as compared to registered users.

For example, I was VP of Technology at a dot COM and we had 750,000 users, most of whom were only active on the site for a few hours a month. We averaged less than 300 simultaneous connected users at any given time, so our infrastructure needs were much less than would be expected given the total size of our subscribed user community.

Eric


## Answer 32588

- posted by: [Barry](https://stackexchange.com/users/-1/14427-barry) on 2011-11-14
- score: 0



That P&L's a hecofalot better than the undifferentiated heavy lifting of a certain type of platform hosting, I can tell you with absolute certainty.

Also be sure to reinvest to reduce risk and give that "can sleep without servers falling over" certainty.  Sometimes areas are missed that don't get addressed, as having no failures can be more risky that having a few actual incidents (google: Netflix Chaos Monkey).  Having staff thinking about the gameplan for traffic, security, conversion concerns is always good in addition to the usual runbook, ticket desk, surveys, etc.

Finally: Showoff! ; D   Good job.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
