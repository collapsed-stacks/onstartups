## Choosing Windows Hosting company for SaaS application

- posted by: [Shawn Mclean](https://stackexchange.com/users/-1/4854-shawn-mclean) on 2010-11-30
- tagged: `hosting`
- score: 4

This is basically a ripoff of this [question][1], but for windows only.

I am building a public website that will handle user data. This website is built on an Authentication system that I would like to provide as SaaS so other websites may authenticate with it and use my data.

We are also seeking a very cheap way out as we have no funding.

**Contraints**:

  1. .Net Framework 4 and MVC.
  2. Full trust.
  3. Automated backups and server administration. (we dont have any experience in server stuff).
  4. Scalable SQL Server database. For now, slow growth, in some months or years, possibly millions of views per month.
  5. Normal Compute server - ability to move to high end compute. (more data = more RAM for algorithms)
 

What kind of host is best for hosting both a public website and SaaS app in one?

*built with asp.net mvc, .net 4 and will use WCF.*

  [1]: http://answers.onstartups.com/questions/394/choosing-a-hosting-company-for-saas-product


## Answer 17239

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-11-30
- score: 6

**"Cheap", "fully managed", and "scalable". Sorry, you'll have to pick just two.**

Windows Azure gets you Microsoft SQL Server storage, and a fully managed service, and the price is quite good. To fully utilize Azure you'll have to program against Azure's APIs, so there is longer development time and vendor lock in. But Azure probably comes closest to what you seek.

Rackspace Cloud Servers is self-managed, so you'll loose a *major* benefit there. On the other hand, the prices are decent, and you can scale horizontally as well as vertically to a point (about 15 GB RAM / 4 CPU's / RAID 10 per node).

If your budget is really tight, you should perhaps start on a shared hosting platform (like DiscountASP), and then move to a dedicated server provider later (like GigeNet, ServerBeach). You'll have to be your own sysadmin then, and this is a significant risk that you should not underestimate (end users tend to get really angry if you loose their data). But if you want it really inexpensive, self-managed is probably your only option.

If you could leave MSSQL and work with MySQL then Amazon EC2 with their hosted MySQL (called RDS) becomes an option. Amazon's support for Windows has been poor, they took forever to support Windows 2008, and they still don't support Windows 2008 R2. But they offer a managed service in RDS, which takes care of the MySQL database + data backup for you...

My preferred choice in your situation would probably be Windows Azure, with a managed service offering from Rackspace as second option (but note that Rackspace's managed services are *not* cheap!).


## Answer 17238

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-11-30
- score: 3

<p>There are many hosting companies that offer full-managed Windows servers with MS SQL, .NET and MVC. Some of the ones I know are <a href="http://rackspace.com" rel="nofollow">Rackspace</a> and <a href="http://www.peer1.com/" rel="nofollow">Peer1</a>. I am currently using cloud servers from Rackspace with SQL Express, it is cheap but you do have to install all of the software besides the server OS.</p>

<p>However, I would like to know of other less expensive (managed) options as I am myself looking for the same type of service and cannot afford some of the plans that these two companies offer.</p>



## Answer 17245

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-11-30
- score: 3

RACKSPACE CLOUD.  Or you can buy your own box and colo it at a place like CalPop (Very Affordable).  Managing your own server is not hard work.  You can also look into Hyper-V hosting where you can move your image from host to host.  The only drawback is that the IP will change.. 


## Answer 17235

- posted by: [Vineet](https://stackexchange.com/users/-1/24-vineet) on 2010-11-30
- score: 2

I am not sure if this is applicable to you, but you might want to look into Microsoft Azure: http://www.microsoft.com/windowsazure/

I know the Microsoft has multiple programs to help startups.


## Answer 17236

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-11-30
- score: 1

I suggest using Netcraft as your starting point for determing whom to host from.  
http://news.netcraft.com/hosting-analysis/ 

Luck


## Answer 17237

- posted by: [Donny V](https://stackexchange.com/users/-1/3864-donny-v) on 2010-11-30
- score: 1

<p>A good start might be <a href="http://www.winhost.com/" rel="nofollow">WinHost.com</a>. There cheap but have great support. Plus they have unlimited subdomains with IIS7. </p>

<p>I would say the next step up is <a href="http://www.jodohost.com" rel="nofollow">Jodohost.com</a> and then <a href="http://www.rackspacecloud.com/" rel="nofollow">Rackspace Cloud</a> is top tier.</p>

<p>If you need control of your server(s) then <a href="http://aws.amazon.com/" rel="nofollow">Amazon AWS</a> is your best bet.
<a href="http://aws.amazon.com/free/" rel="nofollow">Free AWS Usage Tier</a> accounts for new users for a year.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
