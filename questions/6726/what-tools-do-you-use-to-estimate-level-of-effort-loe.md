## What tools do you use to estimate Level Of Effort (LOE)?

- posted by: [Torrie](https://stackexchange.com/users/-1/2111-torrie) on 2010-01-18
- tagged: `project-planning`
- score: 4

What tools or methods are you using to estimate the level of effort on your projects?  I've read a lot of books on the subject, but am curious what people are actually using "in the real world".  Please also specify if you're talking about Commercial Off The Shelf (COTS) product development or consulting services, since I'm curious if the approach is different.


## Answer 6789

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-01-19
- score: 3

It really doesn't matter what is most common or widely used.  The real question is what will work for you.  This is HIGHLY correlated to who is on your team and what their experience has been. 

EBS is nice, but it only works with a history of "guesses" and then fit against actual results.  

You can't really dictate to people how to do this. 

This is essentially one of the biggest, most difficult and unsolved problems (for the general case)  in our field.  Estimates are notoriously bad or unuseful.

As long as you are aware that it is a range with a probability, then you are better off than most people.  

I have found that accurate estimates are easier when you are very familiar with the domain. 


## Answer 6757

- posted by: [Chris Hagner](https://stackexchange.com/users/-1/1523-chris-hagner) on 2010-01-19
- score: 2

<p>From Joel on Software, <a href="http://www.joelonsoftware.com/items/2007/10/26.html" rel="nofollow">Evidence Based Scheduling</a> (EBS) - Definitely worth considering... Even if you don't adopt EBS, there's lots of goodness in this article.</p>

<p>EBS may <em>seem</em> like a lot of work (relative to just going with your gut or using some multiplier to give you a safety buffer), but it mitigates a lot of really tough things to account for (i.e. poor estimation skills, individual productivity factors, etc.).</p>



## Answer 6737

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2010-01-18
- score: 0

For any project I do, the method is exactly the same. Simulate the project in OmniPlan or MS Project and track it via Key Process Indicators (KPIs). Driving my analysis is that I figure out Effort of each task not the Duration that each task would take. This is critical since the Duration of each task will vary depending on the Resources applied to it.

Once the project has been scoped out, then tracking it is done via the KPIs.


## Answer 7763

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-02-07
- score: 0

<p>Defining units of work and their complexity is a bit challenging if it doesn't fit into a wider framework, their business value and inter-relation to other units.</p>

<p>Similar in scope to EBS (scanned it, good stuff), I use crystal clear's <a href="http://devblog.point2.com/2009/09/08/blitz-planning-at-point2/" rel="nofollow">blitz planning</a> 
which can be summarized as:</p>

<blockquote>
  <p>everyone writes down all the tasks
  they know of onto index cards, throws
  them onto a long table, from which
  point they sort, add estimates and
  notes, look for the Walking Skeleton
  and the First Delivery, strategize and
  restrategize about roadblocks, costs,
  time, resources, moving the cards
  around as they go. Older folks will
  recognize this as an annotated Pert
  chart, constructed collaboratively
  with cards.</p>
</blockquote>

<p>Armed with this information, I can create feature lists, a product backlog list and ultimately a burn list.  All very agile terms - but best described in this <a href="http://alistair.cockburn.us/Earned-value+and+burn+charts" rel="nofollow">earned value and burn charts post.</a></p>

<p>There's an excellent book on this subject of small team lightweight agile methodology - <a href="http://rads.stackoverflow.com/amzn/click/0201699478" rel="nofollow">Crystal Clear</a>, by Alistar Cockburn. Rather thank write about how great agile is, the book goes into detail about how to implement it.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
