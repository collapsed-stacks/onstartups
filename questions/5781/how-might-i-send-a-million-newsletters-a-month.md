## How might I send a million newsletters a month?

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-01-01
- tagged: `webservices`, `newsletter`
- score: 5

What would you recommend for sending a very large number of newsletters, e.g. a million or more each month? 

I would want them reliably delivered within a few days. I am willing to pay a reasonable amount (e.g. up to about $400 a month), but I do need something that can handle lists that size, and maybe even up to ten million. (Here's hoping my business grows that large in the next decade.)

Note that most email marketing services don't post their rates for such large lists, and you need to email them for a custom quote. Looking at the way their prices rise as the list size increases, most seem like they might price a sending of 1,000,000 newsletters at about $6,000. I can only guess then that ten million would be maybe $30,000.

If this were a marketing newsletter, then I could probably justify paying that much if the potential revenue returned was enough to cover the cost. But since this is an added-service newsletter I'm asking about, I don't want to spend that sort of money. 

Any suggestions of a way to send a million at around $400 and ten million at no more than $1,000?

There do appear to be three ways to go:

1. Your own server. You do all the work.

2. You maintain the list at your site (e.g. PHPlist) and use an SMTP service for the mailings.

3. You get a service to host the list and do the mailings.

I think I'm leaning towards #2.

---

Note: I wasn't looking for the best SMTP service. I was looking for the general best way to send out a million newsletters at a reasonable cost.





## Answer 5822

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-01
- score: 5

<p><strong>1 million emails delivered within 48 hours?</strong> That's around 6 mails per second. That's doable from a single server, but it would have to be a fast server with excellent network connectivity.</p>

<p>One way to more or less achieve OP's goal is:</p>

<ul>
<li>Lease a good server with a fast disk subsystem (Unix mail servers use disk for mail queuing, meaning disk-I/O is vital for performance).</li>
<li>Install <a href="http://www.postfix.org">Postfix</a> or a similar modern MTA.</li>
<li>Install a distribution list manager, perhaps something like <a href="http://www.phplist.com/">PHPList</a>.</li>
<li>Set up <a href="http://en.wikipedia.org/wiki/Reverse%5FDNS#Uses">Reverse DNS</a>, <a href="http://www.openspf.org/Introduction">SPF</a>, secure Postfix against relaying, and do all the other things that need to be done to avoid getting classified as a spam source. See Serverfault and Stack Overflow for previous debates on what needs to be done, it's somewhat involved.</li>
</ul>

<p>And when you're done? I'm guessing that a server fast enough to handle 6 SMTP deliveries per second will chew up most of the 400 USD pr month budget. Then there is your time spent setting all this up, and the monthly upkeep of administrating the server, handling false positive spam complaints, et cetera -- <strong>unless you value your own time at zero</strong> then I don't see how this can be done within this budget.</p>



## Answer 15203

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-10-17
- score: 1

<p>I ended up using a PHP-based newsletter program on my webhost and selecting LuxSci at <a href="http://www.luxsci.com" rel="nofollow">www.luxsci.com</a> as my SMTP service. </p>

<p>LuxSci seems to be reputable and have prices based on limits. As my amounts increase, I can simply increase my limits and pay more.</p>

<p>I've started at 5,000 emails for $5.00 per month. I can go to 75,000 emails per month at $135 per month. Once I surpass that, I'll take their dedicated server option at $200 per month.</p>

<p>I especially like their bounce analysis, that sends bounces into a file for me, and I can automate the cleanup of my list with it.</p>

<p>My PHP-based newsletter accesses my user database that is in mySQL on my webhost.</p>

<p>It works reasonably well, but takes a little too long to send the newsletters to the SMTP service. So I may have to re-evaluate once my subscriber list grows to the point that the time to send takes longer than, say, 8 hours or so.</p>



## Answer 44750

- posted by: [BrianAdkins](https://stackexchange.com/users/-1/21412-brianadkins) on 2012-12-04
- score: 1

I would have used sendgrid as @JIMG suggested and not your own server. 

Sending a million emails is the easy part... Convincing google, yahoo & hotmail not to reject those emails or dump them to a spam folder should be the real question here. 

Even if you send a million via your own server, odds are that only a fraction will reach your customers.

When ISPs see a new server sending a flood of emails to *their* (the isp's) customers, they tend to hit the panic button and reject everything. 

Try googling "email deliverability" for more info. 





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
