## Is there an affordable way to host an ASP.Net SaaS application when you're a nascent startup without much capital?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-08-16
- tagged: `saas`, `hosting`, `cloud`
- score: 4

My very small company is building a hosted product and looking for options for hosting. Having done RoR for a little while, I love the fact that I can choose between options like Heroku, Linode, or a cheap basement server to get my app out there so I can run it for a couple of clients to test. I would prefer to build in ASP.Net, but the options of shared hosting, running a VPS, or investing in either Azure or Amazon seem to require a good outlay of capital for either monthly fees or software licenses that would be tough for us. Windows shared hosting seems to be a minefield for some people who run ioto SQL Server or IIS problems or limitations that aren't apparent until well after deployment. And who knows how to accurately price Azure/Amazon when you're not sure what your app's profile will be... 

What I'd like to know, is whether anyone's out there already doing this with ASP.Net (and what they're using), and are there any other options I'm missing? Thanks so much in advance.


[EDIT] Per the Amazon suggestion - that $1664 investment is still a ton of money when you're bootstrapping and you're paying up front for 3 years that you might not even use.  That $1664 could cover you a paycheck when you go full-time on your venture, a new laptop or a refurbished office.


## Answer 28860

- posted by: [pillona](https://stackexchange.com/users/-1/4721-pillona) on 2011-08-16
- score: 5

<p>Do you know Microsoft <a href="http://www.microsoft.com/bizspark/About/Default.aspx" rel="nofollow">BizSpark</a>? You can get all the software you want during three years for a one time 100$ fee + free hours on <a href="http://en.wikipedia.org/wiki/Azure_Services_Platform" rel="nofollow">Windows Azure</a>.</p>

<p>Registration is very easy. If I remember well, all you need is to be a young company with less than $1M revenue and have a corporate email.</p>

<p>Even if you do no want to use Azure, it is still worth it for the software.</p>

<p>NB: when the three years end, you can keep all downloaded software.</p>



## Answer 28856

- posted by: [Lloyd S](https://stackexchange.com/users/-1/12549-lloyd-s) on 2011-08-16
- score: 2

We had a web based CRM system developed in C# running on ASP.NET with SQL Server 2005 (now sold on to another company). 

 - We initially hosted on it on Discount ASP (http://www.discountasp.net) and the site worked ok, it is a basic cheap service. We ocassionally had big wait times to connect to SQL Server
 - We eventually purchased our own Dell servers that we hosted at a local company for about $60pm, we had signed up to Microsoft Action Pack (
https://partner.microsoft.com/us/40138499) which includes a load of great software for cheap and we used the SQL Server License and Windows Web Server license on our box. *Seems this isn't the right path, has legal implications*

I would see if you can get it running on a shared/vps first and then if you get demand move over to a dedicated machine.




## Answer 28864

- posted by: [Jim](https://stackexchange.com/users/-1/12718-jim) on 2011-08-16
- score: 1

I would suggest a small Windows box on Amazon EC2. This leave some flexibility. You haven't shelled out for hardware, and you can scale up if you need to support more traffic.

If you pay simply by the hour this will cost:

- $0.12 per hour for 8760 hours (1 year)

**TOTAL £1051 per year ($86.60 pcm)**

If you pay for a reserved instance for a year, the total cost is:

- Up-front cost of $227.50
- $0.05 per hour for 8760 hours (1 year)

**TOTAL $665.50 per year ($54.45 pcm)**

For a 3 year reserved instance, it costs:

- Up-front cost of $350.00
- $0.05 per hour for 26280 hours (3 years)

**TOTAL $1664 = $554 per year ($46.16 pcm)**


## Answer 28888

- posted by: [Areshchanka Alexandr](https://stackexchange.com/users/-1/8736-areshchanka-alexandr) on 2011-08-16
- score: 1

Don't waste your time to different shitty cloud solutions. I made a lot's of analysis whether to host my app on the cloud to dedicated server and got conclusion that dedicated server is much more cheaper, gets you more cpu\memory\bandwidth\control, it fails less (just google for how much time AWS was down this year). 
Take a look at http://www.webhostingtalk.com/forumdisplay.php?f=36 
You can find there 4 core with 8GB memory and 5TB bandwidth for 80$\months( or even less depends on configuration) if to take a year deal, or you can take AWS small instance for 60$\months with 2 not known processors of 2007 year performance with 2GB (don't remember exactly could be mistaken) memory and 1GB of bandwidth included.

What would you choose? It's all up to you)))

Regards, Alex.


## Answer 34149

- posted by: [Joe A](https://stackexchange.com/users/-1/60-joe-a) on 2011-12-26
- score: 1

<p>I use <a href="http://www.winhost.com/a/egcsbk" rel="nofollow">WinHost</a> for hosting my ASP.NET applications. For the money (dirt cheap), they provide the best value out there, and IMO most stable and mature than discountASP. The pitfalls you speak of are minimal, you can run in full trust, choose your framework version, and on and on, and it's all automated. When I launched trivlike.com I used them with the plan to migrate to Azure. I even migrated from the hosted SQL Server instance to SQL Azure without much hit; with Azure you can set a geographic perference.</p>

<p>My advice is go with cheap/shared hosting until the idea is validated, then look for high cost/performance hosting when you are ready to scale.</p>



## Answer 28855

- posted by: [hunter](https://stackexchange.com/users/-1/12714-hunter) on 2011-08-16
- score: -1

If you can find a host that runs .NET 4.0 you no longer need SQL Server Installed. You can use a stand alone and portable SQL Server CE Instance embedded within the web application.

This makes choosing a hosting provider much easier based on the high price of a SQL Server instance.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
