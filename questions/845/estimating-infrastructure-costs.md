## Estimating infrastructure costs

- posted by: [Andrew](https://stackexchange.com/users/-1/519-andrew) on 2009-10-12
- tagged: `infrastructure`
- score: 4

I'm working in the infant stages of a SaaS platform and we're working on estimating cost.  Right now our hosting and bandwidth expenditures are relatively low as we have only one customer, but we need to be able to estimate hosting/bandwidth costs up to a relatively large amount of customers.

What is our best bet for tackling this?  Are there worksheets/calculators around where we can plug in the average request size per user, average number of requests per session, average number of sessions per day (we have these metrics already for our first customers) and work on expanding it that way?  We need to rationalize to our investors the need for "pay ahead investment" for SaaS with real numbers, and the hosting/bandwidth side of things has us scratching our heads.

This is a new road for many of us, and I'm hoping someone in the community may be aware of best practices in estimating these sorts of things.

Thanks for your help!


## Answer 852

- posted by: [Scott](https://stackexchange.com/users/-1/88-scott) on 2009-10-12
- score: 2

<p>If you're using a cloud provider like <a href="http://amazon.com/ec2" rel="nofollow">Amazon EC2</a> or <a href="http://vcloudexpress.terremark.com/default.aspx" rel="nofollow">vCloud Express</a> to host your service, then they ought to be able to help you model these things.  </p>

<p>If you're providing your own infrastructure:  stop doing that. :)</p>

<p>Good luck!</p>

<p>Scott</p>



## Answer 862

- posted by: [Elad Kehat](https://stackexchange.com/users/-1/189-elad-kehat) on 2009-10-12
- score: 2

I'd like to join Scott in his reco:<br>
Since you're building a SaaS platform, it would make the most sense for you to use a cloud provider and "pay as you go". This saves you from the need for pay-ahead investment.<br>

Some tips as for the costs you can expect:<br>

Unless your service involves lots of bandwidth-hungry applications (in other words, videos, you-tube style), then your bandwidth costs would be negligible. 1,000's of users per day would translate into just a few $ per month. Forget the avg. request size calculations etc. - it's truly negligible.

The same goes for backup storage. S3 is $0.15 / GB / month. Use that as your benchmark and figure out how many MB you're going to use per user. My guess is that you'll find it negligible as well - but it depends on your type of service of course.

Your biggest expenditure will be on servers. Costs in the $100-200 (or lower) should serve you well enough when you start. You should be able to estimate you needs by running load tests on your current system, figure out how many concurrent users it can maintain, and use that as your benchmark.






---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
