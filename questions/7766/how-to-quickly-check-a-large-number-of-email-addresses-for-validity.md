## How to quickly check a large number of email addresses for validity

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-02-07
- tagged: `email`
- score: 2

I have about 1000 people who answered a survey about 10 years ago that were interested in the product I was going to develop. They indicated they'd like me to send them an email when the beta release was out.

Obviously it took a long time (10 years), but I finally am in beta and want to send them that email. 

However, I don't want to send them all out without quickly getting rid of the obviously bad email addresses. After 10 years, I expect 80% of the emails will have changed and will bounce back to me. My ISP service would not appreciate that many bounces from one mailing.

So is there a fast and simple way to pre-check the email addresses prior to sending them?


## Answer 7778

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-02-08
- score: 3

<p>If you have a winxp machine, you can use products like <a href="http://www.email-unlimited.com/email%5Fverifier%5Fprofessional.html" rel="nofollow">this</a>. All it does is confirm the availability of a domain and the existence of an email address. Throttle the requests and your ISP shouldn't get angry.</p>



## Answer 15205

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-10-17
- score: 2

<p>I really was looking for an automated way of doing it, preferably on my website with PHP. Something like this: "<a href="http://articles.sitepoint.com/article/users-email-address-php" rel="nofollow">Verify a User's Email Address Using PHP</a>", but I had a lot of trouble getting that to work.</p>

<p>I ended up informing my email host that I'd be sending out these emails just one time and expected a lot of bounces. They allowed it. The emails went out and about 70% bounced, allowing about 300 people to get my product information.</p>



## Answer 51632

- posted by: [JoshSamBob](https://stackexchange.com/users/-1/940-joshsambob) on 2013-11-04
- score: 2

<p>There are services that will do this via an API, either in real-time (one at a time) or bulk (list/batch) mode. </p>

<p>Examples include (<a href="http://LeadSpend.com" rel="nofollow">LeadSpend.com</a>), (<a href="http://qas.com" rel="nofollow">Experian QAS</a>), and (<a href="http://strikeiron.com" rel="nofollow">StrikeIron</a>), among others. Rates and results vary, but integration is generally pretty straightforward.</p>



## Answer 7768

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2010-02-07
- score: 0

Try utility ping.

Otherwise if you are good with linux then you can write your own perl or unix script.

http://www.exefind.com/utility-ping-P25572.html



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
