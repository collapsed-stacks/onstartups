## hyphen in URL : sporttribe.com or sport-tribe.com?

- posted by: [fabrice](https://stackexchange.com/users/-1/1565-fabrice) on 2010-10-11
- tagged: `domain`, `naming`
- score: 1

I own both domain name sport-tribe.com and sporttribe.com

Today we are using sport-tribe.com because we didn't own sporttribe.com at the time we started the site.

I'm wondering if we should change to sporttribe.com now before we start marketing the site (quite soon now)

The site has very few traffics (~20 visits per day), we have around 5 real external links on it and all emails are info@sport-tribe.com.


I have read http://answers.onstartups.com/questions/3822/domain-names-with-a-hyphen-good-or-bad-idea but I still can't decide what is the best for us.

As I own both, which one would you recommend to use ?

Thank you very much for your help.
Fabrice

PS : if I change, i'll be able to redirect all request from sport-tribe.com to sporttribe.com.







## Answer 14974

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-10-11
- score: 7

<p>Since you own both domains, use the one <em>without dash</em> as the primary domain. <strong>It is the most conventional choice, the choice most people are accustomed to.</strong> I think the number of users who actually enter URLs into the address bar is limited, but those who do will probably enter the non-dash version first.</p>

<p><strong>Ideally you should do the following:</strong></p>

<ul>
<li><p>Have a meta keywords tag with the human-readable version of the name in it, fx. <code>&lt;meta ... keywords content="sport tribe, more keywords, ..."&gt;</code>. (To help Google understand where to divide the words in your URL.)</p></li>
<li><p>Use the human-readable version of your name in the title tag, fx. <code>&lt;title&gt;some keywords here | Sport Tribe LLC&lt;/title&gt;</code>. (Again, to help Google and to build your brand.)</p></li>
<li><p><a href="http://css-tricks.com/snippets/htaccess/301-redirects/" rel="nofollow">Redirect from www.sport-tribe.com</a> to the primary domain, as you already wrote. (To help the few users who get it wrong.)</p></li>
<li><p>Set up your email server and domain MX records to <em>send</em> from the primary domain only, but to <em>receive</em> mails for both domains. (To help the very few users who get this wrong.)</p></li>
<li><p>Set up <a href="http://old.openspf.org/wizard.html" rel="nofollow">SPF records</a> in DNS that whitelist the mail servers you're using for your primary domain, and set up SPF records that show that the secondary domain <em>never sends emails</em>. (To help your emails not get falsely flagged as spam, and to make your domains less attractive to spoof in spam emails.)</p></li>
<li><p>Get the most obvious mis-spellings of your domain and redirect them to your primary domain as well. For example, not being a native English speaker, I misread your name as "Sports Tribe". The same might apply to Tribes.</p></li>
</ul>



## Answer 14973

- posted by: [Martin](https://stackexchange.com/users/-1/4248-martin) on 2010-10-11
- score: 2

<p>I would do a <a href="http://www.google.com/support/webmasters/bin/answer.py?hl=en&amp;answer=93633" rel="nofollow">301 redirect</a> from the hyphen domain <code>sport-tribe.com</code> to the one without the hyphen <code>sporttribe.com</code>.  You can also forward the email address as well.  </p>

<p>Here is a link for how to do <a href="http://www.drquincy.com/blog/redirect-entire-domain/" rel="nofollow">301 redirects of an entire domain</a> using .htaccess.</p>



## Answer 15913

- posted by: [Vergil Penkov](https://stackexchange.com/users/-1/5136-vergil-penkov) on 2010-11-01
- score: 2

There's no reason for using the hyphen. It does matter on domains like penisland.net, though. People would *never* assume correctly what it is about :)

PS: do a 301 redirect.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
