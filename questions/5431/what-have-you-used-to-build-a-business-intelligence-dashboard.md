## What have you used to build a business intelligence dashboard?

- posted by: [Joseph Fung](https://stackexchange.com/users/-1/1669-joseph-fung) on 2009-12-23
- tagged: `analytics`, `business-intelligence`
- score: 3

We're putting together a dashboard that highlights some key metrics (helpdesk performance, website performance, distribution, reach, cost centres, digital asset volume, etc) do any of you have experience putting something like this together? If so, what tools did you use?

Our current plan is simply a custom solution comprised of XML web services, some handcrafted data crunching and javascript charting libraries for the presentation layer. Any better solutions would be welcome.

And yes, this is intended to be a "business overview" dashboard, so it doesn't need to be particularly explorable.


## Answer 5437

- posted by: [Jagath Narayan - Ordoro](https://stackexchange.com/users/-1/1975-jagath-narayan-ordoro) on 2009-12-23
- score: 4

<p>I have read a few articles written by <a href="http://www.juiceanalytics.com/" rel="nofollow">Juice Analytics</a>. They seem pretty thoughtful. They also have an <a href="http://www.juicekit.org/" rel="nofollow">opensource</a> framework. I haven't used it, so can't give you a personal review, but it may meet your needs.</p>

<p>On data visualization in general, <a href="http://www.edwardtufte.com/tufte/" rel="nofollow">Edward Tufte's</a> website is a great resource. There are no toolkits there, but just ideas and concepts. He will talk you out of building pressure-gauges, speedometers and look alikes (that we normally see in enterprise software) and instead focus on presenting information in a manner that really benefits the users.</p>



## Answer 5448

- posted by: [Michael Trafton](https://stackexchange.com/users/-1/19-michael-trafton) on 2009-12-23
- score: 4

For running my company, I've found that web-based dashboards are overkill. We tried them, but they were not flexible enough for our fast-changing environment.

**We use Excel instead.** We've created an Excel worksheet with several tabs, each of which has a particular type of data (sales, revenue, expenses, and our various other key metrics). The first tab of the worksheet has several graphs that pull the data in from the other tabs.

There are a few advantages of this: 

- It's easy to add new metrics and graphs - we don't need a developer to do it, and it only takes a few minutes
- It's easy to pull data in from other sources - we pull our pipeline data in from SalesForce using their free Excel-to-SalesForce plug-in
- It's easy to share with other folks - I can just delete the tabs I don't want to share and email them a copy of the spreadsheet
- It's easy to do scenario planning - I can fiddle with the data in the spreadsheet to see what it would look like if we closed a big deal (or lost a big deal), etc.


## Answer 5435

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2009-12-23
- score: 1

Sounds like you have the resources to build whatever you want, so I'm not sure anything you would purchase would be any better. However, you may want to look into some web controls that offer graphs and guages that may provide some real-time data in a usable format.

This is one of my projects for the coming year, so I am interested to see what you find. Our goal is to make sure we build something that will get looked at and used as much as possible. Our data needs are needed daily at best, but we may include some financial market data along side of our data which would be more up to the minute.


## Answer 5438

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2009-12-23
- score: 1

Some of the dashboard objects I have seen and used include:

 - Project Status: All of the projects the company is working on and where they are at.
 - Sales Pipeline: Quotes, PO's, Shipped and paid are all critical sales metrics that are great to see on a dashboard.

The rest of the items you mentioned are great too. I think the real trick to a dashboard is to not make it too cluttered and to really track like 5 critical business parameters. Anymore than that is probably a waste of time.





## Answer 5529

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-26
- score: 1

Just as a little sideproject, I've been building a business web apps dashboard at http://www.appexec.com.  It only has 5 app integrations right now, but when I get some more, I'm hoping it will make for a "business intelligence dashboard" like you say.  It's really simple to use.


## Answer 5446

- posted by: [Siddharth](https://stackexchange.com/users/-1/969-siddharth) on 2009-12-23
- score: 0

We have built a framework for BAM analytics. We extract data from business process instances and copy to BAM repository. This data is exposed via web services. Users can build custom queries on this data. In the UI side, we have a kind of mashup framework which can be used by business consultants to extract required data and the same can be shown as different kind of graphs in dashboard. We have used fusion chart for building the grapgs.

Regards,
Siddharth 


## Answer 5460

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-23
- score: 0

You could have a look at Crystal Xcelcius.


## Answer 5535

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2009-12-26
- score: 0

<p><a href="http://www.pentaho.com/" rel="nofollow">Pentaho</a> has a very nice dashboard. And it's free.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
