## Managing Technical debt in an early stage startup

- posted by: [Jeremy French](https://stackexchange.com/users/-1/1349-jeremy-french) on 2011-05-05
- tagged: `strategy`, `technology`
- score: 7

[Technical debt][1] affects all companies, and in startups where there is pressure to get things out the door as quickly as possible, the pressure to build up technical debt is high. 

Is it an acceptable strategy to build up some technical debt to achieve momentum and market share in an early stage startup? With the view to when there is greater funding and a little more stability this debt can be more easily payed off. 

It seems to me that this isn't a bad idea, as plans and architecture can change dramatically and time spent perfecting systems which have a short lifespan is wasteful. 

But I am unsure at what stage you should start to pay back. Obviously this will cause a dip in perceived productivity at some point. Are there any guidelines as to when and how much you should start to refine the systems?

Or is it realistic to stick to 100% unit tested, peer reviewed bullet proof code from the start?

  [1]: http://en.wikipedia.org/wiki/Technical_debt


## Answer 24506

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-05-06
- score: 3

<p>You will always have technical debt, its just a given and shipping the product is a very important feature.</p>

<p>I heard a great discussion recently on <a href="http://deepfriedbytes.com/podcast/episode-66-getting-a-lesson-about-technical-debt-from-gary-short/?utm_source=feedburner&amp;utm_medium=feed&amp;utm_campaign=Feed%3a%20deepfriedbytes%20%28Deep%20Fried%20Bytes%29&amp;utm_content=FeedBurner" rel="nofollow">Deep Fried Bytes</a> discussed how to manage technical debt and provided a starting point for calculating the ROI involved in "paying off" your technical debt.</p>

<p>I think the answer is, for a startup up, go hard, make sure the user are happy and can do what they intend to. Developers skill and the overall archetecture will define how fast and badly you build up technical debt. </p>

<p>For us </p>

<ul>
<li>we put 1 in 5 to 1 in 8 sprints as a clean up sprint. </li>
<li>we have a policy that says if your revisiting something, fix it properly or not at all (unless the client is loosing money). </li>
</ul>

<p>This has kept our systems fairly clean but eventually, the rest of the surrounding technologies (databases, languages etc) move on and you have to bite the bullet and start again ... everyone puts this off and then says "we should have done it earlier".</p>



## Answer 24484

- posted by: [Doug Donohoe](https://stackexchange.com/users/-1/8906-doug-donohoe) on 2011-05-05
- score: 2

I've worked at multiple startups and seen great accumulations of technical debt and little accumulation of technical debt.  I can say that with absolute certainty that their are some types of technical debt you *never* recover from.  In addition, it is *really, really, really* hard to pay off technical debt (not unlike the United States' national debt). Your objective should be to limit the amount of technical debt as much as possible.  It is okay to carry some debt, just not a ton of it.

What troubles me most about this question is the assumption that doing something correct is something that takes longer than doing it sloppily.  The problem with technical debt is that it is compounding.  A poor decision early in the life of a start up can cost you 100s of times over down the road.

100% code coverage is not a reasonable goal.  100% code coverage of the critical sections of your code is a reasonable goal.  If you have that, then you are less afraid to make sweeping refactoring or other changes.  Don't be afraid to pay off debt as soon as you realize you have it - even if it means changing 400 classes in your system.

So, to summarize:

 - Think carefully about acquiring debt
 - Pay it off early when you do


## Answer 24517

- posted by: [edralph](https://stackexchange.com/users/-1/9362-edralph) on 2011-05-06
- score: 1

> Is it an acceptable strategy to build up some technical debt to achieve momentum and market share in an early stage startup? With the view to when there is greater funding and a little more stability this debt can be more easily payed off.

**Yes**.

When you are more established then having a scheduled amount of debt servicing as Rob says is great.  Embed cleanup in your development schedule.  **As a startup** you have to focus on shipping the core capability so your business can get going.  Going for 100% unit tested and QA'd code may mean that you don't ship the capability you need and your business will never get off the ground.  Don't get into that position.  It is *always* better to have got the business off the ground and have accumulated technical debt than to have almost-delivered lovely systems that support a non-existent business.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
