## How do you discourage piracy of your software or IP?

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2010-02-18
- tagged: `piracy`, `development`, `software`, `intellectual-property`
- score: 4

We're reviewing/exploring anti-piracy measures for a new software product. There is a desktop and a web component. What tactics are you using to prevent/discourage piracy of your software and IP?


## Answer 8217

- posted by: [Slav Ivanov](https://stackexchange.com/users/-1/23-slav-ivanov) on 2010-02-18
- score: 5

<p>Probably not the answer you are looking for, but <a href="http://blogs.balsamiq.com/product/2008/10/19/my-views-on-software-piracy/" rel="nofollow">this powerful post</a> from Balsamiq's blog describes "the main categories of software users when it comes to purchasing software versus stealing it" and how to deal with them:</p>

<blockquote>
  <p>People buy products from companies
  they trust and respect, and who treat
  them well in return. People buy
  software if they know that the people
  behind it care for your success while
  using it. They want to see the
  software improved continuously and
  with a passion. They care about a
  sensibility for usability and
  attention to details. </p>
  
  <p>These aren’t things one can steal.</p>
</blockquote>

<p>There are also several anti-piracy measures discussed there too.</p>



## Answer 8235

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-02-19
- score: 3

The <a href="http://www.asp-software.org">ASP</a> has a members only series of very active newsgroups that discuss this topic in detail. There are typically 75 - 100 new posts each day. It costs $100 per year to become a member and gain access to these newsgroups.

For desktop software there are three general approaches. Which approach you take depends a bit on who your target audience is (business / consumer) and your type of product.

1) Build you own software protection scheme that is incorporated into your software. Advantages- it can be harder to crack. Disadvantages- you must spend a considerable amount of time building and maintaining this system. You also have to hunt for cracks to know when to repair your system.

2) Purchase commercial software protection and incorporate that into your software. Advantages- much less work on your part. Disadvantages- you must spend time integrating the software with your own. You also have to hunt for cracks to know when your system has been cracked.

3) Divide your product into two versions, a trial version and a full version. Make sure there is no way to convert a trial version into a full version. When customers buy the full version they download a new copy and install that. Advantages- much less work on your part than the other approaches. There is also nothing to crack. Disadvantages- crackers can post a stolen copy on a bit-torrent.

From the general comments in the ASP forums, approach 3 seems to have the least number of problems.



## Answer 8216

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-02-18
- score: 2

<p>Maybe there is someone from the classic Shareware community hanging out here -- if not, then I guess you'll get the best answers at places like <a href="http://www.oisv.com" rel="nofollow">OISV</a>, <a href="http://www.asp-shareware.org" rel="nofollow">ASP</a> and <a href="http://discuss.joelonsoftware.com/default.asp?biz" rel="nofollow">Business of Software</a> forums. Oh, and do use the search; it's a age-old question.</p>

<p>I've never been in the situation, but my gut feeling is that you're never going to win over the hard-core hackers, so you should settle for discouraging the casual copyist.</p>

<p>To me, that implies:</p>

<ul>
<li><p>If you're using .NET / Java for the desktop part, then absolutely obfuscate the files of the desktop component. If you don't then it's super-simple to look inside your code and see what it does.</p></li>
<li><p>Have a licensing system with license keys. Traditionally this was a component you bought from another micro-ISV. Since you have a web component, maybe it's just as easy to have your desktop app call the webapp to verify license status?</p></li>
<li><p>Have a good EULA, and have the end user <a href="http://www.fenwick.com/docstore/Publications/Corporate/Top%5F10.pdf" rel="nofollow">actively accept it</a> during installation.</p></li>
</ul>

<p>You don't write what the business model looks like -- subscription "as a Service" or purchase the desktop app for a one time fee. Depending on your model I would suggest having a good FAQ to outline how license key renewals, upgrades with new functionality, security updates and bugfixes for old version etc are handled.</p>



## Answer 13871

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-09-03
- score: 2

<p><a href="http://www.keylok.com/" rel="nofollow">We use a dongle to protect our software from Keylok</a>.  It is not for everyone.  The hardware costs $30 per unit.  Our software licenses start at $9000 and go up from there.  </p>

<p>We are under no illusion that this will thwart a determined cracker or hacker.  The main goal is to keep honest people honest.  We sell to financial institutions and large news corporations.  They have a lot to lose for violating our license agreements.  </p>

<p>Someone else mentioned different classes of users/people.  You have to take a close look at your expected user base and figure out what your plan will be - how much time and money you will spend on this issue.  It has to be considered, but once you resolve how to handle it move on to the important part of delivering value in a way that is not intrusive.</p>



## Answer 13859

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-03
- score: 1

Check out my question about an Anti-Piracy startup!
http://answers.onstartups.com/questions/13858/digital-anti-piracy-system-your-opinion-comments-and-a-few-questions



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
