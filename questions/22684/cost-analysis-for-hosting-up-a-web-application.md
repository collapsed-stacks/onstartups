## Cost Analysis for hosting up a web application

- posted by: [aklin81](https://stackexchange.com/users/-1/8962-aklin81) on 2011-03-31
- tagged: `website`, `software`, `hosting`
- score: 3

I am in the process of planning a venture related to a **social web application** targeted towards a very specific user group. 

I need your help to do **cost analysis** of **hosting my web application (on the servers)**. 

Some information for this:-

1. The development of the project is being done by the founding members themselves, thus until now there has been no cost incurred for the development. 

2. We're using all open source solutions for the development so no licensing fees are involved. 

3. You may also ignore the expenses related to marketing etc of the product. Consider only the expenses for bringing up the site live and keep it running with users. 

4. Of course that would depend on how many users are registered on the application, thus you may consider a sample size of, lets say, 100,000 users on the application. 

5. The application is expected to have similar usage pattern as `linkedin.com`. The application is viral in nature(spreads by users invites).

Let me know in case you need any more information.



## Answer 22691

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-03-31
- score: 4

@aklin81: Your question is, I'm sorry to say, not possible to answer. You're basically asking "how long is piece of string", to which there is no answer only another question. This will be completely dependent on:

 - How much CPU, RAM, disk I/O etc *your application* typically consumes per connected user.

 - How many users **are online / using the service simultaneously during peak usage**.

 - How much **system administration help you need**, i.e. how many hours of a qualified sysadmin's time you need to purchase as a consultant for you.

I can offer a few pointers / things to think about:

 - Typically, the cost for servers is rather small. The human time costs -- sysadmins patching OS, setting up backup, tuning servers, scripting deployment etc dominate over machine costs.

 - If you nevertheless want to model expected machine costs, you need to *a)* measure how many requests per second your application will handle on a average server, *b)* guesstimate how many online users you will have during peak loads and how many requests they'll make, *c)* whip up a small spreadsheet.

 - If it's not that important, then you could just guesstimate machine costs. Say <100 USD/month during initial development when you're just using a staging server, <200 USD/month during first launch where you have almost no customers, <500 USD/month for a couple of servers on Amazon EC2 / Rackspace Cloud etc for up to the first 20,000 or more customers.

Sorry, but if you need *exact* numbers, then you will have to **measure** your application performance, and do some elementary school math on load and resources required.


## Answer 22685

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2011-03-31
- score: 3

We've just brought up a site using Amazon Web Service, specifically the auto scaling and load balancing.

The advantage is that is you have few users the cost is low, but if there's a spike it easy to configure to bring up resources to copy with the spike. The time it took to bring the system up was trivial, compared to trying to do it ourselves, we balanced higher processing costs against an order of magnitude improvement in time to market (although this is specific to us, it's unlikely to help you that much).

The only thing I would say is if you get to a point where the costs start to mount up, think about which parts really require the Amazon high availability and which don't. 

The great thing, of course, is if you have high server costs, it means you have a lot of users (or a terrible architecture :) ), so you should either by generating money or have a business case to get burn-money funding.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
