## Major expenses of a web-based startup?

- posted by: [im_chc](https://stackexchange.com/users/-1/12689-im-chc) on 2011-08-15
- tagged: `website`, `planning`
- score: 5

I have an idea of a social web-app and am seriously consider to have my own startup on that.

So I would like to ask, what are the major expenses of running a web-site?
Specifically, what are the stuffs I need to spend on before I am able to reach the point where the user base is large enough?

(Or to rephrase it: if the web app does not have a lot of users yet, is it possible for it to have virtually no expenese at all?)

I am the one who does the programming (and might have one more founder to do it too), so the development costs should be mainly in terms of time.

---

Also, I have several "sub-questions":

 1. Is it possible to hire as few as 0-3 employees - at least at the beginning? I would like to minimize the expense - as few as possible...

 2. I know there are a few unavoidable types of expenses, like hosting, graphic design etc. Any more?

Ideally, if the idea etc works as expected, everyone around the globe should be using it... so I would say that certain types of resources would definitely be needed, e.g. customer services, cost on scaling the infrastructure etc.

Please help, and thanks to you all!



## Answer 28830

- posted by: [Alain Raynaud](https://stackexchange.com/users/-1/502-alain-raynaud) on 2011-08-15
- score: 4

By far, the main expense is paying developers. Most sites can be coded by one person or two at most, so don't start with a plan that shows 3 developers unless you were an R&D manager in a previous life and know what you are doing.

That's it. The monthly hosting can be had for less than $50/month, so I wouldn't count that as a major expense. Most people I know with ideas for a web site struggle to find a developer. Everything else is easy in comparison.


## Answer 28832

- posted by: [Steve Wortham](https://stackexchange.com/users/-1/1791-steve-wortham) on 2011-08-15
- score: 4

<p>This is going to vary widely but if you're like me and are essentially doing all the work yourself then your expenses could be very low.  </p>

<p>In my case, my greatest single expense is web hosting.  I'm paying $270/month for a dedicated dual-core web server with Windows Server 2008 and SQL.  I went the dedicated route because I'm  doing a few automated tasks with the web server that a shared hosting provider wouldn't allow.  Plus the performance is nice to have. But you could easily pay less with shared hosting, or a virtual dedicated hosting service.</p>

<p>Then there's advertising.  Of course if you're offering something truly remarkable, the website can spread by word of mouth and you may not need to advertise.  I have one product that doesn't really need advertising, and another that does.</p>

<p>My monthly expenses are something like this:</p>

<ul>
<li>web hosting - $270</li>
<li>advertising - $100</li>
<li>merchant account fee - $20</li>
</ul>

<p>Then throw in the occasional big purchases like enterprise software and such.  I've spent over $2,000 on software during the past two years.  And I did hire a lawyer to write some agreements for one of my sites which had more legal complexities than other sites I've done.  That was about $1,500.  Beyond that, there hasn't been much.  Like you said, when you're a one-man show the biggest investment is time.</p>

<p>My plan is to do all the work myself for as long as I can.  I want the company to be profitable and healthy before even considering hiring other developers.  The stakes are higher once you start hiring.  And as Alain stated, payroll will be the greatest expense by far.</p>

<hr>

<p><strong>Cloud Hosting</strong></p>

<p>On the subject of web hosting, I just wanted to make a few points and suggest a few things for you to look into.  As we discussed in the comments, it sounds like you're attempting to build a website that could potentially see a lot of traffic so it'd be good to choose something like Windows Azure, Amazon EC2, or Google App Engine.  There's a discussion <a href="http://programmers.stackexchange.com/questions/64727/windows-azure-vs-amazon-ec2-vs-google-app-engine">here</a> about these 3 services.  The pricing is very competitive with these services and they make a lot of sense for high-traffic websites.</p>

<p><strong>Efficiency</strong></p>

<p>You have to keep in mind that these services charge based on compute time and server resources.  So to save cost, I think it's important to start with an efficient server-side language and database engine.  Twitter made the mistake of building their site with Ruby, which is one of the slower web-friendly languages in existence.  C# and Java are compiled languages and either one would be a better choice, depending on what you're more familiar with.  If you're curious, <a href="http://shootout.alioth.debian.org/u32q/benchmark.php?test=nbody&amp;lang=all" rel="nofollow">here's a list of benchmarking results</a> showing the raw number-crunching horsepower of various popular languages.  And here's a slightly more realistic <a href="http://shootout.alioth.debian.org/u64q/performance.php?test=knucleotide" rel="nofollow">benchmark heavy on string manipulation</a>.   Java is 67X faster than Ruby in the first benchmark and 14X faster in the second.   Of course most of the time the bottleneck is actually going to be on the database side of things and the two most popular choices out there (Microsoft SQL and MySQL) are very well optimized.  But when you're concerned about scalability, even the web framework matters.  So yeah, don't use Ruby.</p>

<p><strong>Content Delivery Network</strong></p>

<p>And then you should host static content (images, css, js) with a CDN (content delivery network) like <a href="http://aws.amazon.com/cloudfront/" rel="nofollow">Amazon CloudFront</a>.  They are ridiculously cheap.  I was paying them around 10 cents a month.  Of course my sites were only getting around 500 visits a day collectively at the time, but still it's a bargain.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
