## Why would OKCupid write their own web server?

- posted by: [Michael Pryor](https://stackexchange.com/users/-1/130-michael-pryor) on 2011-03-09
- tagged: `technology`
- score: 56

OKCupid [wrote their own web server][1].  Isn't the technology stack basically a commodity at this point? They serve a lot of people and want to be fast, but there are very large companies that use MSFT and open source tools to get the job done.  Wasn't spending time writing a web server time that could have been spent writing one of those awesome OKCupid blog posts?


  [1]: http://www.okcupid.com/about/technology


## Answer 21377

- posted by: [Chris Coyne](https://stackexchange.com/users/-1/8450-chris-coyne) on 2011-03-10
- score: 80

The simplest part of the answer is that we started programming OkCupid back in 2003, which was a special time:

 1. It was the dark age of the Internet: a difficult time to raise
    money, it was harder to make money,
    and serving costs were still high.
    This plus the unique technical
    challenges of OkCupid made us very
    sensitive to performance.
    
 2. More important, a lot of the technologies we now take for granted
    didn't exist back then. Or they were
    unproven. The typical model in 2003
    was Apache and something like PHP +
    MySQL. (As a further example, even
    memcached didn't exist in the
    beginning of 2003.) Alternatively,
    we could've gone with
    Microsoft-based solution, but we had
    no experience in administering
    Windows servers.

As product people first and programmers second, we believe wholeheartedly in the strategy of rapid prototyping, launching with something that performs well enough, and rearchitecting - or throwing hardware at the problem - if our idea takes off. And if it doesn't take off, move on quickly with minimal investment. It's a strategy we employed regularly in 1999-2001 while building the features of SparkNotes.com & TheSpark.com, our first businesses. We didn't overengineer then, and we didn't want to with OkCupid.

So what was different?  First, we expected that it would take 2-3 years of being live before we'd learn whether OkCupid would take off. (As it turns out, it took like 5 years.) We wanted to commit to an architecture that would lend itself to scalability, security, and easy changes, since the "prototype" would be a huge project in itself.  Second, we estimated that the front end work necessary to build a fully featured dating site rivaled the back-end work of building OKWS and the back end services. This estimate proved to be pretty good.

Each problem we discussed didn't seem to fit in with the normal webserver model. Everything from the way we needed to calculate matches to the way we wanted to cache (both distributed and locally, in memory) kept pointing at an event-driven model (prferably in C++) for speed and reliability.

We wanted all these services:

 - proxies in front of the databases, for caching and other optimizations, not necessarily with a 1-1 mapping,  
 
 - general rpc servers for solving specific problems using in memory data structures (e.g., who qualifies for a match search given dozens of
   constraints and millions of users;
   what your match score is with 10,000
   qualifying people, given you've all
   answered hundreds of different
   questions each on average),   

 - a distributed cache, 

 - front end web
   services (such as profile, the
   program that serves profiles, and
   signup, the program that handles the
   signup process), which also have
   internal caches,   

 - and our templating engine

...all to be running async, speaking a common language, fast, and programmed in C++.  There wasn't really a great way to do this. And OKWS is a webserver framework that made it all work together very nicely. In fact, despite how crazy it all sounds (a custom webserver, programming in C++) developing here is extremely fast and safe.


Ok, all that said: if you're reading this and working on a new startup, I don't recommend writing your own webserver. Great tech is available now, serving is cheaper, and you probably don't have the computational workload OkCupid does. I also can't recommend using OKWS, because we don't have good documentation or configuration instructions.


## Answer 21330

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-03-09
- score: 8

<p>There can be many good reasons for DYI higher up in the stack; in the more value-adding layers. One somewhat contrived example could be a highly scalable application-specific OR/M talking to a database or NoSQL datastore.</p>

<p>But for a startup to write its own HTTP server today is <em>either a)</em> a non-commercial project people undertake for their own gratification, for the fun of learning by building it, <em>or b)</em> a mistake.</p>

<p>When OKCupid began writing their own HTTP server, there could have been a reasonable reason to do so: <a href="http://en.wikipedia.org/wiki/Comet_%28programming%29">Comet, aka long polling, aka "HTTP push"</a>.</p>

<p>Comet / long polling is kind of a hack on top of HTTP, whereby you enable application servers to "push" data to the client when data changes. Long polling places unique burdens on the web server, because it will have very many (thousands, tens of thousands) open TCP/IP connections at any time -- something traditional HTTP servers were not built for. But today there are several open-source long polling optimized HTTP stacks available.</p>

<p>(Sidebar: Comet may eventually be replaced by <a href="http://en.wikipedia.org/wiki/WebSocket">WebSockets</a>, a more generalized bi-directional communication socket that is being specified as part of HTML 5.)</p>

<p>I mentioned some edge cases, so just to be clear: Building your own HTTP server today (or file system, or notepad.exe) is generally a commercial mistake. There is no end-user visible improvement in it right now.</p>



## Answer 21415

- posted by: [Dmitriy Likhten](https://stackexchange.com/users/-1/7556-dmitriy-likhten) on 2011-03-11
- score: 4

I noticed the answers of "it was 2003" is a common story when it comes to web servers and such. I've experienced same exact reasons before.

Remember history. 2002 = the year of the first really good performing jvm (1.4). And it wasen't till later when good frameworks started to become mainstream.

2004 = the year RoR was open sourced. Nowhere near production ready for most projects. Slow as hell. Community was next to nothing.

Basically around 2005/2006 is when the amazing tools started to take shape and become mainstream. If you were to say "a web server in C" today you would be laughed out of the office. Java is chosen for "performance" because java is fast compared to ruby. C is chosen for insane optimization where writing code speed is sacrificed in favor of performance. Also note the required knowledge to write C code is significantly greater than java, as in C you have to understand how to not get memory leaked to hell while java just tells you to null out your reference when you are done with it. You can get pretty far without understanding the JVM garbage collector.

So that's that. This is why it seems so funny/stupid they chose a custom web server. But in reality its quite a good choice for the time. 


## Answer 22380

- posted by: [Eric Kennedy](https://stackexchange.com/users/-1/8976-eric-kennedy) on 2011-03-27
- score: 3

I was a 2004 user of OKCupid, wrote a webserver in C++ in 2002, and worked at Expedia.com in 2003-2004 (which was built in C++ on Windows) so I have some perspective on this.  

OKCupid started off with a big emphasis on tests and algorithmic matching; the current UI offers a lot more options for people who just care about photos so it's easy to underestimate how complex their matching code was in 2004. 

As Chris Coyne says, it took them 5 years to hit scale and they definitely could have gone the Facebook route by starting in PHP and only building the application layer in C++.  That worked for Facebook largely because they kept contributing back to the open source projects that made PHP fast (APC, memcached).  Before that, scaling a website was very expensive.

Expedia.com in 2003 had millions of users and 30+ Windows webservers running IIS with a custom C-like scripting language which talked to 15+ severs running an application layer/caching system (C++) that ran MS SQL queries on a bunch of other database servers.  Every few months the database server would get a bad query plan and the whole hotel booking engine would grind to a halt.  Having more of the logic in SQL Server stored procedures compiled into the C++ caching layer would have prevented that but taken more time.

Handling the HTTP headers isn't hard -- the hard part is perfecting the core of your application.  I wrote a webserver in C++ so files could be downloaded with a browser from the synchronization system that was my Yale senior project: http://erickennedy.org/great-idea-before-Dropbox  Using an existing protocol instead of creating an arbitrary new one made sense.

A friend recently sold his startup to Goodreads that uses Ruby for the front-end and C++ for the machine learning recommendation engine.  That configuration, or PHP and C++ (to avoid switching between very different languages) would be the best strategy for anyone who is bootstrapping a website with heavy computational needs and has a strong background in C++.  If you don't love programming in C++ (I prefer SQL), stick to Python or Ruby and MySql/Postgres.




## Answer 21373

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2011-03-10
- score: 1

I can only speculate on this. My background on web site optimization tells me that site with large traffic like OKCupid have to optimize on low levels that most web servers don't do by default or is impossible to do. General purpose web servers are not optimal in terms of speed and memory for some specific type of server settings. They probably implemented the server based on some other OS implementation and specifically hard coded some operations that can save them a processing here and there. Similarly Nginx was developed by Igor to handle the tremendous traffic of one popular Russian web site.


## Answer 21398

- posted by: [Kilo](https://stackexchange.com/users/-1/1375-kilo) on 2011-03-10
- score: 1

Some things don't make sense...

"More important, a lot of the technologies we now take for granted didn't exist back then. Or they were unproven."

Java unproven in 2003?

"The typical model in 2003 was Apache and something like PHP + MySQL. (As a further example, even memcached didn't exist in the beginning of 2003.) Alternatively, we could've gone with Microsoft-based solution, but we had no experience in administering Windows servers."

Ignoring Java in 2003?

"As product people first and programmers second, we believe wholeheartedly in the strategy of rapid prototyping, launching with something that performs well enough, and rearchitecting - or throwing hardware at the problem"

You can throw hardware at a LAMP or Linux + Java platform or even Apache, lightHTTPD + raw CGI...

Did they really write their own web server from scratch?  

I simply don't by the reasoning.  In 2003, even if you didn't know about scalability options, you had services such as Akamai you could throw money at.

I work on all sorts of technologies for a fortune-5 company.  I routinely plan for traffic loads like superbowl ads, large events like concerts where our product is paying for ad time, etc... I've never seen the need to write a web server from scratch to deal with these kinds of traffic loads....


## Answer 21351

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-03-10
- score: 0

<p>They're perceived as an innovator that really knows what they are doing which is why <a href="http://www.huffingtonpost.com/2011/02/02/matchcom-buys-okcupid_n_817368.html" rel="nofollow">match.com bought them for 50 Million.</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
