## How important is the server location?

- posted by: [jitbit](https://stackexchange.com/users/-1/4407-jitbit) on 2011-04-27
- tagged: `hosting`, `server`, `ux`
- score: 7

My small software company - [Jitbit][1] - currently uses servers located in the US (for both our website and SAAS solutions) because the majority of our customers is there.

But I consider moving to a dedicated server in Netherlands (LeaseWeb provider). Or is it a bad idea? Should I be worried? We offer **web-based** solutions, so another 100ms delay in latency should not be not crucial right? (unlike, say, in gaming industry, where extra 100ms can ruin your experience...)

Thanks!


  [1]: http://www.jitbit.com/


## Answer 24103

- posted by: [edralph](https://stackexchange.com/users/-1/9362-edralph) on 2011-04-27
- score: 13

<p><strong>Performance matters</strong>...  wow.  I know I'm going to be surprised by the variety of responses here.  A regular eCommerce site benefits hugely from rapid page loads and response times, with visitors exiting the site much more readily when the site is slow.  For an SaaS provider, I would have thought that performance is even more of an issue.  When I select SaaS solutions for my business performance is one of the biggest considerations - a brilliant system that does everything you want, but is just a bit slow, is almost good enough reason to not go with that provider.  Just trying the sales-end of your website isn't enough to judge performance - the SaaS solution is much more likely to be database-driven and serving more data - so page load times are going to be more of an issue.  When I select an SaaS solution for the business which may have, lets say, 100 users, I have to live with the consequences of that site being slow and unwieldy: potentially I'll have 100 people complaining at me.  Site speed matters.  @Ross also mentioned the potential impact on SEO - as last year <a href="http://www.mattcutts.com/blog/site-speed/" rel="nofollow">Google introduced site speed into their ranking algorithm</a>.  So faster website may mean better rankings as well.  Marvellous.</p>

<p><strong>Measure the performance from an end-users point of view</strong>... For our eCommerce website we use a product from Gomez Inc called <a href="http://www.gomez.com/products-solutions/products/web-performance-management/browser-based-real-user-monitoring/" rel="nofollow">Gomez Actual Experience</a> which gives us the page response times and load times for every visit to key pages on my website.  These numbers differ from regular backbone monitoring solutions in that you get data directly from the end-users visiting your site.  If it took 1.24s for the page to load in front of them, that is the number that is reported.  The data is segmentable by region, browser type, etc. and is a great way of monitoring how well you are serving your customers.  For SaaS, I would think this type of monitoring is key to understanding whether your customers are getting the page response times you are expecting them to.  <strong>Edit:</strong> Since posting this answer Google has released page load tracking in Google Analytics.  Fantastic.  Now you will be able to segment your page load times by any of the variables in Google Analytics and really get a good idea of how page load times affect the user experience.  <a href="http://analytics.blogspot.com/2011/05/measure-page-load-time-with-site-speed.html" rel="nofollow">Official Google blog post here</a>.</p>

<p><strong>Global location still matters if you can afford CDN</strong>... <a href="http://www.akamai.com/" rel="nofollow">Akamai</a>, <a href="http://www.limelight.com/" rel="nofollow">Limelight</a> and other CDNs make the physical location of your host matter a little less.  However, if your website or SaaS solution is highly dynamic (probably) and database dependent then there is reduced scope for caching which is the CDN's primary mode of delivering content faster.  Yes they have solutions that help get around that, but if you are serving a page that needs real-time data from a database from one side of the world to the other side of the world then the CDN is not going to magically eliminate the latency.</p>

<p><strong>I'd stay where my customers are</strong>... Unless there are some really compelling reasons to move other than cost, I'd probably keep my servers where the majority of my customers are.  Perhaps you are able to segment your offering so that your European customers can use a datacenter in the Netherlands and your US customers can still use the US.  The only issue with that is global companies that have offices in the US and Europe, and want to use a single connected system.</p>

<p><strong>If you do move, test thoroughly</strong>... Hosting centers will usually let you have access to a machine on their network to do some latency tests - and you can use <a href="http://www.lookinglass.org/" rel="nofollow">'Looking Glass'</a> services from other ISPs located near your customers to test what the latency is like from ISP to datacenter.  Furthermore I'd be keen to test the SaaS solution <em>in situ</em> and test the performance from your customer location.  Spend the extra money on the testing from the Netherlands before cancelling your contract with your main hosting center; the last thing you want is to have migrated your servers only to find that your customers are now complaining that their SaaS solution is now running slower, and threatening to leave unless it speeds up.</p>

<p>Hope that helps.</p>



## Answer 24101

- posted by: [Jeremy McGee](https://stackexchange.com/users/-1/1152-jeremy-mcgee) on 2011-04-27
- score: 1

Nice site!

I think you're right to not be worried about performance: I've just tried this from the UK and all seems just fine. If and when you grow to the point where performance turns into an issue then the CDN providers out there can help mitigate this.

More critical is perhaps the legal framework of where you host. In particular privacy laws differ in the US from Europe, as does the attitude of ISPs to protecting servers and data from law enforcement. 

This might well be an issue for the hosted CRM software, for instance -- here in the UK customer data of this kind really should be hosted in Europe as it could be considered personal data. You'll probably want help from a lawyer on this.


## Answer 24933

- posted by: [jtauber](https://stackexchange.com/users/-1/3994-jtauber) on 2011-05-14
- score: 1

Performance is important but so are the data protection / privacy laws in various countries. While many sites we develop for clients outside the US still host in the US; we have had some clients who have required hosting in the EU due to data protection / privacy laws applicable to their business.


## Answer 24107

- posted by: [Brian Karas](https://stackexchange.com/users/-1/8465-brian-karas) on 2011-04-27
- score: 0

Why are you looking to move to a server in the Netherlands?  Is there some financial incentive to do so?  It seems that you are in the UK, and most of your customers are in the US, so I don't get the rationale for a server in the Netherlands.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
