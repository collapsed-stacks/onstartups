## Collect usage metrics of software

- posted by: [Sebastian Hoitz](https://stackexchange.com/users/-1/313-sebastian-hoitz) on 2011-05-24
- tagged: `metrics`, `data`, `collection`
- score: 2

What would be the best way to collect usage metrics of a SaaS software?

I want to collect something like logins, clicks and time spent in my software.
Are there existing services out there that allow such data collection? Or would you advise to write our own custom data analysis?


## Answer 25394

- posted by: [tinny](https://stackexchange.com/users/-1/10522-tinny) on 2011-05-24
- score: 3

<p>Google analytics is a pretty standard approach. Just a small bit of javascript on your web pages. <a href="http://www.google.com/analytics/" rel="nofollow">http://www.google.com/analytics/</a></p>

<p>Also has features to help you track usage against marketing campaigns.</p>



## Answer 25402

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2011-05-24
- score: 1

If you are writing the code to your saas application(s) I don't see why you wouldn't write your own over time.  

Start off with simple data provided by google - but that will probably be limited to page views - and likely won't be able to tell you more detailed information only available from your database and other servers.  




## Answer 25406

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-05-24
- score: 1

<p>Here is a list of possibilities:</p>

<ul>
<li>I like Google Analytics (GA) for the price (free). One drawback is that it updates daily, not in realtime.</li>
<li><a href="http://statcounter.com" rel="nofollow">StatCounter</a> may be what you want if you want to tag certain actions on your website and you are willing to do a little programming.</li>
<li>You may also what to look at <a href="http://crazyegg.com" rel="nofollow">Crazy Egg</a> for heat maps that give you a visual of where visitors are clicking.</li>
<li><a href="http://kissmetrics.com" rel="nofollow">Kissmetrics</a> is put out by the same company as Crazy Egg. It is more of a direct competitor to GA, arguably better as it works in realtime.</li>
<li><a href="http://getclicky.com" rel="nofollow">Clicky</a> is another realtime web analytics tool.</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
