## Possible to run high volume website on managed hosting?

- posted by: [sk24iam](https://stackexchange.com/users/-1/4660-sk24iam) on 2012-01-11
- tagged: `hosting`, `server`
- score: 5

These days, obtaining managed hosting is very easy.  You can get a reliable managed dedicated server from a reputable host for just a couple hundred of dollars per month. Is it possible with the addons available or using multiple managed dedicated servers to host high volumne websites such as blogs or ecommerce stores.  For instance, would techcrunch or ebay survive on multiple managed dedicated servers from an online hosting solution?  I'm wondering at what point you absolutly have to supply your own hardware/servers and maintenace to go along with it.  


## Answer 34712

- posted by: [Paul Cezanne](https://stackexchange.com/users/-1/14795-paul-cezanne) on 2012-01-11
- score: 4

You don't need that. Just get on Amazon Web Services. Right now I pay about $50/month and the scalability is tremendous.


## Answer 34733

- posted by: [ejain](https://stackexchange.com/users/-1/15437-ejain) on 2012-01-12
- score: 2

Amazon does have dedicated instances as well: http://aws.amazon.com/dedicated-instances/.


## Answer 34770

- posted by: [Matt Dusek](https://stackexchange.com/users/-1/15571-matt-dusek) on 2012-01-12
- score: 1

Yes, this can be done.  We grew from a solitary server to 1B+ page views per month and 10s of thousands of requests per second on managed hosting.  (We complement our managed hosting with a variety of cloud and 3rd-party services that we deploy and decommission freely.)

One advantage is the degree of control you wield over your infrastructure.  We achieve high volume, low latency, low variance responses at the infrastructure layer in part because of our ability to run in isolation on equipment we select and are able to monitor closely.  Similar to cloud-based hosting, you can effectively amortize your start-up costs and gain fractional access to network and sysops staffing.

At the same time, they will make mistakes, and you may find as you grow that the strain sometimes breaks their processes or exceeds their expertise.  Because your success (or failure!) affects you much more directly than it affects them, I recommend that you approach the relationship as a partnership.  You must take an active interest in the work that is performed on your behalf and manage it actively.

The only point at which you simply **must** supply your own hardware/servers/maintenance (run a private datacenter) is when your ability to do it provides a significant price or execution advantage.  I don't think it **ever** makes sense when you're thinking in terms of a single server or a couple thousand dollars per year.


## Answer 34732

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-01-12
- score: 0

I think they would survive on 'multiple' managed dedicated.  But I can't imagine ebay running on a single machine no matter how awesome it was. That thing has to be load balanced, server farmed, database sharded... thing is probably distributed across a lot of dedicated servers.

Something like Stackexchange (this entire system) I think I read runs on a single dedicated machine. I think it's something huge and bad ass because they have their SQL Server setup to essentially cache in memory everything.  Something nuts like that. But it sounded like it was a single machine not a web server / database server. Could be wrong... max (as of a podcast I listened to 6 months ago) it's a dedicated web server and a dedicated db server.

Maybe not the type of specs you could provision for a couple hundred a month though.

You'll have time to scale, you shouldn't outgrow a dedicated machine over night.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
