## What QA & security steps to take before launching web app?

- posted by: [Joe](https://stackexchange.com/users/-1/11334-joe) on 2011-06-19
- tagged: `launch`, `product-launch`, `security`, `qa`
- score: 2

I've seen plenty of questions dealing with beta testing, marketing, market research and so on.

My question is which **practical quality assurance and security steps** should a web app or service make sure they have ready when launching to real people?

Suggestions: 

 - double-checking against SQL injections
 - user password recovery
 - double checking file & folder permissions
 - 404 pages

Even in a private beta, what things should absolutely be a part of a launch?


## Answer 26481

- posted by: [Justin C](https://stackexchange.com/users/-1/6947-justin-c) on 2011-06-19
- score: 1

<p>Even if you are in private beta, your server can be reached by the public. That means you'll experience occasional lightweight attacks by bots. If you have information that is valuable there is a much greater chance of large attacks on your server(s) and that will require additional hardening. For now I would recommend the following.</p>

<ol>
<li>Be sure to get an SSL certificate and only allow https traffic.</li>
<li>Familiarize yourself with the <a href="https://www.owasp.org/index.php/Top_10_2010-Main" rel="nofollow">Open Web Application Security Projects Top 10 Risks</a> </li>
<li>Get some free open source applications to scan your server. The exact applications depends on the technology your server is running (Apache vs IIS, MySql vs Sql Server, etc). In general though I would recommend a Sql Injection specific tester like <a href="http://sqlmap.sourceforge.net/" rel="nofollow">sqlmap</a>, and a fuzzer like <a href="http://wapiti.sourceforge.net/" rel="nofollow">Wapati</a></li>
<li>Double check all accounts for all services on your server. If you run FTP, bots will attempt to login with standard names and passwords. Lock down all unnecessary accounts and shut off all unnecessary software (like don't run a print spooler if the server is not a print server), this is called reducing your "Surface Area" so there is less to attack.</li>
</ol>



## Answer 26526

- posted by: [Rafferty Pendery](https://stackexchange.com/users/-1/11003-rafferty-pendery) on 2011-06-20
- score: 0

<p>That is more of a technical question, I suggest you ask it on <a href="http://stackoverflow.com/">Stack Overflow</a>.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
