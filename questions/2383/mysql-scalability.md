## MySql scalability

- posted by: [kabir](https://stackexchange.com/users/-1/849-kabir) on 2009-10-25
- tagged: `technology`, `infrastructure`
- score: -1

Can anyone point me to any data that shows validates the scalability promises of the MySql database ? Specifically I am looking for real life examples of applications running MySql server and handling millions of transactions. I need this data to sometimes convince some of our customers that the LAMP platform is production grade.


## Answer 2405

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-25
- score: 2

<p>You may want to ask at <a href="http://superuser.stackoverflow.com" rel="nofollow">http://superuser.stackoverflow.com</a> as the sysadmins will have a better idea about scalability.</p>

<p>My concern with MySQL now is that is has basically forked. Since Sun took it over I haven't been as impressed, and now that Oracle controls it I have more concern, so I am moving to Postgres.  </p>

<p>You may want to look at what the future of MySQL is going to be before completely settling on it.</p>

<p>Here is a starting point that may be helpful:
<a href="http://ostatic.com/blog/monty-widenius-mysql-founder-forecasts-the-mysql-future" rel="nofollow">http://ostatic.com/blog/monty-widenius-mysql-founder-forecasts-the-mysql-future</a></p>

<p>You will want to at least be able to have answers about what you expect the future to hold, as your investors may ask, and not knowing would be a major problem.</p>

<p>Before you ask about scalability you will want to rephrase to give more specifics. For example, millions of transactions per day or hour? What percentage of queries will be inserts/updates and which would be selects?  What kind of hardware will you be using, and how many machines?</p>

<p>I would hope that you will have a competent dba to take care of the database, as the administration of this will be a challenge.</p>

<p>Also, in my experience the scalability problems I faced was due to the webserver, mysql could handle whatever I sent to it, but the webserver would reach limits and some connections would fail due to that.</p>



## Answer 2407

- posted by: [Ian](https://stackexchange.com/users/-1/1110-ian) on 2009-10-25
- score: 0

<p>Craigslist uses MySQL.  Check out these slides from a Craigslist engineer who describes their requirements and how they scaled.</p>

<p><a href="http://www.slideshare.net/jzawodn/mysql-and-search-at-craigslist?type=presentation" rel="nofollow">http://www.slideshare.net/jzawodn/mysql-and-search-at-craigslist?type=presentation</a></p>



## Answer 2409

- posted by: [Omer Gertel](https://stackexchange.com/users/-1/441-omer-gertel) on 2009-10-25
- score: 0

There are many companies currently running MySQL in production. Most of them had to build on top of MySQL to sustain the capacity they required: Facebook, Friendfeed, YouTube, Flickr, 37Signals, etc.

Some links:

http://bret.appspot.com/entry/how-friendfeed-uses-mysql

http://www.youtube.com/watch?v=ZW5_eEKEC28

http://dev.mysql.com/tech-resources/interviews/david-heinemeier-hansson-rails.html

However, these sites are much bigger than most, so MySQL out of the box is a reasonable choice. However, sometimes that is not the main issue. For example, if your customers are a Microsoft shop (Windows, MSSQL, .Net, etc.), they'll have a hard time with the sysadmin experience required for LAMP because they don't have the facilities (and personnel) to deal with it.


## Answer 2420

- posted by: [user1119](https://stackexchange.com/users/-1/1119-user1119) on 2009-10-25
- score: 0

Also, whole Wikipedia and it's sister projects <a href="http://meta.wikimedia.org/wiki/Servers#Overall_system_architecture">run on MySQL</a>.


## Answer 3793

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-18
- score: 0

all the top guys use MySQL like google, wikipedia, facebook, yahoo ...etc

All list of customers that use MySQL can be found here http://mysql.com/customers/

more case studies of using MySQL in mysql.com. I am not able to post case studies since the site does not allow to post more than 1 hyper link

-chandru
www.mafiree.com



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
