## Does anyone have any evidence of cost-per-user scaling on AppHarbor?

- posted by: [Simon Gill](https://stackexchange.com/users/-1/21855-simon-gill) on 2013-02-03
- tagged: `startup-costs`, `cloud`
- score: 0

I'm trying to work out the viability of a web service and I'm trying to wrap my head around the impact that increasing numbers of users will have on costs. This is mostly a concern about not running out of money during the beta and growth phases.

Ideally somebody has already published a study of the number of AppHarbor workers or Heroku dynos needed for certain numbers of registered users broken down by usage amount and processing time. I'll happily accept something with the evidence that I have to learn some statistics to understand and apply though.

Any evidence-backed hints as to what kind of cost thresholds there are through the early life of a cloud-hosted web service would also be helpful.


## Answer 47147

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-02-04
- score: 2

<p>Impossible to determine without hard facts about the application, codebase and complexity.  </p>

<p>For example, there are tons of articles on the interweb talking about how to support high traffic sites using wordpress on commodity aws instances. Whether or not you can support thousands of requests depends on what plugins / caching / apache/nginx settings are set at.  The question of "how many users can wordpress support" cannot be answered here, since the number of requests wordpress supports out of the box on a vanilla instance is radically different than an optimized one. </p>

<p>Heroku is no different in that regard - dynos are simple 512M ubuntu instances. Apps built using the <a href="http://12factor.net/" rel="nofollow">12 factor rule</a> can take advantage of Herokus services beyond simple instance creation (horizontal scaling across instances, etc.) A good semi-rant on figuring out heroku (and isolating performance issues) can be found <a href="http://rdegges.com/heroku-isnt-for-idiots" rel="nofollow">here</a>. Good luck!</p>



## Answer 47151

- posted by: [Johannes Rudolph](https://stackexchange.com/users/-1/11487-johannes-rudolph) on 2013-02-04
- score: 1

It's hard to say without more details.

It's much more likely that other cost factors will dominate your calculation. If you're not trying to engage in a business that requires costly computing resources (HPC or equivalent) or vasts amount of bandwith (like YouTube), I bet hosting costs are close to irrelevant.

This is not saying that AppHarbor won't grow expensive beyond a certain scale, but you can always look to either provison AWS resources directly, rent dedicated servers or colocate your own when that will provide you significant cost savings. (Significant in this case means it's worth the opportunity cost to not implement new features/aquire more customers, the cost to administer your own servers, developer effort etc.). 


## Answer 47155

- posted by: [Simon Gill](https://stackexchange.com/users/-1/21855-simon-gill) on 2013-02-04
- score: 0

I did find a solution which at least gave me a ballpark figure. Using a free load-testing trial from [neustar](http://www.neustar.biz/enterprise/web-performance/what-is-load-testing) I set up a 1 hour test with 31 concurrent users (the limit of the free trial). I also had the New Relic add-on enabled at the free level so I could see what was going on in the worker.

The script involved was a simple unauthenticated request of the homepage (which does check the database for authorization of visible navigation elements).

Requests took an average of 7ms to complete on the server. CPU usage was around 5% during the entire test and memory usage at 100Mb. The worker served an average of 700 requests a minute from those 31 madly refreshing users.

Since memory usage at rest is around 100 Mb as well, CPU Usage is the main limiting factor of those I've measured. Bandwidth usage and DB usage are the other limiting factors (from the [AppHarbor Program Policy](https://appharbor.com/page/programpolicy)) so those will need to be measured and kept under control as the site grows.

I'm comfortable with CPU going up to 80% which means the worker should be able to handle 16 times the load I gave it - 11000 requests per minute, or almost 500 concurrent users.

Obviously as request times, bandwidth requirements and database hits go up, this will affect the number of users. This is something to keep testing on an on-going bases.

Yes, these are very loose numbers, but they are a good enough ballpark figure. It's helped me get from the thought that I could only handle a hundred or so registered users per worker and into the confidence that I can bootstrap cost-effectively.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
