## Easiest way to track users and metrics in MVP?

- posted by: [Greg](https://stackexchange.com/users/-1/2427-greg) on 2010-04-23
- tagged: `metrics`, `analytics`
- score: 1

I'm working on a very early stage web app, and I'm trying to figure out the easiest way to track some basic user metrics beyond traffic and all that.

Some context:

 - Limited budget - free or cheap is good
 - Constrained dev resources
 - More interested in usage behavior (e.g., which features people are using, how often) than conversion right now
 - Would like to be able to tie to cohorts/individual users as much as possible rather than looking at averages - hate averages ;-)

I'll probably be using Google Analytics, but I haven't had time to figure out whether it can do this stuff and how well/easily.  Should I just study up on it, or is there a more appropriate option?

Also, I'm not very knowledgeable in this area, so terms like event-based metrics make me more rather than less confused.




## Answer 10545

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-04-23
- score: 1

<p>Outside of traffic it depends what other metrics you're looking for. Unless you ask your users to register and fill out some date in their profile, it is probably a good idea to have a multiple sources, by comparing which, you will get a better idea of what your typical user looks like.</p>

<p>Google Analytics is a good start.  </p>

<p><a href="http://www.compete.com/" rel="nofollow">Compete</a> is another tracking option. </p>

<p><a href="http://www.quantcast.com/slatecast.com" rel="nofollow">Quantcast</a> is yet another. </p>

<p><a href="http://www.alexa.com/siteinfo/slatecast.com#" rel="nofollow">Alexa</a> started tracking this as well.</p>

<p>From my personal tracking data I can see that neither one is very accurate, but by looking at all of them I can certainly see the trends.</p>



## Answer 10558

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-04-23
- score: 1

<p>First off, you can track what's being clicked on in just about any analytics package, you may just have to set it up manually. In Google Analytics I think it's called "event tracking".</p>

<p>In the past, may uISV's recommended <a href="http://getclicky.com/" rel="nofollow">Clicky</a>. It is not strongly optimized towards cohort or funnel analysis. It is more of a general tool in the same way Google Analytics is, but it's more real-time and fine-grained.</p>

<p>The new hotnezz seems to be <a href="http://kissmetrics.com/" rel="nofollow">Kissmetrics</a> (in semi-open beta) -- I haven't used them, but there is a lot of buzz around their product. Ash Maurya has written a bit about <a href="http://www.ashmaurya.com/2009/12/a-first-look-at-some-metrics-numbers/" rel="nofollow">how he uses Kissmetrics</a>.</p>

<p>If you really want to learn about user needs and behaviour, then website analytics will not be enough. The better tools are A/B testing, talking with actual customers, and usability tests (observing actual customers while they're interacting with your site). Regarding A/B testing, I can recommend <a href="http://rads.stackoverflow.com/amzn/click/0470290633" rel="nofollow">"Always Be Testing"</a> as a very good introduction.</p>

<p>Last but not least; see the "Related" sidebar on this site...</p>



## Answer 10555

- posted by: [David Wang](https://stackexchange.com/users/-1/2895-david-wang) on 2010-04-23
- score: 0

<p>I'm currently trying to figure this out as well for my site, <a href="http://www.simplizt.com" rel="nofollow">Simplizt</a> (shameless plug, I know!).  I'm using Google Analytics (GA), and I think it's a pretty good product that fits into your budget (free!).  The core feature of GA is the ability to track page views and some of the other basic info you'll get from another metrics package.  </p>

<p>However, to determine the REAL health of your site, you'll need to use event tracking.  An event is anything that you deem worthy of tracking.   I also happen to be figuring this out right now, so i'll share what i'm learning so far:</p>

<p>I think site health (metrics) can be broken down into three pieces, (this may change based on what your site is/does):</p>

<ol>
<li>User Acquisition - is there a general acceptance to your product in the market (visits to your site)?  are you converting well (visits-to-registration ratio)? </li>
<li>Stickiness - once people register, are they coming back?  are they doing the things on your site that you were expecting them to? are they doing it often?  what are they doing instead?</li>
<li>Viralness - are they sharing out your site?  are they seeing what link you're providing to share out your site?  </li>
</ol>

<p>An example of an event would be the answer to each of the questions above.  I'm currently working on using Google Analytics to track each of those to see if my site is functioning like it's supposed to .</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
