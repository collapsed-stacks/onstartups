## To avoid your emails being treated as spam, does it help to attach a vcf file?

- posted by: [Anthony](https://stackexchange.com/users/-1/5791-anthony) on 2011-01-01
- tagged: `spam`
- score: 4

For my online business, I need to send emails to my customers. Sometimes they get rejected by their spam filter. I try to encourage my customers to add my email address to their address book.

Do you think it would help if I attached a vcf file with my contact details? It would make it easier for my customers to save my contact details but at the same time it means that all my emails would have an attached file.

Is it a bad/good idea?



## Answer 18385

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-01
- score: 6

<p>Sorry but no, <strong>adding a VCF with your contact information doesn't help your emails to go through spamfilters</strong> (i.e. be classified as 'ham').</p>

<p>I think you should split the question into two parts, there is the "content" side, i.e. how to lay out the message content so that it looks legit, and there is the "server config" site, i.e. how your servers should be set up.</p>

<p>I actually only know about the latter part, the server configs. And I don't feel it appropriate to discuss it here, it's IMHO off topic. (And if you search around on Serverfault.com &amp; Stackoverflow.com and you will see it very well described there.)</p>

<p>While I don't want to discuss the technical aspects of server configuration here, it may be useful for others if I write up a short list of what needs to be done. Here it is, make sure that:</p>

<ul>
<li>You're sending emails from a server with a permanent, public IP address.</li>
<li>The server <a href="http://www.google.com/search?q=mx+reverse+dns+site%3Aserverfault.com" rel="nofollow">has reverse DNS properly set up</a>.</li>
<li>The server <a href="http://www.mxtoolbox.com/blacklists.aspx" rel="nofollow">isn't blacklisted for present or past violations</a> of the Internet standards.</li>
<li>You have set up <a href="http://serverfault.com/questions/tagged/spf">SPF records for your domain</a>, to 'whitelist' the servers that are allowed to send emails for you.</li>
</ul>

<p><strong>The simplest and fastest way to handle the above is to use 1-2 good hosted mail service providers.</strong> Don't set up mail servers yourself, it's too much work and the spammer / antispam battle rules are constantly changing. <strong>A good common config for many new startups is:</strong></p>

<ul>
<li>Google Apps for Domains as your main email provider, for 1-on-1 business email. If you have a webapp that needs to send emails (like account confirmation emails), then send these via Google Apps via their APIs.</li>
<li>A newsletter service provider like fx MailChimp for newsletters etc.</li>
<li>A SPF record for your domain, which <a href="http://www.google.com/support/a/bin/answer.py?answer=178723" rel="nofollow">links Google Apps' SPF records</a> into your own.</li>
</ul>



## Answer 24869

- posted by: [Martin](https://stackexchange.com/users/-1/10430-martin) on 2011-05-13
- score: 0

Mailchimp is a no go - they insist on using vcf: http://kb.mailchimp.com/article/can-i-remove-the-vcard-vcf-information-from-my-confirmation-emails



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
