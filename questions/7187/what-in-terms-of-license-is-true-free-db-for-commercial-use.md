## what in terms of license is true free DB for commercial use?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-27
- tagged: `database`, `license`
- score: 3

I like to distribute with my application that is commercial db installation 
mysql is gpl so i guess this is out of the question .
what do you suggest to use as real free db for commercial distribution ? 
Thanks


## Answer 7190

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-27
- score: 4

<p>That's actually a hard question to answer, because much of this isn't really tested in the courts -- and on top of that the national differences in laws make a truly international approach very hard.</p>

<p>First up, the <a href="http://www.gnu.org/licenses/old-licenses/gpl-2.0.html" rel="nofollow">GPL version 2</a> (the license used by MySQL and many others). In the olden days the common interpretation of the GPL was that you were bound by it if your program was <a href="http://en.wikipedia.org/wiki/GNU%5FGeneral%5FPublic%5FLicense#Linking%5Fand%5Fderived%5Fworks" rel="nofollow">compiled or linked</a> together with GPL code, i.e. your code runs in the same memory space as GPL code. However, I have since heard a gentleman from MySQL state that a webapp using MySQL via MySQL's networked SQL interface is subject to the GPL. I don't think that's correct, but clearly there is some confusion &amp; doubt about what exactly falls under the GPL.</p>

<p>One approach I've seen people take is to distribute their own application without database, and provide installation docs for the end customer so that he can download and install MySQL himself. I don't think this changes the root licensing issue problem at all; but some people have been doing this for years.</p>

<p>So, with some thinking, you can probably use MySQL for redistribution.</p>

<p><strong>If you don't want the hassle of GPL</strong>, then <a href="http://www.postgresql.org/" rel="nofollow">PostgreSQL</a> is a great and very full-featured SQL database (BSD-like license).</p>

<p>For embedded use the most popular picks are <a href="http://www.sqlite.org/" rel="nofollow">SQLite</a> and for Windows it's <a href="http://www.vistadb.net/" rel="nofollow">VistaDB</a>. These all have different, but developer-friendly licenses. Be sure to read their licenses carefully, but they permit redistribution free of charge or for a very low license fee.</p>



## Answer 7220

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2010-01-27
- score: 3

<p>If it's a single user database, have a look at <a href="http://www.sqlite.org/" rel="nofollow">SQLite</a>. Fast, amazing, in use by major players (looked at Quickbooks file format lately?) and completely free.</p>



## Answer 7189

- posted by: [Olivier Lalonde](https://stackexchange.com/users/-1/1030-olivier-lalonde) on 2010-01-27
- score: 0

How will you distribute your application? Could you host the databases for your clients? I doubt there is any free database that will allow you to distribute it with commercial software. However, MySQL does offer licensing but it's not free.


## Answer 7203

- posted by: [mitcheljh](https://stackexchange.com/users/-1/2195-mitcheljh) on 2010-01-27
- score: 0

<p>You should also definitely check out <a href="http://www.firebirdsql.org/" rel="nofollow">Firebird</a>.  I did a lot of research before deciding on a db engine for my commercial application, and decided this was the best for me.  I've never regretted my decision.  They have both a server and an embedded version.</p>



## Answer 7226

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-01-27
- score: 0

There's this thread re: mySql and PostgreSQL.  

There are other similar discussions on that forum.  Including one (but I can't find it now) that discussed the apparently ironic attempt of the person who sold mysql to sun and is now in an uproar about its status...


## Answer 7231

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2010-01-27
- score: 0

SQL Server Compact Editions and MS Access are free for commercial distribution as well. You might need to feel up a form in MS's website for 2008 though.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
