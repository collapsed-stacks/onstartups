## My startup built on ASP.NET/SQL Server 2008 stack. What are my hosting options? Costs?

- posted by: [Joe A](https://stackexchange.com/users/-1/60-joe-a) on 2009-11-07
- tagged: `infrastructure`, `launch`, `metrics`
- score: 5

I'm in the final stages of development on my startup. The site is built in ASP.NET using SQL Server 2008. It is a consumer-focused website that I intend to concept-test next month and gather feedback with a small group of users (100-200), then do a full launch in January. I'm hosting on a cheap shared hosting plan now, but soon after launch I'm hoping to draw 100,000+ users per day to the site.

What's a good scaling strategy, i.e. from shared hosting to managed hosting or cloud, etc. As assuming the metrics above + say 100kb to 1mb per user per site visit, what would the best approach be, who would you recommend, and what would the costs be?



## Answer 3301

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2009-11-08
- score: 7

<p>a) <strong>Run your first user tests from a VPS.</strong> Head over to serverfault.com and stackoverflow.com , and find the previously asked questions about best Windows VPS + SQLServer hosting providers.</p>

<p>b) Head over to <strong><a href="http://browsermob.com/" rel="nofollow">BrowserMob</a> or a similar scalability testing service</strong>, and run tests against your site to get a ballpark figure for how many users it can handle. Be sure to run a realistic test which pulls data from your database.</p>

<p>c) When the VPS gets too small, do you then go to a <strong>dedicated server first, or direct to cloud computing?</strong> This is debatable, there are fair arguments for both. I guess it will depend on your growth expectations, i.e. how long you see that dedicated server lasting, and how sensitive you are to server downtime of your single server.</p>

<p>If you choose to run on a single server / 1-3 servers, then head over to the <a href="http://www.webhostingtalk.com/" rel="nofollow">webhostingtalk.com forums</a>, and find recommendations for a good host. My preference would be for a host that offers:</p>

<ul>
<li>a firewall or a network intrusion detection system in front if your server.</li>
<li>renting servers, not co-locating your own hardware (if you colocate you have to provide <strong>all</strong> hardware replacement yourself).</li>
<li>a good remote management solution (KVM-over-IP, self-service portal).</li>
<li>optionally, more expensive but depending on your own skill set possibly better, a fully managed service.</li>
</ul>

<p>d) Ultimately I think most people will want to run their <strong>webapps on a cloud computing</strong> service provider.</p>

<p>Amazon is a poor choice for .NET right now, as they have <strong>not</strong> supported Windows 2008 for years, and there is <strong>no date</strong> on when they will support Win 2008 / 2008 R2. (I believe they are working on it, but their Windows track record so far is poor.)</p>

<p><strong><a href="http://www.microsoft.com/windowsazure/windowsazure/" rel="nofollow">Windows Azure</a> looks awesome</strong>, and the more I have read about it, the more it appears that Microsoft is deadly serious on building a strong presence in cloud computing. <a href="http://www.rackspacecloud.com/" rel="nofollow">Rackspace Cloud</a> looks fine too, and could be a better choice right now since Azure is still in beta. Longer-term I think Azures roadmap looks more impressive.</p>

<blockquote>
  <p>soon after launch I'm hoping to draw 100,000+ users per day</p>
</blockquote>

<p>100,000 unique visitors per day, so 600,000 - 2,000,000 page impressions per day? That sounds very high to me, but of course I don't know what your app is about. But if you're realistically going to get that kind of traffic soon after launch, then head for cloud computing hosting ASAP, maybe even during your beta test period.</p>

<p><strong>Update:</strong> I forgot to mention Microsoft Bizspark, but luckily Bob Walsh wrote a good answer about it; see his answer. You want BizSpark if you co-locate your own hardware, or if you use a web host who is a member of the BizSpark programme. Windows Azure already has the license fees included in the compute cost; I don't think there is a discount on Azure for BizSpark startups.</p>



## Answer 3302

- posted by: [Bob Walsh](https://stackexchange.com/users/-1/346-bob-walsh) on 2009-11-08
- score: 4

<p>Joe - Since you're building on Microsoft's stack, definitely check out <a href="http://www.microsoft.com/BizSpark" rel="nofollow">Microsoft BizSpark</a> - if you're a startup, less than 3 years old, &lt; $1m revenue you get development/testing and production licenses for team foundation, Sequel Server, IIS., etc. free. Furthermore, certain Hosting companies - such as Rackspace - will cut you a deal. I'm not sure if RackSpace has to sponsor you, but if they don't, I can. (for my sins, I've ended up being the single most active BizSpark Partner - pushing 400 startups). </p>

<p>[Typed on my MacBook Pro],
Cheers,
Bob </p>



## Answer 3300

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2009-11-08
- score: 1

I colocate my servers...  There are lots of hosts out there, but with colocation your costs start getting cheap right away.  The problem is that you need to put in a good system of redundancy, mutual backups, etc...  so you need to have some level of technical knowledge.  I pay about $100/month for colocation of my boxes with 3TB monthly bandwidth (CIHost).

If I had to do it again from scratch today, I would look at colocation and Amazon's EC2 ( http://aws.amazon.com/ec2/ ).  On paper, their offering seems very nice, very cost effective.  You don't have to worry about hardware costs or failures, which is a big plus.  It's easier to call someone when the thing goes down than to have to drop what you are doing and fix it yourself.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
