## Interpreting smoke test results

- posted by: [guidupuy](https://stackexchange.com/users/-1/16153-guidupuy) on 2012-02-02
- tagged: `market-opportunity`, `testing`
- score: 1

Looking for early market validation re our startup idea, we did a simple smoke test: we created a facebook ads campaign, linked it to a launchrock page and looked to see what happened. We set a $20 daily budget and here came the results for our first day: 

* On facebook : 139 clicks, click rate 0.039% 
* On launchrock : 49 page views, 8 signups, 16.33% conversion rate


I've got 2 questions: 

* Where did the 139-49 = 90 missing clicks go? Is facebook stealing from us? 
* How good/bad are these numbers? Any valid point of comparison out there?


## Answer 35854

- posted by: [rbwhitaker](https://stackexchange.com/users/-1/15024-rbwhitaker) on 2012-02-08
- score: 1

<p><strong>Where did the clicks go?</strong></p>

<p>It's probably not really something to be worried about, and in the end, you may need to just accept a difference as a part of life.</p>

<p>There are lots of things that lead to inconsistencies like this.  As Ryan pointed out, delays in processing and timezone changes could easily be the problem.</p>

<p>I have a website with Google Ads, and also on that site, I have StatCounter.  Sometimes, StatCounter tells me I have a certain number of clicks that went to Google Ads, but Google only shows 1/3 of that.  I looked into it and discovered that there can be quite a bit of difference in clicks and page loads with things like this.  For example:</p>

<ul>
<li>If a person clicks on a link, and then, before the page can fully load, they realize they didn't mean to click it and push the browser's Back button, you'll get a click without a page load.  </li>
<li>Launchrock may not count it as a page load if the same person loads the page twice in a row.</li>
<li>Launchrock may be keeping track of your IP address, and not counting your clicks.  If a lot of them were yours, they may not be counting.</li>
</ul>

<p>My point is not to enumerate all possible things that could be causing the inconsistency, but rather, to illustrate that there could be valid reasons why there's a difference.  Even a <em>substantial</em> difference.</p>

<p><strong>How do these numbers compare?</strong></p>

<p>dnbrv is right, one day isn't enough to go by.  </p>

<p>I'm saying this completely out of the blue, but if you have 16% of people signing up (for an email list, I'm assuming?) that seems pretty decent to me, considering you've provided absolutely no value to them, just a hook.  </p>

<p>The average conversion rate for going from first visit to purchase is along the lines of <a href="http://www.searchmarketingstandard.com/what-is-the-average-conversion-rate" rel="nofollow">0.5% to maybe 2%</a>.  It is really impossible to say how your really compares to that, since we don't know all of the details, and also, it doesn't sound like you've asked people to spend money yet.</p>

<p>I'd caution you that any comparison to other people's conversion rates is like comparing apples to oranges.  There are just too many variables involved to truly compare them, so only do so carefully.</p>



## Answer 35832

- posted by: [user16257](https://stackexchange.com/users/-1/16257-user16257) on 2012-02-07
- score: 0

I did a facebook ad campaign last fall for our student consulting firm. We spent 50€ (app. 66$) over 6 weeks. We had 500.000 Impressions and a CTR of 0.17%. The important thing I noticed was, that after a while (2 weeks) the numbers got better and better. I think if the campaign would have gone any longer the result would be even better. Hope this helps to interpret your numbers. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
