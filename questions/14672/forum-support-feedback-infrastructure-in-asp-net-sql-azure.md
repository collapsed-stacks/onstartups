## Forum/Support/Feedback infrastructure in ASP.NET & SQL Azure?

- posted by: [Igorek](https://stackexchange.com/users/-1/4395-igorek) on 2010-10-02
- tagged: `website`, `customer-support`
- score: 0

I'd like to put up a support forum/feedback/message-board feature on my site to support the upcoming preview of our application as well as perhaps host future discussions on related topics.

I'm using ASP.NET Forms Authentication against SQL Azure to authenticate users against the application itself and was hoping to find such a software hopefully in a "modern" shell that integrates with Forms Authentication so that users do not have to login twice or maintain two accounts.

Pricing is definitely a factor and I hope to find something that's either free or that has a smaller one-time fee.

So far I know of Yaf.net (Yet Another Forum) that's open source, supports Forms Authentication and is in ASP.NET but it seems a little "old"... not modern enough?  Any suggestions that would look more Web 2.0?


Thanks!

Igor


## Answer 20594

- posted by: [rbp](https://stackexchange.com/users/-1/7971-rbp) on 2011-02-22
- score: 1

i recommend GetSatisfaction.com which has "FastPass" single signon for .NET

there are instructions for .NET integration at the bottom of this page


http://getsatisfaction.com/developers/fastpass-implementation



## Answer 14674

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-10-02
- score: 0

<p>I'd love a solid answer to this one as well. AFAIK the open source forum scene on .NET is just much less developed than, say, PHP.</p>

<p>I only know of <a href="http://yetanotherforum.net/" rel="nofollow">YAF.net</a> and <a href="http://telligent.com/community/" rel="nofollow">Telligent Community Server</a>. One comment, I think you must accept a certain investment into customizing the HTML &amp; CSS to get the right look for your needs. The good news is that you can generally find people to do this for you.</p>

<p>The 'Web 2.0' option would be to purchase a hosted forum and blog, i.e. forums.company.com and blog.company.com . There are many providers -- Vanilla Forums, UserVoice, GetSatisfaction and more. The downside is no synchronization of logins.</p>



## Answer 14755

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-10-04
- score: 0

Another commercial option that I've used in the past is from InstantASP - http://instantasp.co.uk .  It's a small company but they've been around a while and keep plugging away.  It's got a number of modern features, is ASP.NET and SQL Server Based (doubt it supports Azure however).  I know a few folks that have integrated that forum into their existing authentication infrastructure.


## Answer 20396

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-02-17
- score: 0

Some choices to look at:
SmarterTools.com (has a product for tickets)
Assistly.com subscription product, but good for tickets
ZenDesk (Tickets and forums)
Interspire Knowledge Manager (PHP, but solid)

KAYAKO - my favorite.
They offer hosted and non-hosted... I think its worth buying the lic, but try it hosted first.
They combine tickets, forums, and chat. 


If you are on a poor mans budget, id sugget:
 1. Livezilla for customer chat (FREE)
 2. Question2Answer.org for forums (similar to what we use here)
 3. Cerb5 HelpDesk (Free for startups, you have to email them for a lic)  For tickets and cases.




kayako combines the top 3 products in a very elegant system, but it does cost money. 



## Answer 20418

- posted by: [Ivan Zlatev](https://stackexchange.com/users/-1/6642-ivan-zlatev) on 2011-02-18
- score: 0

I am actually in the same boat as you in the long run as I too am interested in integrating a simple forum/discussion solution into my work in progress ASP.NET MVC web site. I can't go with GetSatisfaction or UserVoice because they don't offer me internationalization nor localization. My personal preliminary requirements are:

 1. Easy to install and configure, maintain, update.
 2. Very simplistic rather than a full blown forum.
 3. Single sign on with my existing web site.
 4. Easy visual integration with my existing web site. Best if I can embed it directly inside a ASP.NET view.

However after some research I have yet to see something in ASP.NET that does what I need. On the other hand there are gazillion free PHP forums of all sorts and kinds. 

So I have personally given up on ASP.NET for a forum and I am considering using a PHP forum instead. Based again on preliminary research it appears to be technically doable to implement PHP <-- ASP.NET single sign on especially if one is using ASP.NET Forms Cookie authentication and the PHP and ASP.NET are on the same domain (e.g. forum.domain.com or domain.com/forum). Also as far as I understand the PHP app can be kept separately from the ASP.NET on disk (so things won't get messy) by the use of virtual directories to "unite" them.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
