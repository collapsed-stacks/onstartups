## Free tools to help increase conversion rate of a site?

- posted by: [Genadinik](https://stackexchange.com/users/-1/8929-genadinik) on 2012-02-01
- tagged: `conversion`, `ab-testing`
- score: 2

I am at a stage of growing a site where it is in open alpha, and there are about 50 people coming to the site per day or so...without any solicitation. They come from stumbleupon, google, and a few scattered places across the web.

What I am trying to do now is increase the conversion rates of pages. My site is a UGC site and it is important that the users register and contribute in the community. 

What software out there (preferably free) can I try to help me understand why users are not signing up?

Thanks!


## Answer 35584

- posted by: [Jay Neely](https://stackexchange.com/users/-1/1801-jay-neely) on 2012-02-02
- score: 3

<p><a href="http://www.optimizely.com/" rel="nofollow">Optimizely</a> (cheap), <a href="http://visualwebsiteoptimizer.com/" rel="nofollow">Visual Website Optimizer</a> (free trial), and <a href="http://www.google.com/websiteoptimizer" rel="nofollow">Google Website Optimizer</a> (free) will all let you do A/B testing if you want to see how different versions of a particular page element (or even totally different page layouts) affect conversion.</p>

<p>Outside of A/B testing, digging into your analytics can provide many insights as to why people are leaving your site. Three things I'd look at:</p>

<ul>
<li>Based on the referring site link or search keywords, what is the visitor looking for? Is the page they're landing on providing them that?</li>
<li>If visitors are staying at least long enough to view a few pages, which pages are causing them to leave (top exit pages) -- is there something on these pages causing them to leave / lose interest? Are the pages calling for an action too difficult / too confusing? Are they simply reaching a dead end where there's not a clear next action?</li>
<li>How many visitors are reaching the signup page at all? How long are they spending on it? If they're leaving immediately, your signup is too difficult. If they're leaving after a bit, they're reaching a point of difficulty or something's triggering hesitance, and you need to figure it out. Try <a href="http://rejoiner.com/" rel="nofollow">Rejoiner</a> to see which forms they're filling out. The ones they're not are likely causing the difficulty.</li>
</ul>

<p>Also, try alternative analytics tools like <a href="http://www.crazyegg.com/overview" rel="nofollow">CrazyEgg</a>, which can provide click heatmaps and scroll heatmaps -- are people not seeing the signup prompt? Are people clicking on a logo or image that doesn't actually link to anything?</p>

<p>Finally, learn from others. <a href="http://www.abtests.com/" rel="nofollow">ABtests.com</a> has many conversion case-studies. As always, your industry / audience has unique considerations, so use these to get ideas and improve what you're initially testing, but make sure you are doing your own testing.</p>

<p><strong>2012 Update:</strong> Another tool I've started using is <a href="https://mixpanel.com/" rel="nofollow">Mixpanel</a> (free up to a certain amount of data per month). They're event tracking analytics; the main way to use this for increasing conversions is through their funnels feature. By defining a series of events (more detailed than page views (e.g. form field clicks, progress through a series of lightbox/modal windows)), you could see exactly which step is where most people are falling out of the funnel.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
