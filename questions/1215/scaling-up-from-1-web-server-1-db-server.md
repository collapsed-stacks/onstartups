## Scaling up from 1 Web Server + 1 DB Server

- posted by: [Etienne](https://stackexchange.com/users/-1/688-etienne) on 2009-10-13
- tagged: `technology`
- score: 5

We are Web 2.0 company that built a hosted Content Management solution from the ground up using LAMP. In short, people log into our backend to manage their website content and then use our API to extract that content. This API gets plugged into templates that can be hosted anywhere on the interwebs.

Scaling for us has progressed as follows:

Shared hosting (1and1)
Dedicated single server hosting (Rackspace)
1 Web Server, 1 DB Server (Rackspace)
1 Backend Web Server, 1 API Web Server, 1 DB Server
The question is, what's next for us? Every time one of our sites are dugg or mentioned in a popular website, our API server gets crushed with too many connections. Or every time our DB server gets overrun with queries, our Web server requests back up.

This is obviously the 'next problem' for any company like ours and I was wondering if you could point me in some directions.

I am currently attracted to the virtualization solutions but need some pointers on what to consider.


## Answer 1228

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-10-13
- score: 3

Great answers above.  Also you'll find Rackspace tech support is *really helpful*, and could actually help you with this problem.

They've solved this problem and seen other solve it, so at least give that a try.


## Answer 1233

- posted by: [user709](https://stackexchange.com/users/-1/709-user709) on 2009-10-13
- score: 1

It's difficult to give you the best recommendation without knowing much more about your application and setup. I would suggest getting someone knowledgeable in scaling to take a look at your architecture and evaluate your options.

As others have mentioned the best solution might be a caching layer in your application or more hardware. Another option is setting up a reverse proxy cache if you content is mostly static. Or maybe you just need to put yout assets into a CDN. Or something else altogether. It really is hard to give concrete advice without knowing more about your setup and requirements.


## Answer 10435

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-20
- score: 1

Yeah cloud hosting is great for cpu, but when it comes to I/O which is what you are having a problem with, I would stick with dedicated unless you can have the whole SAN to yourself which is obviously not going to happen at anything close to affordable. Been there on the cloud, and your I/O will suffer especially if everyone is backing up etc or you have other I/O hogs on the SAN. 


## Answer 1221

- posted by: [James Avery](https://stackexchange.com/users/-1/288-james-avery) on 2009-10-13
- score: 0

There isn't one answer and you have a number of different options. The easiest route is going to be to scale up the servers you have to the largest you can manage, that means a huge DB, Web, and API server. Of course you can only go so far this route, and you still have a big single point of failure. 

Reading about your problem it seems like what you would want to do is cache the content that is being pulled from your DB at the API server level using something like memcached, that way you could scale out the number of API servers and not put too much pressure on the DB. You could employ something like EC2 to scale the API servers out as you need them and prune them when you don't need them anymore. This let's you handle spikes without having to have all the servers up at the same time.

It also sounds like you should look into document databases like Couch or MongoDB as both of these can scale out with replication and would make perfect sense for your domain (although they would probably require much more re-architecting)

I would also make sure that the people consuming the API are doing caching on their end.



## Answer 1223

- posted by: [raminf](https://stackexchange.com/users/-1/404-raminf) on 2009-10-13
- score: 0

You may want to re-architect your app and split in into separate layers based on functionality. In your case, it sounds like you could have a load-balancer, a front-end webserver+memcached, an app-server, an API server, and a back-end database layer. Configure it so you can have multiple instances of each running simultaneously on one or more systems. Then throw each layer onto one or more slices.

There are a lot of VPS sites like Amazon EC2, Dreamhost, or Slicehost. You can scale horizontally if the app is too slow by cloning each slice and reconfiguring so it's incorporated into the running app. As you grow, just add more slices. At some point, inter-slice communication delays get in the way and you get a point of diminishing return.

Then you can move onto your own dedicated servers and grow that way, but the basic architecture stays the same.


## Answer 1463

- posted by: [skillguru](https://stackexchange.com/users/-1/742-skillguru) on 2009-10-14
- score: 0

Why don't you talk to your server provider to give you double/triple of burstable RAM ? For that they should charge a small amount than having a guaranteed RAM.
Burstable RAM would help in handling occasional high loads.


## Answer 1539

- posted by: [Hanno Fietz](https://stackexchange.com/users/-1/862-hanno-fietz) on 2009-10-15
- score: 0

The web server should be easy to scale out, using a load balancer and as many workers as you need. For the DB, tweak the hell out of your queries first. Then, buy a beefier server and immediately start thinking about how to shard your database, i. e. split it into chunks that can be operated independently.

A clustering DB engine like MySQL Cluster might also be worth looking at.

Also look at serverfault.com and stackoverflow.com. There's also sites dedicated to MySQL and SQL Server performance, that have great advice on making your DB more performant.


## Answer 3790

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-18
- score: 0

I think your main issue is database performance. To scale the database you need to audit the database and find out where are you hitting the bottle neck. You need to find what is the percentage of Reads and Write ratio that you are hitting, based on which you need to decide on what kind of scalable solution do you require. I can help you audit the database and do performance tuning for MySQL. If you can provide more details on MySQL version and the number of hits and concurrency to the database, which help better to find what needs to be done.

-chandru
www.mafiree.com


## Answer 12707

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-13
- score: 0

<p>It sounds like you might have a peak load issue. I'm not sure how your application is architected, but chances are if you wrote a LAMP (Linux, Apache, MySQL, PHP) application that <a href="http://rightscale.com" rel="nofollow">RightScale</a> or <a href="http://scalr.com" rel="nofollow">Scalr</a> can help you out. Couple these services with AWS and/or RackSpaceCloud, and you should have effortless horizontal scaling, that elastically handles your peak loads. </p>

<p>Nothing's perfect, of course, but I keep hearing success stories from people using Scalr or RightScale. </p>



## Answer 1218

- posted by: [blekkzor](https://stackexchange.com/users/-1/281-blekkzor) on 2009-10-13
- score: -2

One of your main issues is hosting with rackspace. I'm guessing you're paying hundreds on a single server without getting awesome specifications.

Start using cheaper server hosting companies with more powerful servers, and start employing load balancing techniques. You'll want to stay away from shared architectures like clouds and virtual servers, as you will be sharing resources and not getting your money's worth.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
