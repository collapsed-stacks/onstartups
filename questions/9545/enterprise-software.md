## Enterprise software

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-03-24
- tagged: `enterprise`, `software`, `business`, `sales`, `market-analysis`
- score: 4

With the proliferation of web-based applications in the small business sector, it's tough to gauge the purchasing trends for enterprise-level or mid-size business server software.

I'm not referring to SaaS where the product is hosted on a third-party server, but rather to installable software installed on the customer's internal servers.

The question is, is software implemented in an "old-school" server-client style, where a dedicated server "daemon" app is placed on an intranet machine, and a dedicated rich-client is used on the desktop - is that type of software still viable as a product targeting larger-size companies, or, has the market, even at the mid-size to large-size company level, changed to web-server driven, browser-client, web-app style? 

Would a pure client-server solution be "looked down on" as a product at this day and age?



## Answer 9550

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-03-24
- score: 4

<p>Everything Ngu says is true, web-delivered software is the trend and for very good reasons.</p>

<p>However, <strong>I don't think you should just write off rich clients</strong> (or <em>smart clients</em> as I heard Microsoft refer to them) without .  There are some applications where you need a very rich, interactive experience which is hard to do in a browser.  As an example, I worked on an application for securities traders, which had to process up-to-the-second information on their trades plus real-time data from the markets.  We wrote a .NET client for this purpose which worked very well.  I'm sure with enough effort, you could have done the same with web technologies, but I have no doubt we'd have spent more time working around browser limitations and incompatibilities than addressing the business problem.</p>

<p>Of course, you have technologies like <strong>Silverlight</strong>, which mean that you have a chunk of the .NET framework available to you in the browser, but my experience so far has been that you end up struggling because the piece of the framework you need isn't supported.  It's Microsoft's strategy to address this, but that doesn't help us now.  (There are obviously other web programming environments worth looking at too, but I think the issue remains.)</p>

<p>Another thing to consider is <a href="http://msdn.microsoft.com/en-us/library/142dbbz4.aspx" rel="nofollow">ClickOnce</a> - using that technology, you can have a lot of the benefits of web delivery in terms of deployment and updates, but it gives you a full application on the desktop.</p>

<p>The bottom line is that if you want to sell people a more 'traditional' architecture in this day and age, you need to have a <strong>compelling reason</strong> for <strong>not</strong> delivering it as a web app**.</p>



## Answer 9546

- posted by: [Graviton](https://stackexchange.com/users/-1/85-graviton) on 2010-03-24
- score: 3

> Would a pure client-server solution be
> "looked down on" as a product at this
> day and age?

It should.

The reason I said this is because updates for client-server is a great hassle. You have to remember to update every single client machine whenever you make code changes. 

Deployment is another issue. Instead of deploying on one machine ( browser-based web app), you have to deploy on server+ the number of clients machine. These are the machines whose environment you can't control. Your installation can fail mysteriously, your client app can stop responding and you can't reproduce the problem.

Plus that modern web browsers are getting better and better, so they can serve more and more powerful applications. Think about Google Docs, Gmail and you will get what I mean.

Web browsers are the new OSes, and your client-side business logic is your AJAX. Forget about the client-server concept. It will hurt you in the long run more than you can realize. 


## Answer 9552

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-03-24
- score: 3

As some one who is out selling to enterprise-level or mid-size businesses everyday I would report that '"old-school" server-client style with rich-client on the desktop are alive and well. 

Customers like the idea of a web interface, but still prefer the comfort and security of controlling their system. We recently switched a client off SalesForce to a hybrid Web/Convential solution and had a heck of a time getting the data from SalesForce. 

It may be a little different in a couple of years as web/SaaS products gain greater acceptance. But, for now we are still selling alot of conventional ERP. Conventional ERP will be in place for decades to come. 

As the other commenters state, it depends on your audience. I am a big fan of SaaS solutions and see a lot of good products that are only on a web platform. 

We are doing mixes of Web solutions that integrate with "old school" systems. I am focusing on both platforms.


## Answer 9549

- posted by: [SmartCompanySoftware](https://stackexchange.com/users/-1/1629-smartcompanysoftware) on 2010-03-24
- score: 2

Desktop apps and web apps are just two different models of technically delivering your software. They both have pros and cons, but there is no way I would say that a desktop app would be looked down on.

Enterprise applications tend to have very rich interfaces that just can't be delivered through a web browser. The clients I'm targeting with my desktop application mainly express a concern about the data being stored off site and not within their control. What happens if they want to switch to another application, can they get their data exported easily enough? That kind of thing.

The desktop vs browser app is always being debated, and there is no single answer. You choose the platform that most suits your target audience. Enterprise apps can be very expensive and are sold to fewer people (more niche) whereas a web app is sold at a small price and aimed at more clients. It's important to identify whether you are targeting a vertical or horizontal market.


## Answer 9551

- posted by: [Mike](https://stackexchange.com/users/-1/2696-mike) on 2010-03-24
- score: 2

I agree with Ngu. However, it all boils down to the type of business problem you're addressing. If it is a highly collaborative solution that is accessible to many different types of employees, with multiple user profiles and access rights, then web apps tend to be easier to implement and maintain

I'm in the web app development business, and from my experience I see that companies are following a trend towards web based applications. They start by considering web apps because of all the benefits that were mentioned already (deployment, maintenance, support...). But, at a certain point, they look at web as a means to attain a longer term benefit that is many times overlooked: the ability to grow an ecosystem of web apps that share the same integration components (to hook up to legacy systems) and databases.

Most of our customers have started by building a web app to address a specific (sometimes even tactical) business problem, and then continue building on top of those apps and create new ones, to cover more business processes. At the end they create what we call a software factory of web apps that are all interconnected and interoperable, accessible from a central location, and with common style-guides and usability patterns (which makes it very easy to roll them out without having to train employees).




## Answer 9554

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-03-24
- score: 2

It depends on the market and Enterprise size companies are different. Some users do not want to give up the functionality of desktop apps. Like it or not, Microsoft Office is king in the enterprise. Take a user who has been working in Excel and tell them you've purchased a web based application to take over their pivoting and charting and you will get anarchy. "Sorry boss, I can no longer create the monthly report because I switched to Google Docs. I know you won't mind since it is so much easier on our IT department and vendors." I've seen time-billing apps converted to web apps by major vendors in their field and the data entry is painfully slow. 

Don't get me wrong, web based apps have huge advantages for the developers and admins and sometimes users, but they don't make purchasing decisions in most companies. I have a net book and have avoided installing software as much as possible. My other laptop is loaded with development tools (which there are hardly any web based substitutes.).

Most enterprise size companies image desktop machines and then copy the image to new hardware. They don't install every single application one at a time. It's not that hard to write a desktop app that updates itself when a newer update file is on the LAN or Web. Visual Basic Express can do this and it is free. Granted, I had to prove this to myself and create an app on my website to download & install.

Anyone with any anecdotes about a Fortune 1000 company who has rid their company of client-server apps?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
