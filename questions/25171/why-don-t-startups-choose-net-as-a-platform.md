## Why don't startups choose .Net as a platform?

- posted by: [7wp](https://stackexchange.com/users/-1/10600-7wp) on 2011-05-19
- tagged: `technology`, `platforms`
- score: 30

I was reading the article about "[Why Startups Could Use .NET, But Don’t][1]".   Essentially the article says that it comes down to culture.  

I don't want to start a holy war, I just want to know the core reason start-ups would be against using .NET could it really because of culture?  

I mean StackExchange was built on .Net right from the beginning, which is now one of the top 200 sites in the world with millions of visitors.  Obviously this proves .Net is a very capable platform.   I would be curious to know if S.E. would have had the same success or challenges if it had been built with other technologies.

If you are a start-up and you're against using .Net, what's your reason for dismissing it?


  [1]: http://www.piehead.com/blog/2011/05/why-startups-could-use-net-but-don%E2%80%99t


## Answer 25182

- posted by: [Bryan Migliorisi](https://stackexchange.com/users/-1/8352-bryan-migliorisi) on 2011-05-19
- score: 30

There is a stigma attached to anything Microsoft.  As the article says, its a cultural thing.

Please remember that 

 - the C# compiler is **free** just like PHP, Ruby, Java, or Python are.  
 - Visual Studio has free versions that are not as featurefull as the others, but are still **free**
 - You do not *need* to run ASP.NET on Windows.  Mono allows you to run it on any flavor of *nix, including OSX
 - Windows Web Server 2008 is $469 which, while isnt free, certainly isnt terribly expensive.
 - Amazon EC2 powered Windows server's cost as low as $36/month which is absolutely affordable
 - There is a huge community around the technology


## Answer 25172

- posted by: [Sean](https://stackexchange.com/users/-1/6610-sean) on 2011-05-19
- score: 24

Although my current startup DOES use .NET (because we're all mostly MSFT people by day), a previous one did not.

The main reason was cost.

Finding a reasonably priced slice/virtual from a good provider is very tough.

If you decide to buy a server, you have to make special decisions as to what flavor of hardware and software you buy/install.

Server 2008 is pretty expensive unless you stay with one of the lower options.

SQL Server 2008 is VERY expensive unless you stay with Express ($free).  Express has limitations on the memory and database size and CPU supported.

Pre-Azure, there was really no "cloud" for .NET/MSFT hosting.  And I'd say that Azure sucks (even as a MSFT partner, I say it sucks).  The development model for it blows.  But that's a different subject.

Another good (likely non onstartups question) is how does a startup that wants to use .NE/MSFT technologies limit their licensing and capital expenditures.


## Answer 25179

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-05-19
- score: 17

There is another side to this. Not everyone is so much deciding against .NET as they are deciding in favor of another platform. I am not anti-.NET but my background and my contacts are on other platforms. For those who grew up with PHP or Rails or Java or something else, it might not be a conscious choice against .NET but rather just a lack of considering it.


## Answer 25207

- posted by: [vartec](https://stackexchange.com/users/-1/10635-vartec) on 2011-05-20
- score: 17

The main reason: **Vendor lock-in**

Choosing .NET means vendor lock-in with Microsoft, both for development as for servers. Mono is just not compatible enough to be drop in replacement.

Server market is dominated by Linux. If you're startup interested in cloud hosting, there are plethora of Linux based ones, and only a few Windows ones. And if some platform offers both, Windows is more expensive (for example with Amazon EC2 standard instances its +50% to the price). Of course MS is trying to address that with Azure. But that means you'd be getting even deeper into vendor lock-in.

On the other hand, if you choose different technology, you have your options wide open. You can run Python, Ruby or even PHP on about any web server there is. You can develop using any tool stack you like. On any developer OS.  


## Answer 25173

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2011-05-19
- score: 12

- Licensing costs
- Preference for non MS platforms and technologies
- Anti-Microsoft sentiments in some developer communities


I'll add one other thing that is somewhat related to the others - MS is a technology that is mostly shunned in colleges - thus the linux stack and OSes are more comfortable and thus the development tools of choice for the recent grads are not MS based.  

Many startups are skewed to younger founders and employees, thus another reason for the bias in startups.  

(The bizspark and other programs were a way for MS to address some of the issues.  They finally saw the danger of the open source development stack.

Ballmer's "Developers developers developers developers developers developers developers" rant/speech becomes void if you lose developers.)

**NOTE**

**Given the nonsense arguments in the comments and in the answers I do have to point out that the choice of OS and development tools has almost NOTHING to do with the success of the company or product.  As long as there is no complete mismatch of technologies then the overwhelming considerations for success or failure are the people, the execution of the idea and the relationships with customers.  I have rarely, if ever, seen a project fail because of a choice of technology stack.
I assumed the original question was not meant to start a religious war, and I am giving it the benefit of the doubt.  Unfortunately it seems to be headed that way.**


## Answer 25196

- posted by: [jtauber](https://stackexchange.com/users/-1/3994-jtauber) on 2011-05-20
- score: 7

My guess is that most startups that use .NET were founded by people that had previously used Microsoft technologies in a larger enterprise setting.

The younger generation of startup founders, without enterprise software experience, are probably using the same technologies for their startups that they used as hobbyists: Rails, Django, Python, Linux, MySQL, Postgres.




## Answer 25376

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2011-05-24
- score: 7

Your question assumes startups (or most of them) do not choose .NET as their technology stack and this is incorrect. 

While it might be true that most startups that visit this site might not be using .NET as their technology stack, it is also true that the reason is not cost, or culture, or dislike of Microsoft but instead the fact that most startups will use whatever they have experience with, whatever they have immediate access to, because that is what will help them get their product out sooner than later.

The idea that startups do not use the Microsoft stack because of the high cost makes no-sense. Microsoft has always offered ways for starting companies to get their development tools, and server licenses at a very low cost, that is a fact. 

The vendor lock-in argument is also not valid, because the same apply to any technology stack you choose to use. While some technology stacks might not have a license cost, they all will cost you money, in the way of support, learning curve, difficulty to find experienced people, etc... 

My personal opinion about "what technology stack to use for my startup" is, use whatever helps you get your product out the door quickly, nothing else. The technology behind your product is not what will make your product either a success or a failure, period.




## Answer 25307

- posted by: [jitbit](https://stackexchange.com/users/-1/4407-jitbit) on 2011-05-22
- score: 5

Startups DO use .NET, actually. I know quite a few .NET-based startups and I even co-founded several NET-based startups, including my main software business (in my profile).

The reasons we chose (and keep choosing) NET over the alternatives are:

 1. The "Bizspark" program. Registering is free and it gives you all the MS products
    **free of charge**. SQL Server (all editions), Visual Studio, Windows OS
    etc etc. So I kinda don't get the "costs" argument going on here
 2. Visual Studio is by far the best IDE on the market
 3. The .NET team at Microsoft is great and kinda "non-Microsoft". I know a couple of
    guys working there, and it's the most agile and innovative department (btw, Bing division is also heard to be a "non-MS" dep).
 4. Easy to hire ppl, easy to find info (just look at stackoverflow - "c#" tag is **the** most popular tag)


## Answer 25181

- posted by: [thaBadDawg](https://stackexchange.com/users/-1/10579-thabaddawg) on 2011-05-19
- score: 3

You have also got to consider the available workforce for your development team. One of the reasons MySpace failed where Facebook became wildly successful is tied to the amount of talent that either company could find for developing the product. Consider the following:

 1. .Net development tool cost (minimum $500 a seat) vs PHP/Python/Ruby development tool cost (Usually free)
 2. A quality .Net developer will be somewhere in the $60k-$90k realms vs A quality PHP developer will be around $50k-$70k.
 3. It's hard to say exactly how the breakdown goes, but most employment specialists I've talked to say that you have 2 or 3 PHP guys to every 1 .Net guy.
 4. Because PHP has been free from the beginning (only recently is MS starting to get into the free realm) you have people who have been working on PHP or Python or Ruby since they got into programming, but you had to go out of your way to either beg/borrow/steal a copy of Visual Studio so you could start working on the MS platform. Most .Net developers haven't been doing it consistently over their whole development career... but most PHP, Python and Ruby developers picked up the stack at the beginning and may have played with other stuff, but always come home to their happy hunting grounds.

In a lot of ways the MS/.Net platform is the very best available tool for the job... if you are willing to pay for it. And let's face it, Facebook, LinkedIn, Wikipedia, and hundreds, if not thousands of other successful programs have come from PHP.




## Answer 25230

- posted by: [Richard Turner](https://stackexchange.com/users/-1/10652-richard-turner) on 2011-05-20
- score: 3

<p>There's a lot of cr@p being posted here about the supposedly huge differential between building a start-up atop Windows vs. *N*X.</p>

<p>This is not necessarily true.</p>

<p>Rackspace virtual machine hosting for Windows instances is $8 per month more compared to (otherwise identical) Red Hat instances. If you want to host a cloud/web-based solution, there are a ton of Windows hosting providers offering everything from shared (@ $2.99 a month) to dedicated hosting (@ $150 a month) and everything inbetween which should allow you to find a solution to fit your needs and budget. Explore some of the options here: <a href="http://www.microsoft.com/web/hosting/home" rel="nofollow">http://www.microsoft.com/web/hosting/home</a>. </p>

<p>Also, take care to do your own research - don't mistake the ignorance of others as actual reality.</p>

<p>For example, <a href="http://www.microsoft.com/windowsazure/" rel="nofollow">Azure</a> is, increasingly, a really kick-ass infrastructure. The enormous investment Microsoft is putting into this infrastructure &amp; the associated tooling is now really starting to pay off with the introduction of the Azure CDN, eventing &amp; pub-sub delivery network, elastic scalability and availability, etc. And if you wish, you can host .NET, Win32, PHP, Java, Ruby and anything else you can run in Windows within your Azure instances too.</p>

<p>In general, the costs for your hardware, software and licenses are going to be dwarfed by your costs for legal, HR, accounting, travel, marketing, rent, supplies, etc. If they're not, chances are that you're doing it wrong! Buying all your founding members MacBook Pro's so that they can write Ruby/PHP/Perl, for example, is just stupid. </p>

<p>Building a start-up with astronomically high IT costs is only going to lead to ruin, but investing in tools and technologies that reduce your time to market (e.g. Visual Studio) is often money well spent. I've spent a lot of times in Eclipse, NetBeans and XCode recently - they don't even come close to VS when the going gets tough. </p>

<p>Augmenting some of those investments with judicious use of additional free and/or commercial offerings (e.g. Mercurial/GIT, BitBucket/GitHub source private/public hosting, an effective task &amp; bug tracking system, etc.) is wise and effective.</p>

<p>Regarding .NET on non-Microsoft platforms, I have been VERY impressed with Mono of late - particularly the platform-specific bindings to iOS &amp; Android that Miguel &amp; Co. created in the now sadly defunct MonoTouch and MonoDroid (thanks Attachmate ... not!). </p>

<p>I'll be one of <a href="http://www.xamarin.com/" rel="nofollow">Xamarin</a>'s first customers when they ship their new products to replace the now defunct MonoTouch and MonoDroid and I plan on contributing to Mono where I can. Being able to reuse a very significant portion of my code across PC/Laptop, Windows Phone, iOS, Android, Linux, OSX, BSD is a wonderful thing.</p>



## Answer 25233

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-05-20
- score: 3

Turn the question around. Those that have gained enough experience with .NET (Usually a requirement before getting into a software startup is knowing how to program.) are not as likely to venture into startups. Most get this experience on the job working for medium to large businesses. I'd like to see some numbers on what people were doing before their startup. Not that there aren't any people who switched from the corporate world of .NET shops, but this is a huge pool with a small percentage who ever leave.

If you are fresh out of college, worked at a university, have been working with an open source project or were with a previous startup, you're less likely to have used Microsoft products. If you have to spend the time to learn something new, you don't want to take on the additional cost.

A large number of startups are iPhone/Pad app developers; you have to go the Apple route.

Microsoft's BizSpark campaign is trying to combat this by making the cost of entry into their development suite less expensive.


## Answer 25177

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2011-05-19
- score: 1

Mostly due to:

 - Cost of tools (though you can get MSDN sub if you put in enough effort)
 - Lack of solid could solutions and cloud licensing issues
 - Cost of developers, since most are used to Fortune 500 salaries and bennies even VC backed startups can't dole out.


## Answer 25188

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-05-20
- score: 1

From my experience there are pretty clear cut reasons people don't use .NET. There's no doubt that .NET is capable and awesome, scales really well and is a dream to use, however the following issues prevent it from becoming more widespread;

 1. Licencing costs.
 2. Smaller community in comparison to PHP or RoR.
 3. Harder to find a cheap and reliable .NET host as there is for PHP.


## Answer 25204

- posted by: [Dmitri Nesteruk](https://stackexchange.com/users/-1/10634-dmitri-nesteruk) on 2011-05-20
- score: 1

One reason is that IIS is really not that good. Seriously, it's overengineered and fiddly and not as performant as one would like to be. So if we assume that IIS is out of the window, then you suddenly do not need Windows! (Windows is a requirement for IIS.) SQL Server, you say? Seriously, a startup is far more likely to go for a MongoDB+Redis combination which means, again, Windows is not required.

As for the front-end technology, yes, lots of people are doing Rails, but lots of people also think about HTML+JS single-page-AJAX solutions and let's face it, it doesn't really matter what you serve this with, so long as you can keep some RESTful back-end to consume data from.

So the only attraction that remains is the C# language (yes, you can use it with Mono, but still). And I'm not sure if the language alone is enough to sway people towards building .Net-based startups.


## Answer 25198

- posted by: [Jean-Christophe Meillaud](https://stackexchange.com/users/-1/10622-jean-christophe-meillaud) on 2011-05-20
- score: 0

.Net platform is strongly related to Microsoft workstation. On most of the startup i've been, developpers have the choice of their system, and often they prefer to have a powerfull workstation with a linux in it. 
Futhermore startup founders choose technologies based on the cost, and often, they choose a classic [L|M|W]AMP stack wich is powerful and easy to develop. 

Lastly asp .NET is just a me too of php by microsoft, it benefits of huge investment by microsoft, but is still a technology supported mainly by a private company. Developpers of libraries and other stuff for the technology, should not invest to much in it, as they are not sure it the company will continue to support it.

In term of cost, i cannot be more accurate than TheBAdDawg

StackOverflow is the only website i know which is built on ASP.NET, if you think about website buildt with PHP technologies, there are plenty : facebook, wikipedia, wordpress


## Answer 25203

- posted by: [tylerl](https://stackexchange.com/users/-1/10631-tylerl) on 2011-05-20
- score: 0

First of all, lets get one assumption out of the way -- if you're using .NET, then you're using a Microsoft stack. And if you're not using Microsoft, you're not using .NET. No two ways around that one.

So the real question is, "Why don't startups use Microsoft in their server environment?"

Well, the simplest reason is cost. Using Microsoft tools costs more -- it costs more to license, it costs more to maintain, it costs more to scale, it costs more to manage. Microsoft servers are more difficult to automate, they lack some of the more advanced performance tools, they lack the diversity of options found in the Unix world, and dozens more reasons.

As someone who manages server setups for startup companies (both Windows and Linux), I can tell you that the ones who use Windows have more trouble cause *because* they use Windows than the opposite for Linux users.

While .NET is a great platform and C# is a great language, the fact that you can't realistically run it on a Linux server makes it no longer a viable option for savvy developers.




## Answer 32779

- posted by: [B Seven](https://stackexchange.com/users/-1/14522-b-seven) on 2011-11-20
- score: 0

For us, the answer was ***agility***. You don't know if anyone is going to use your product/service. You will make numerous changes to the database schema, classes and functionality of the site. I think the easiest way to deal with the unknown but certain changes is to use Ruby on Rails.

Coming from a background in C#/C++/PHP/Perl, it didn't seem to be a great idea to try a whole new technology. But Ruby on Rails is all the rage in San Francisco, and there is a good reason: it is easy to make changes. It's designed for everything that makes the programmer cringe and for everything that you didn't plan.

Interesting question. And yes, Stack Exchange is awesome.


## Answer 51081

- posted by: [Abel Melquiades Callejo](https://stackexchange.com/users/-1/27776-abel-melquiades-callejo) on 2013-09-24
- score: 0

<p>It's not about the <strong>startup</strong>, It's about the <strong>community</strong>. There's this connotation in computing that <strong>.NET</strong> developers embrace the <em>closed-sourcing philosophy</em>, thus making their software resources not available for everyone. Startups would gladly go into technologies which they know they can get great talents that indulge in a full sharing community.</p>

<p>Yeah, S.E. is a great project and many domains have already implemented it like <em>Answers.onStartUps.com</em> and <em>askubuntu</em> but wouldn't it be nice if SE is a <strong>deploy-anywhere platform</strong> like wikis and wordpress?</p>



## Answer 51113

- posted by: [Jaana Kulmala](https://stackexchange.com/users/-1/26030-jaana-kulmala) on 2013-09-25
- score: 0

<p>Let me offer a bootstrapper's viewpoint. I have previous experience on Java (&lt;10 yrs) and C# (2 yrs), but I still decided to use RoR for my startup.</p>

<p>Why? Productivity and because RoR is de-facto for SaaS. </p>

<p>You'll get things like SaaS authentication and authorization almost out-of-the-box and if there's anything you need tutorials for, they are easy to find and target SaaS-specific problems. You'll get Heroku and tons of different services that are easiest to integrate with RoR apps. </p>

<p>Now, it may be that I have to rewrite my apps with Java or C# later, but I rather spend that investment of time after I know that those apps can earn me money. </p>

<p>When I'm building my MVPs and searching for product-market-fit, I need the extra productivity and flexibility that RoR gives me. I still like Java and C# better than Ruby, but I think we should pick the tools to match what we do - and RoR matches building startups quickly.</p>



## Answer 51455

- posted by: [Mark0978](https://stackexchange.com/users/-1/10006-mark0978) on 2013-10-21
- score: 0

<p>Well, you could point to costs and you'd be right, but that is only a small part of the equation.  If you look at hosting just at rackspace you have $16/month vs $160/month  (If you want SQL Server Web).  That is a factor of 10x right there.  And a 1GB windows server is going to have serious performance issues where a 1GB linux server will support a pretty hefty load.  <a href="http://www.rackspace.com/cloud/servers/" rel="nofollow">Rackspace server pricing</a>.  Bizspark gives you for 3 years what Linux gives you for life.  What about when you need 1000 servers?  And if you use Linode like we do, you save 50% on what Rackspace charges making the cost factor 20x instead of 10x.</p>

<p>Developer tools are worth spending for, but you don't need Visual Studio, unless you are targeting MS products.  We have purchased very good tools for about 25% the price of the Visual Studio that do exactly what we need.</p>

<p>A Linux server outperforms a Windows server on I/O.  We have both types of VMs in our shop, and both types of Hypervisors.  Windows loses on disk I/O on BOTH Hypervisors, and our Linux hosted VMs on openstack are at least 2x faster on I/O.  Linux needs less RAM to do the same things as well.  I'd say more bang for the buck, but I'd get a divide by 0 error on the cost of Linux.</p>

<p><strong>But my primary reason for not using MS products is Trust</strong>.  </p>

<ol>
<li>MS was a founding member of the BSA.  They used the BSA to send out 1000s of overnighted letters, fishing for people to sue.  </li>
<li>They spotted someone (Netscape) that they thought threatened their hegemony (Netscape) and they used underhanded techniques to put them out of business.  They licensed Internet Explorer from Spyglass then gave the product away, denying any money to Spyglass. If you want more details, you can find them on <a href="https://en.wikipedia.org/wiki/Microsoft_litigation#Private" rel="nofollow">Wikipedia</a>.  </li>
<li>They foisted Internet Explorer on the web and with their hammerlock on the desktop, forced everyone to build webpages with quirky behaviors.  Something that has only recently unraveled for them, yet they refuse to provide newer, more correct versions of IE for older OSes, using that as a way to FORCE upgrades on customers (yes, I know it is legally their right to do so, but remember I'm pointing out how they aren't good to work with, and if Google and Mozilla can support their browser on the same OSes, why can't Microsoft?).</li>
</ol>

<p>They want you locked into their platform, where you can't go elsewhere.  Face it, they only make money if you buy their server software; until recently the only divisions of MS that turned a profit were Office, and OSes, XBox recently began turning a profit as well, but the cash cows are still Office and OS.</p>

<p>When you do your startup on MS, you are getting into bed with one severely mean operator who has the money and muscle and the proven lack of scruples to do anything they want to squash you like a bug.  Do you really want to fund someone that could easily decide to run you out of business?</p>

<p>I read that C# is really a pretty nice language, that it has some really nice features and that you can supposedly run it on linux using mono which is only a few versions of .NET behind.  Our experience has been that it is slower to develop on, adding months to development.  Maybe it's just our people, but we came from a MFC/C++ environment to .NET and things got slower to develop.  We've since moved to Python and Django as we move to more web based products, and productivity has soared.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
