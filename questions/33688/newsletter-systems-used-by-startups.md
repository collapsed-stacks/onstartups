## Newsletter systems used by startups

- posted by: [Shawn Mclean](https://stackexchange.com/users/-1/4854-shawn-mclean) on 2011-12-13
- tagged: `email`, `newsletter`
- score: 1

Is there an existing system that startups or websites uses to send their newsletters out to users that are signed up to their site? I don't really want to go build a subsystem just for that so I'm seeking some.

Features that I could think of:

 1. Templates
 2. Bulk
 3. API (some way to add users to the system) Or maybe I'll have to provide an API for it.
 4. Categories.

I'm mainly look at open source or even a paid app that I will install on my server. Nothing SaaS like [MailChimp][1].


  [1]: http://mailchimp.com/


## Answer 33690

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-12-13
- score: 1

<p>There are these two: </p>

<ul>
<li><a href="http://www.phplist.com/" rel="nofollow">http://www.phplist.com/</a></li>
<li><a href="http://dadamailproject.com/" rel="nofollow">http://dadamailproject.com/</a></li>
</ul>

<p>Both are not really satisfying compared to tools like Mailchimp. Both are a bit tricky to install and I have never found trust into them. But my experience is pretty old, they might have become better. WHile phplist is using php, dada is based on perl. I think both have templates and categories and are able to send bulk mail. I also think they have at list a post-interface for adding new subscribers.</p>

<p>If you like it more archaic, you might be able to use mailman:
<a href="http://www.list.org/features.html" rel="nofollow">http://www.list.org/features.html</a></p>

<p>This is more for mailinglists, but very powerful and can be controlled by mail commands. </p>

<p>That being said, when using this tools for a lots of subscribers you likely get problems. Your hosting provider might get anxious on you sending thousands of mails and cut you down. When using pop3 for sending this might be true for your mail provider. After all, don't send it from the same machine as your startup webapp runs. If a user complains (be it correct or not) it might happen that you get blacklistened and your app mails will become spam.    </p>

<p>This and the high load bulk sending of mails brings is why I usually recommend providers like MailChimp or Yourmailinglistprovider.com.</p>

<p>If you just have a few hundreds subscribers phplist/dada will do the trick.</p>



## Answer 33718

- posted by: [Ryan](https://stackexchange.com/users/-1/465-ryan) on 2011-12-14
- score: 1

<p>If you're ever going to be sending more than a trivial amount of email (more than a few hundred) then, quite frankly, <strong>you are insane trying to self host this. ;)</strong></p>

<p>Bulk email is a dirty messy business, full of bodged hacks, held together with Duct tape and obscure incantations and you should have plenty of better things to spend your time on.</p>

<p>Its not the software that is the problem (sending emails is trivial and there are plenty of options and you could even throw something together yourself in a few hours) its <em>everything</em> else that you've got to manage. Like what? How about <a href="http://mailchimp.com/resources/guides/html/email-delivery-for-it-professionals/" rel="nofollow">Email Delivery for IT Professionals</a> (especially the Feedback Loop part which is an exclusive club you will struggle to get invited to). Even allowing for the source and it being over-stated for marketing purposes it should make you think twice.</p>

<p>If you still want to self host then consider using one of these services to actually handle the delivering part :-</p>

<ul>
<li><a href="http://aws.amazon.com/ses/" rel="nofollow">Amazon Simple Email Service - Amazon SES</a></li>
<li><a href="http://sendgrid.com/" rel="nofollow">SendGrid.com</a></li>
<li><a href="http://postmarkapp.com/" rel="nofollow">Postmark.com</a></li>
</ul>

<p><em>(And there are dozens more)</em></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
