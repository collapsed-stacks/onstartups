## Solutions for sending large amount of opted-in mails

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-09
- tagged: `email`, `webservices`
- score: 2

We are launching a web application which will send large amount of emails to user's first degree connections (OPTED IN, NOT SPAM). Now this is a sensitive issue and most hosting providers doesn't support doing it. Can you please suggest us how we can handle this? What does people usually use for sending notifications to large amount of users?

There will be initially approx 30,000 mails per day which will grow upto 100,000 at some point. 

Is there any paid service provider/API for managing such a large amount of outgoing mails? Can we do this by installing mail servers like postfix in our hosting (RackSpaceCloud) 

Regards
Derek


## Answer 18733

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-09
- score: 3

<blockquote>
  <p>send large amount of emails to user's first degree connections (OPTED IN, NOT SPAM).</p>
</blockquote>

<p>That's a bit hard to read. I will take it to mean that the "first degree connections" have themselves opted in, not that the "users" have opted in the "first degree connections" without asking them. The former would be fine, the latter could be debated, depending on the specifics of the situation.</p>

<blockquote>
  <p>Is there any paid service provider/API for managing such a large amount of outgoing mails?</p>
</blockquote>

<p>Yep. You can start off with <a href="http://stackoverflow.com/questions/3746213/sendgrid-vs-postmark">this thread over at Stack Overflow</a>.</p>

<p>You'll need to decide whether you want a pure outgoing mail server (i.e. your own application handles all logic), or whether you want a newsletter provider (the provider handles un-subscription, has some templating logic, etc). Search around on Stack Overflow, there are multiple variations on this question already, and good answers over there.</p>

<p>If you want pure outgoing "SMTP-server-as-an-API", then I think <a href="http://www.SendGrid.com" rel="nofollow">SendGrid</a> is the largest provider. For the newsletter providers, there are many good services -- MailChimp, Campaign Monitor, AWeber, etc. Most of the newsletter service providers also have an API for just sending a mail from your app.</p>

<blockquote>
  <p>Can we do this by installing mail servers like postfix in our hosting (RackSpaceCloud)</p>
</blockquote>

<p>You <em>could</em> if Rackspace would allow you. It's probably <a href="http://answers.onstartups.com/questions/5781/how-might-i-send-a-million-newsletters-a-month">cheaper than using a 3rd party provider</a>. But generally I'd advise against it. Getting emails delivered without being marked as spam is real work; and it's a constantly evolving field. See <a href="http://answers.onstartups.com/questions/6291/how-to-prevent-legit-emails-sent-to-customers-who-asked-these-emails-from-being-c">my answer here for a introduction</a>, and then go read more on Server Fault and Stack Overflow.</p>

<p><strong>One last thing:</strong> If you're cheap, then Google App Engine can be used to send emails. But <a href="http://code.google.com/appengine/docs/quotas.html#Mail" rel="nofollow">watch out for the quota limits</a>, and in general, research this before settling on it.</p>



## Answer 18734

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2011-01-09
- score: 1

<p>100,000 emails per day is 3,000,000 a month. That is considered a very large number. </p>

<p>I'm using <a href="http://luxsci.com" rel="nofollow">LuxSci</a> who are Email hosters. THey are designed for high volume affordable outbound SMTP, and do not allow spam to be sent via their servers.</p>

<p>At your daily volumes, you'll want one of their dedicated high-volume email servers, which is $200 to $350 per month depending on whether you only need their basic or their premium services.</p>



## Answer 18729

- posted by: [Ankur Jain](https://stackexchange.com/users/-1/6146-ankur-jain) on 2011-01-09
- score: 0

There are numerous email marketing providers out there. Check with Aweber - http://www.aweber.com/ , MailChimp - http://www.mailchimp.com/ 

I personally use Aweber and quite satisfied with it. Mailchimp is a good option if you want to see how these solutions work, they provide a free plan to start with.

(btw Am not affiliated with any of the above companies)


## Answer 18732

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2011-01-09
- score: 0

You could check out http://sendgrid.com. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
