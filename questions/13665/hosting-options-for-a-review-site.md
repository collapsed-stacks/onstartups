## Hosting Options for a Review Site

- posted by: [Emon](https://stackexchange.com/users/-1/3955-emon) on 2010-08-25
- tagged: `hosting`, `scale`
- score: 1

I am part of a start up site that will review restaurants. We are in the process of finding the right hosting provider. What would be the option for an application like ours? We want the infrastructure to be scalable. Is something like godaddy's $12/month plan work or do we need a $45/month dedicated virtual environment at other hosting companies?

Any guidance on this would be really helpful...

Thanks,
Emon


## Answer 13667

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-08-25
- score: 2

<p>I'll check Rackspace's cloud hosting offerings... it works great and it offers the scalability you are looking for, you can read the details here:</p>

<p><a href="http://www.rackspacecloud.com/" rel="nofollow">http://www.rackspacecloud.com/</a></p>

<p>Good luck!</p>



## Answer 13675

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-08-25
- score: 1

Scalability is important, but I would start my short list with providers that either specialize or are very knowledgable about your development environment. There is a difference between hosting PHP and really knowing PHP, different versions, add ins, hardware requirements and assisting when problems come up. You are responsible for your code, but they should be able to work with you.

This also applies to the database you plan on using. Many sites charge extra for SQL Server.

Make sure the provider can work migrate your app when you go from virtual to dedicated to hosted servers without too much down-time.

Curious if you've considered any non relational db's like MongoDB, couchdb, etc.?


## Answer 13681

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-08-25
- score: 0

VPS'es provide you the opportunity to increase resources (memory, CPU, disk) as your needs increases, whereas a shared hosting server typically does not.  I wouldn't start a site on a shared server - you never know what loads will be imposed by the other shared sites, and you run the risk (if you're sharing an IP) that the box can get blacklisted - and with it, your site.  Why risk it for $10 / month?

VPS'es are all not $45 / month... there are cheaper options.  I use eapps with success - also serveraxis. Do some research - you'll find a great VPS to grow with.  



## Answer 13686

- posted by: [Krzysztof Kowalczyk](https://stackexchange.com/users/-1/3945-krzysztof-kowalczyk) on 2010-08-26
- score: 0

Scalability doesn't come from hardware but from architecture of your software.

Neither option is viable for a site with lots of traffic that needs to do lots of database transaction.

You can start with $20/month linode server. Chances are you will fail before you'll need a bigger server (competing with yelp or foursquare or google places is hard).

You can scale with linode simply by buying bigger plans but if you're really serious about scalability ultimately you'll have to architect your application in a way that allows partitioning load among many machines and you'll need to operate your own servers (leased on co-located in a datacenter) or go with ec2. How to do that exactly is a topic for a book, like this one: http://oreilly.com/catalog/9780596102357



## Answer 13693

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2010-08-26
- score: 0

1. Start with a VPS from linode or slicehost.  See http://www.slicehost.com/ and choose something that fits your budget.
2. When you start seeing some traffic, upgrade to a bigger VPS.
3. When you see that you're spending more than $500/month migrate to Amazon EC2.

The hosting provider is a small issue. The bigger challenge is system administration and development in ways that scale. 

Having said all of the above, just get a VPS, focus on your product and don't worry too much at this stage about scalability. You can tackle it later, when the product has proven itself.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
