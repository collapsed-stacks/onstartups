## How to properly estimate the cost and necessary income for a new SAAS project?

- posted by: [mamcx](https://stackexchange.com/users/-1/15061-mamcx) on 2011-12-15
- tagged: `software`, `launch`, `cost-estimation`
- score: 2

I will launch a new SAAS (software as service) invoicing app for the iPad. This is in late-stage development.

My startup is small, and I want a clear picture on the cost of the project, and correctly estimate the revenue that can be generated from it.

This project is funded from my own pocket, and we don't have investors, which are hard to get in Colombia. It's important to manage/estimate the economics properly.

The project has the following costs involved:

- 2 developers
- Cloud Hosting: Fixed price to be online and for on-demand data transfer. I don't know the cost of data transfer as yet. I'm waiting for the first test with a big data set.
- 30% cut to Apple (in-app purchase) or 9% for another payment processor.
- Regular office, internet, phone, etc.

What else do I need to consider?




## Answer 33823

- posted by: [PhD](https://stackexchange.com/users/-1/8167-phd) on 2011-12-17
- score: 1

> As today, I have this costs identified...

Let's *assume* a you can 'fix' a number to every item you listed and it turns out to be $100,000. Will it help? Does it paint a clear picture? Will you go ahead with the plan if you can afford it?

The fact that you've asked this question implies that there is still something more and it just may not be all that simple :)

So here's what you can try - create a top-down decomposition of your project and keep these **top-level** costs in mind:

 - Execution costs (= build/construction + project management)
   - Build/Construction = requirements/prototyping + design + construction + integration etc., (Software cost estimation is a field in its own right! - estimating this itself could be problematic and it's better not to handwave it's cost but break it further down and estimate)
 - Quality assurance (= testing, reviewing etc.,)
 - Deployment & Support (= user documentation, installation, user support, website etc.,)
 - Office-space/facilities 
 - Operational costs (= hardware/software, internet, wifi etc., you need to execute the project)

These are some high-level items to consider (you may look at examples of what all to show in a business case and you'll get a broader picture).

Now, for the income: It seems your only income is the number of sales? But there could be manyyyyyyyy more channels! E.g., Licensing, maintenance contracts, training. Making money by saving money (i.e., applicable if the tool/software helps save time in essence saving/making money)

In the latter you will "deduct" about 30% of the revenue and that will give you an overall benefit.

You could either do a simple cost-benefits analysis or IRR/ROI + NPV analysis to know whether your project is indeed worth it.

The BIGGEST FLAW of the above 'model' is the notion of 'fixed numbers' i.e., you may assume the most likely number and base your calculation and may land up in doom when you look at it a year or two from now. What's wrong? Well you used A NUMBER which you knew nothing about (not really but you get the point) - only a gut feel! Basically you haven't accounted for RISKS! Things that could go wrong! You could just calculate the risk exposure ( RE = Probability of loss x impact of loss) and scale your estimates accordingly. Ex.: if the probability of failure is 40% and the impact $10,000 your RE = 0.4 * 10,000 = $4000 So scale down your estimate by $4000)

You may also do this: use a range for some of the estimates that are relatively unknown (e.g., internet costs/month can be quite fixed, but not so much for development/QA efforts). Take a worst, most-likely, best case scenarios to know your 'range' of expenses/revenue options. You'll have 3 estimates at the end and will have a better idea about the overall 'risk' so to speak

If you wish to make it more complete feel free to supplement it with Monte Carlo Analysis :)

The thing is this - create a work breakdown structure (WBS) like the above and go a few levels deep till you are confident about the estimates. Sum them up all the way to the top (WBS is like a tree structure). This estimate of 'deep' WBS is more accurate than that of a shallow one (like you gave in your post). Talk to the relevant people and try coming up with the best realistic estimates and then decide!

Hope this helps!





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
