## Building New Product: ASP.NET/MVC vs SharePoint 2010

- posted by: [Shankarooni](https://stackexchange.com/users/-1/5635-shankarooni) on 2010-11-27
- tagged: `web`
- score: 1

Hi I met an investor who wants a new product to sells to other companies. We agreed to make it SaaS, but we're arguing over three options:

SaaS product made by ASP.NET Saas product Made up of huge SharePoint server SharePoint add-on (as group of solutions/web parts)

I can disclose the product exactly, but, its is about collaboration and involves many interaction between users. That is the reason why we have SharePoint as an option, also because a user might optionally create web pages (single home page).

Some users dont want SaaS. There is possibility of hosting the product at a company server (some want their 'sensitive' data hosted locally).

So my question is: which one would you choose? is there a SaaS that runs on top of SharePoint?


## Answer 17100

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-11-27
- score: 0

<p>and welcome! :-)</p>

<p>Mnn, I think you may get better answers on a site more oriented towards technology. Try <a href="http://stackoverflow.com/">Stackoverflow</a> as well as <a href="http://www.sitepoint.com/" rel="nofollow">Sitepoint's forums</a>.</p>

<p>Then I'm a little bit worried about the question. My typical answer for which tech platform to develop on is <em>the one you have built 2-3 products on before</em>, i.e. prior experience on platform often trumps most other concerns. As you present the question, it sounds like no-one on your team has that level of experience with Sharepoint or ASP.NET MVC.</p>

<blockquote>
  <p>is there a SaaS that runs on top of SharePoint</p>
</blockquote>

<p>I don't know a SaaS company that runs on Sharepoint off the top of my head, but there are plenty of moderate or higher traffic web portals that run on Sharepoint. In that sense Sharepoint is 'proven' enough.</p>



## Answer 17102

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-11-27
- score: 0

Offering SAAS and a local installation is a lot to manage. For those worried about their sensitive data, are they going to take responsibility for securing their network and your application or are they just going to blame you for a breech? Will you have the resources to do local installs, configurations, upgrades and support while maintaining a SAAS site? 

You may want to do a prototype in SharePoint and see if it will work. No reason to reinvent the wheel, but there are probably features and functions you want to include to separate your product. Otherwise, everyone can just use SP and hire a consultant to customize if necessary. I don't think offering the ability to customize a home page would be that difficult to build yourself.

I guess the question is, do you want to be a software company or a value added reseller?


## Answer 17136

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-11-28
- score: 0

My advice, CUT OUT SHAREPOINT.
Sharepoint requires a decent investment from your clients. Those who dont use sharepoint will never be your customer.

A few years back, we built a CRM application.
In its early phases we built it upon MSFT exchange.
The MSFT exchange spec was so complex it would have taken us 2 years to do the development.

Once we realized that we went back to the drawing table.
We realized we wanted Email, Tasks, and Calendar in our app.
We wanted the ability to use pop and Imap to handle messages.
We did not want our clients to require exchange, it would have made their investment very expensive.  Plus we also wanted to target those in the Linux market.

We ended up looking at what functionality our clients would need.
We created a web app (this one was in PHP), that fit 95% of our requirments and built it in about 3 quarters.  Over time, we planned on itnergrating with Exchange through its api, but it never became necessary.

That CRM has since been retired, and itergrated into a few of our smaller B2B products.
But if we had built on Exchange it would never have worked.


Sharepoint has changed quite a bit.
Unless if you are planning to build the product and sell it to MSFT then dont bother making your product around it.

The anology i would use is,  Dont Remodel an apartment  you dont own.  If you remodel a condo, its yours, and you have full control and get the full value.  If you remodel an aparment, it only makes sense as long as you are in that apartment.

Rethink Sharepoint!!!


Build a simple product that can integrate with system like Sharepoint, Box.net etc. 




## Answer 17696

- posted by: [ThomasH](https://stackexchange.com/users/-1/5798-thomash) on 2010-12-11
- score: 0

You really need to understand the licensing implications of using Sharepoint vs ASP.Net MVC. Sharepoint either requires per user licenses or an internet license whereas ASP.Net does not require additional license fees to be deployed. 

Sharepoint licensing costs would make local installations of your software much more expensive than ASP.Net.


## Answer 17738

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2010-12-13
- score: 0

If your product is a good fit for most companies that already have SharePoint and you can use that as a differentiator and selling angle then it may be a good fit. But if the people you are marketing to aren't already SharePoint users and don't really care about the technology behind it I would strongly suggest ASP .NET MVC.

If you are building a PRODUCT then ASP .NET MVC will give you:

 - Testable code 
 - Cleaner markup 
 - Simpler architecture 
 - Less expensive licensing & hosting costs 
 - Happier developers
 - Happier clients

You'll be able to build exactly what you need, how you want it to work without the overhead of SharePoint. Which in my opinion has always been a piece of crap for extending and building upon.

Unless of course SharePoint can get you 80% there out of the box and you just need to implement 20%... but chances are with SharePoint you will paint yourself into a corner at some point. 


## Answer 23011

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-07
- score: 0

If you need what SharePoint provides out of the Box much of which would take years or months to design, code and test then this is the way to go its also in my experience super stable and super scaleable, further to that its really a software platform. Using Claims AUthentication or SharePoint 2010's built in security services you can pursue a number of Models and authentication mechanisms Federated AD, Forms Based AUthentication, LDAP. 

In short you can host yourself authenticate your clients in use MS hosting or the client can host it themselves MS have thought this through its very very compelling. Also you can tweak or configure the security to authenticate MS Passport, Google Facebooks and or use AD and Forms as well.

I have developed ASP.NET apps forms apps that authenticated in and out of SHarePoint you just need to wire up the application page security (so it moves seemlesly in navigation terms from SharePoint Pages to layouts. This can be done with MVC 3 or with your MVC app in another web app. In MOSS 2007 I used this thechnique for the Telerik Dialogue and Wizard.

I have seen posts on the internet about how to transfer claims auth federated claims between apps if its outside the _layouts



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
