## Recommendations on analytics approaches for web startups

- posted by: [Howie](https://stackexchange.com/users/-1/1694-howie) on 2010-01-31
- tagged: `analytics`, `metrics`
- score: 3

Like most startups with a focus on quick execution and conservation of cash, we're looking for a good-enough analytics solution that provides us the minimum of amount of *business specific* measurement capability.  A solution that provides the best balance of features with reasonable implementation time and reasonable cost.

Certaintly Google Analytics is a great start.  However, the reason I said "analytics" vs. "web analytics" is because shortly after I get the normal metrics that a web analytics solution typically provides, I'd like metrics that are specific to my business.  Examples of these metrics might be:

a) the number of repeat visitors (as measured by my site's user ids, not cookies) for each day, where I define "repeat" as coming back over multiple days, not multiple times per day, etc.

b) the number of users who take a given site-specific action (so if I'm an auction site maybe that action is making a bid)

etc.  (I provide lots of specifics in (a) and (b) not because I'm looking for your answers to these questions but rather to demonstrate what I consider busines-specific requirements.)

My questions are:

1. How far will Google Analytics (or other free web analytics solutions) go in terms of providing business-specific metrics like the examples I gave above?  Said differently, have people been able to use GA and other tools beyond providing the standard "web" metrics?

2. For resource-constrained startups, is the task of collecting and analyzing web-specific metrics ("web-specific" meaning data points like uniques, page views, etc.) a separate and distinct exercise (from a technology and process standpoint) from that of non web-specific metrics ("non web-specific" meaning qty of business-specific actions like bids or votes)?  Or, is it possible based on tool capabilities to take a holistic approach?  I make the web-specific vs. non web-specific distinction because the web is a channel whereas the business-specific metrics span channels.

I'm looking for an approach which doesn't break down (requiring me a lot of time and effort) the moment I ask questions that aren't part of the package defaults.


## Answer 7366

- posted by: [newyuppie](https://stackexchange.com/users/-1/1961-newyuppie) on 2010-01-31
- score: 1

It's hard to beat Google Analytics: it's simple, free and so powerful. You can create your own custom reports so contructing business specific analyses is really simple. You can also define Goals, where you can define a goal to be "Landing on a specific page". If you make a bid, you would input that bid page on to the Goal area of Analytics and you would have that metric in no time.

As I see it, there is a decision you must make, and it is whether you outsource or you install the analysis tools on your server. The latter is also made possible by Google (the tool is called Urchin), but it's expensive, and hard to configure.

I would definitely go with Analytics.

Hope it helps


## Answer 8073

- posted by: [Chris](https://stackexchange.com/users/-1/412-chris) on 2010-02-14
- score: 1

Start with the end in mind. So somewhat similar situation for me. My steps:

- What were the Key Performance Indicators I wanted to capture to measure my business? My whole wish list of what I thought was important. Cost of Customer Acquisition, traffic conversion percentage to free trial, activity levels (via various datapoints) for users, revenue per user, etc.

- Map out how to get those metrics. Google Analytics, potential other web analytics solutions, internal development, etc.

- Prioritize and analyze - what did I really have to have, what would be the costs for implementing these other solutions beyond what we already had, how did this prioritize against other tasks on my plate? It was about compromise. And about reasonably working in my needs against my resources (especially engineering) to implement.

- We did the first phase. The absolute mandatory items.

- As we went, we would periodically determine new KPIs/metrics that would really make an impact on our understanding of the business. So we'd determine what new we could do and when based on the importance. Now I've got a fantastic dashboard but it took awhile to get here.

Hopefully that helps a bit,




## Answer 8244

- posted by: [Rich](https://stackexchange.com/users/-1/1501-rich) on 2010-02-19
- score: 1

<p>Howie,
David Skok recently authored a <a href="http://www.forentrepreneurs.com/saas-metrics/" rel="nofollow">very detailed blog post</a> about this exact topic as it relates to SaaS companies.  Even if you're not starting an SaaS business, it is worth your time to read through it.</p>



## Answer 7370

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-01-31
- score: 0

<p>For our software startup we use two tools to cover our needs.  We did start out with Google Analytics, but found that it didn't answer the technical questions as well as we wanted and didn't give us enough specifics on the business interactions.  </p>

<p>As with most business intelligence tools, it's essential to not get distracted by the flashing lights and pretty colors but instead keep challenging yourself to demonstrate that the tool is telling you something you didn't know <em>and</em> can act on in a way that will make a difference.  If not, you're just having fun and wasting time.</p>

<p><strong>Technical Web Site Stats</strong>  </p>

<p>For the technical side we use an application that processes the log files of the web server.  There are some downsides to this approach (notably it can be more challenging to filter out spiders and bots) but you get a more complete view than one that's strictly client side because we can see information on hits that don't run scripts.  For us this is particularly important because we want to track in some detail downloads of our software installation file and hits to a few other things in scenarios GA wouldn't count.  Finally, we like that our data is consistent and updated quickly - we got into this after starting with GA and noting a range of discrepancies we couldn't explain including when historical data would change without apparent cause.</p>

<p>In our case, our hosting provider supplied a license to SmarterStats which, after we evaluated several other options, we decided to use and have been pretty happy with. </p>

<p><strong>Business Web Stats</strong></p>

<p>For the business / sales side we have taken a completely different approach.  We use a SaaS product called <a href="http://www.getleadspy.com/" rel="nofollow" title="Lead Spy">LeadSpy</a> that was easy to integrate into our web site (about on par with GA) and provides us very specific information that lets us track from lead source (e.g. advertisement or other web site) to goals to sales.  It would probably be unwieldy if we were a large company with thousands of unique visitors per day, but for a more normal scale it provides outstanding insight into what channels aren't just passing you traffic but <strong>are passing you real business</strong>.  It's made us much more bold about investing in advertising because we can really assess what is working and what isn't, and do it soon enough to react.</p>



## Answer 7381

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-31
- score: 0

<p>Howie, I think you have it backwards. As best I can understand your distinction between "web-specific" and "business-specific", they're both actions taken on your company's website, but one kind is a horizontal metric like page views, and the other kind is 'specific to your business' like buying your product.</p>

<p>All good current systems can do both. The difference lies with the man behind the screen, i.e. how the analytics guy configures Google Analytics. GA is very extensible and can track just about anything; read up on "Goals", <a href="http://www.google.com/support/googleanalytics/bin/answer.py?hl=en&amp;answer=55521" rel="nofollow">virtual pageviews</a> and link tagging in GA. </p>

<p>The way I see it, Google Analytics is the current world champion of web analytics for startups, but the battlefield is changing. There are 2 new directions being offered up:</p>

<ul>
<li>More real-time than GA (<a href="http://www.getclicky.com/" rel="nofollow">Getclicky</a>)</li>
<li>Analytics more set in context of business goals, more optimized for action-able results out of the box (by combining metrics with a vision of "what is important"). (<a href="http://www.kissmetrics.com/" rel="nofollow">Kissmetrics</a>, Jason Cohen's <a href="http://www.simplestartuptools.com/" rel="nofollow">LeadSpy</a>)</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
