## Are there any sites that measure the page response speed of various hosting companies?

- posted by: [Mark Rogers](https://stackexchange.com/users/-1/5934-mark-rogers) on 2011-01-15
- tagged: `website`, `web`, `hosting`
- score: 1

I'm looking for the equivalent of consumer reports for hosting companies. But I would be happy with any neutral data comparing one site to another.

Does anyone have any links to data the speed of various popular hosting sites versus one another?



## Answer 19019

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-15
- score: 2

<p><strong>I don't think that exists; at least I have been looking but never found anything that fits 100%.</strong></p>

<p>Netcraft runs a series of benchmark and data gathering runs against a large'ish population of servers. One part of this gives <a href="http://uptime.netcraft.com/perf/reports/Hosters" rel="nofollow">uptime and performance numbers</a>, but this is hardly descriptive of all hosts on the Internet. Maybe Netcraft could produce something close to what you're looking for.</p>

<p><a href="http://www.webpagetest.org/" rel="nofollow">WebPageTest.org</a> is a fantastic site, which enables you to test the performance of a live website from a number of locations around the world. But this is a one-webpage-at-a-time test tool. The gentleman behind the site had a good <a href="http://calendar.perfplanet.com/2010/the-state-of-web-performance-optimization-2010/" rel="nofollow">2010 web performance review dataset</a>, but this is aggregated for the Internet at large, not broken down on each ISP.</p>

<blockquote>
  <p>data the speed of various popular hosting sites versus one another</p>
</blockquote>

<p>Just to be clear, the performance of the ISP is only one (actually smaller) part of the overall speed -- the <a href="http://stevesouders.com/hpws/" rel="nofollow">application and frontend (HTML, CSS &amp; JS) matter more</a>.</p>

<p><strong>Update 17th Jan:</strong> An additional note -- there are plenty of companies who have the technology to obtain latency metrics for a large collection of web hosting providers. Gomez, Keystone, etc as examples of companies coming from the uptime monitoring service angle, and LoadStorm and BrowserMob as examples of companies coming from the load testing side. You could consider working with some of these companies to obtain that kind of data. And do consider the web hosting providers too -- running a load test against a hosting provider who hasn't agreed to this arguably constitutes a denial of service attack</p>



## Answer 19067

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-01-17
- score: 1

if you want serious tracking check into Browsermob.com.  As for speeds, you really need to make sure that you get guaranteed so many MBPS.   



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
