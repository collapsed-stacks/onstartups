## Want to offer SaaS product via RDP, any recommendation on hosting

- posted by: [Jag V.](https://stackexchange.com/users/-1/5792-jag-v) on 2010-12-03
- tagged: `saas`, `hosting`
- score: 1

We already have a desktop product for Windows.

Unfortunately it is a win32/64 exe for Windows, and making a web version would take some years.

We want to join the SaaS party, so we want to introduce an RDP hosted version (so they don’t have to install anything, they can access everywhere, etc, etc).

Are there any successful commercial solutions offered via RDP?

Could you recommend a Windows hosting with several RDS CAL licenses?

Thanks a lot for your feedback...

JV


## Answer 17361

- posted by: [vellad](https://stackexchange.com/users/-1/4779-vellad) on 2010-12-03
- score: 1

Check spoon.net.

You might want to use their service.  I believe that you can host the service yourself as well.

They have VERY neat technology.  You will appreciate it once you test it out.

http://www.spoon.net/


## Answer 17360

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-03
- score: 0

I guess you could theoretically use some sort of terminal lic, RDP, or gotomypc type licsence for your clients to access your software, but the likelyhood of it being successful are very low.  Virtual access is extremely slow, expensive for your server to maintain, and clunky.

Your best bet is to create your application either as:
1. A full web SAAS
2. A free version that gets updated through the WEB based on a subscription.  This can be done with MSFT Smart Clients, Adobe Air Apps, and more.




## Answer 17407

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-05
- score: 0

Close to your users. For RDP-style applications, you neeed low latency on the network.

If your service is not in the same continent, the experience is going to suffer greatly.


## Answer 17901

- posted by: [ThomasH](https://stackexchange.com/users/-1/5798-thomash) on 2010-12-16
- score: 0

I have seen desktop applications offered on a hosted basis using Citrix, which is probably better than RDP for publishing an application rather than an entire desktop environment.

Would make hosting tricky, as you would need to run a VPS or dedicated server.


## Answer 19015

- posted by: [Sean](https://stackexchange.com/users/-1/6610-sean) on 2011-01-15
- score: 0

In the industry I work with the most, there is a bunch of software that's a glorified desktop app that they run in a terminal services environment (rather than running it on the client workstations).  Are you currently selling the product to work in that fashion?  If not, you might and then you can go after larger clients that would push back against installing on 1000 PCs.  You could also look at getting a hardware bundle with a vendor (Dell, etc.) and sell an "appliance" solution that you can drop off at clients ($xxk up front or some sort of lease where you get the appliance back at the end of the lease).


## Answer 20005

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-09
- score: 0

<p>If you want your users to access applications over RDP, and you are concerned with performance or latency issues, you should look at Ericom Blaze, a software-based RDP acceleration and compression product that provides improved performance over WAN and congested LANs. Besides delivering higher frame rates and reducing screen freezes and choppiness, Ericom Blaze accelerates RDP performance by up to 25 times, while significantly reducing network bandwidth consumption over low-bandwidth/high latency connections. </p>

<p>Ericom Blaze works with any standard RDP host, including VDI, Terminal Servers and remote physical machines.</p>

<p>You can read more about Blaze and download a free evaluation at:</p>

<p><a href="http://www.ericom.com/ericom_blaze.asp?URL_ID=708" rel="nofollow">http://www.ericom.com/Blaze</a></p>

<p>Adam</p>



## Answer 20021

- posted by: [Nilesh](https://stackexchange.com/users/-1/6985-nilesh) on 2011-02-09
- score: 0

I was in the same boat. I have instead begun to develop a web version completely from scratch.

I am assuming that by going SAAS you want to leverage cheaper monthly pricing on a recurring basis, correct?

If so, rather than hosting the software as SAAS, why not just let them use it as downloadable but bill them using the SAAS pricing. This would mean that the software would have to be modified to enable recurring payment from within the desktop app. Every month it would connect to your server or payment provider and renew itself. All of the user management stuff you can start building on the web so it would be kind of hybrid until you get your true web app out.






## Answer 23197

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-04-12
- score: 0

I believe that this is a strategic mistake to do that. Offering your product through RDP is not scalable, not cost effective, prompt to discrepancies between versions and opening the gate to a world of pain going forward.

If going SaaS is really your business model going forward, think strategically, and take this opportunity to invest in your future. Go around all your customers and try to learn from the current usage of your product, what did they like, what did they use, what did they not use, etc.. and build a new product, faster, accessible through any platform (mobile/tablets), that will be a true multi-tenant architecture that can scale and be cost effective.

Really. Don't take the RDP route, you will pay this mistake if not by imploding, because your competition will be SaaS before you and will be much more aggressive and competitive.

Good luck.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
