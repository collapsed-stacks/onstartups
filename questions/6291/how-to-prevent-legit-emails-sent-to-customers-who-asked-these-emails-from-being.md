## How to prevent legit emails sent to customers who asked these emails from being considered spam?

- posted by: [Tristan St.](https://stackexchange.com/users/-1/2151-tristan-st) on 2010-01-11
- tagged: `email`, `customer-support`, `bootstrapped`, `deliverability`
- score: 5

I'm bootstrapping a business software and I've got a serious issue: I don't plan on doing any "mass mailing" nor "email campaign".

I will never ever send one email to someone who didn't ask.  My business model doesn't resolve around mass mailing/spam at all: I've got a legit software that people so far do actually like very much :)

However I've got a very serious issue: I've got about a hundred beta-testers and some of them are PM'ing (sending me PM on message boards/forums) or contacting me directly from our software (it's a fat client and there's an option in it to leave your email: if the user does so, then his email is directly send to our Webapp server).

I need to send emails to these people yet some of them get considered as spam and end up in their spam folder.

I'm not alone: I've read horror stories on "Business of Software" about customers buying products and being unable to activate them, then being unable to reach or be reached by email.  (for that specific case we're taking precaution: the very payment processing is going to be tied with the app and it shall automatically 'unlock' as to prevent that catastrophic scenario from happening).

Yet my question is: is there anything I can do?  Can I contact, say, Google (we use GMail for a lot of things, including email) and tell them "we're not spammer, we won't ever send a single mail to a person who didn't ask?"

How can I make it so my legit emails are not considered spam?  Once again: I emphasis that these are emails sent to people who willingly gave us their email address through either private messages or from our software and that are waiting for our emails.




## Answer 6300

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-01-11
- score: 3

There is no bulletproof answer to this; the techniques used to identify spam are constantly evolving as the spam evolves so what works today may not work tomorrow.

The key things that often trip people up:

 1. **Use your domain as the from address not Gmail**.  This may be controversial but it enables the next item.
 2. **Have DNS configured correctly for your domain**.  This means a few things, primarily ensuring that DNS round trip name resolution (Your Domain's MX record->Server A record->IP Address->the exact same Server A record) is correct and you have an SPF record for your domain that's correct.  This is largely in your control even with Gmail (because your domain is in your control.
 3. **Monitor your domain's reputation if you think there's an issue**.  There are a number of free sites that can check if your domain is on any blacklists.  If you get on a blacklist there's nearly always a mechanism to demonstrate you're a good guy and get off it (although they may be painful...)

Finally, I'd caution you to **avoid have email be the only way of completing a transaction** that's important to your business precisely for this reason.  Email should be a backup / alert mechanism that ideally drives people back to your site.  That way if an email went missing they can always go back to your site to get the information, complete the transaction, whatever.  



## Answer 6304

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-11
- score: 3

<p>Tristan, you should look at the previous discussions at <a href="http://serverfault.com/" rel="nofollow">Serverfault.com</a> -- a site much like this one, but targeted at system administrators.</p>

<p>In short, there is no way for you to say "Hey, I'm not spam! Don't filter me.". If there was, then spammers would abuse this system too (sic).</p>

<p>There is a war going on between spammers and good people, and sometimes innocents get hit. What constitutes a correct answer today may not be entirely correct tomorrow.</p>

<p>Having said that, here is a terse list of what I consider the most important things to do right now:</p>

<ol>
<li><p>Use separate outgoing mail servers for bulk email and business email (you stated that you don't do bulk email, so this is not relevant for you).</p></li>
<li><p>Make absolutely sure that each outgoing mail server has a static IP address, has its SMTP HELO string configured correctly, and that reverse DNS lookup to the IP address will return its HELO address. <em>(If you exclusively use professional mail providers (such as Google Apps) then this is already handled for you.)</em></p></li>
<li><p>Set up <strong><a href="http://www.openspf.org/" rel="nofollow">Sender Policy Framework</a> for your domain (SPF)</strong>, i.e. whitelist which servers are allowed to send email on your behalf. It's not that hard to do; if you use multiple email providers then you just need to include each providers SPF record into your own. Here is Google's <a href="http://www.google.com/support/a/bin/answer.py?hl=en&amp;answer=33786" rel="nofollow">Apps for Domains SPF info</a>. SPF is something you set up in your own DNS records.</p></li>
<li><p><strong>Write good email body text</strong>, i.e. use the recipients name prominently (maybe both in the subject and first line of the body), don't send pure HTML emails (if you use HTML, include a plain ASCII version too), don't use spammy language (ALL CAPS, MORE !!!!!!'s, certain words).</p></li>
<li><p>Make sure the <strong>"unsubscribe"</strong> link or mechanism for opting in / opting out of communication is <strong>easy to find and easy to use</strong>. If people can't unsubscribe when they want to, they'll just hit the "This is spam" button in their email client, and your online reputation will suffer.</p></li>
<li><p>This one is debatable: Send from a real address on your domain, which you actually monitor &amp; respond to. This is to catch complaints from the (total ******) users who only know how to operate the "reply" button in their email client, and / or can't be bothered to actually press a "unsubscribe" link. Of course, providing good customer service is always valuable.</p></li>
</ol>

<p>There is also a fine standard for strong email sender authentication called <a href="http://www.dkim.org/" rel="nofollow">DomainKeys</a>. It's a good standard, a few large email recipients support it (notably Yahoo! mail), so I'm not down on it at all. But right now it's pretty complicated to set up by yourself and support is not that widespread, so I don't consider it a "must do".</p>

<p>Real, honest statistics about email delivery success rates are hard to come by. Most of what I have seen was commissioned by the email deliverability industry itself, and therefore possibly biased -- and certainly some of it seemed alarmist to me. A fair guess is that if you do the above, then 'more than 98%' of your emails will be delivered successfully.</p>

<p>For peace of mind, you can from time to time check a online resource like <a href="http://www.mxtoolbox.com/blacklists.aspx" rel="nofollow">MXToolbox's blacklist tester</a> to verify that you're not blacklisted anywhere. This is for each outgoing mail server IP address, so if you use a large provider like Google for outgoing mail, then don't bother -- they already do this for their mail servers.</p>



## Answer 6324

- posted by: [Joe](https://stackexchange.com/users/-1/1572-joe) on 2010-01-11
- score: 3

The simplest, low-tech way to improve deliverability is to remind people to add your email address to their address book.  Wherever you offer a user the ability to contact you, suggest adding your-address@gmail.com to their address book to ensure they will receive your reply.


## Answer 6327

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-01-11
- score: 0

<p>Great answers!  For a wealth of information and on-going news about email deliverability, check out the <a href="http://blog.deliverability.com/" rel="nofollow">Deliverability Blog</a>.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
