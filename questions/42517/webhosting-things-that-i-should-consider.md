## WebHosting - things that I should consider

- posted by: [Ionut](https://stackexchange.com/users/-1/17772-ionut) on 2012-10-08
- tagged: `hosting`
- score: 1

We build an application that uses Java's Servlet 3.0 features. Among others, we use heavily its Non-blocking IO support therefore a high CPU requirement should be expected. Furthermore, we use Apache Lucene for searching (which needs disk space for the index) and some caching systems which require RAM memory.

Some Web hosting issues:

1. Considering the Servlet 3.0 API, Tomcat 7 or Glassfish 3 are required. These are surprisingly hard to find and it seems a little bit more expensive. Is there any well known provider for Java Servers?

2. For scaling we may need a lot of disk space for Lucene's index and RAM memory for the caching. Should we start by purchasing the best offer at first or an improve the hosting over time?

Are there any important things we should know on this topic? We have no experience hosting big web applications and it would be desired to avoid any bad decision from the beginning regarding this topic.


## Answer 42520

- posted by: [NeedAGeekIndy](https://stackexchange.com/users/-1/19608-needageekindy) on 2012-10-09
- score: 3

What you will be looking for is a dedicated server for hosting, where you have root access.  Then you can install whatever applications you will need.  You could also look into a colocation arrangement where they host servers that you provide.  It seems like from the questions you have asked that you have been looking for what you need in a VPS or perhaps even shared hosting.

How much do you think you will be needing to scale?


## Answer 42523

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-10-09
- score: 1

I have made a good experience with Amazon EC2. You have root access as with a "normal" engine and you can install whatever you need. You could start with a small server and easily scale out.

I made it similar and started with a cheap micro sized instance. Here is how i upgraded:
http://www.grobmeier.de/upgrading-an-ec2-instance-from-m1-micro-to-something-bigger-10072012.html

As you can see, its straightforward.

For testing, AWS offers a free tier for 1 year. You could try it out pretty well and then decide to stay or leave.
http://aws.amazon.com/de/free/

The good thing with AWS is you can easily buy extra services which are managed. For example, if DB management gets to complicated because of too much data, you could buy an RDBMS instance from amazon. They do care on the gory OS details themselves. For the start it might be enough to install your own Database on the EC2 instance.

Also they provide Loadbalancers etc.

Another option would be to use PaaS (platform as a service). Like Jelastic:

 - Jelastic.com
 - Cloudbees.com
 - Openshift.Redhat.com (beta)

and so on. The problem is they limit your access. Most often the provide a container like Glassfish, but you usually don't have root access. 

If I were you I would check out if there is a Lucene provider who offers Lucene as a service. if that is not possible I would go with EC2. It seems you have some special needs and it might be required to build up something on your own. AWS is giving you most freedom you need, altough you need to work as $root and therefore read the docs.

As a last note, I have learned from experience that "using the first option and migrating later" is a bad idea. Once you have chosen your host, you'll stick there long time. It just to painful, riskful and complex to "simply" migrate. Better take a few days more on thinking about that matter than chosing a quick/dirty solution.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
