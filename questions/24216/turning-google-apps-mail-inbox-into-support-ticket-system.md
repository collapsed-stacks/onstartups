## Turning Google Apps mail inbox into Support Ticket System

- posted by: [Saif Bechan](https://stackexchange.com/users/-1/10668-saif-bechan) on 2010-04-15
- tagged: `email`, `support`
- score: 0

I have an account at Google apps and most of my email is done trough Gmail. Now I just manually respond to support email. I was wondering if there is an easy way using filters and auto responders to create a support ticket system.

I think something like this would be great, but is it possible:

>Gmail has to make a unique ID for every email that comes in. After that all the other incoming mails should be grouped using that unique ID and not grouped by email.

Something like that, or are there things I am not taking into account. I really don't want to use separate software for this, because I think with some small configurations this can do the trick quite well.

Or are there some free apps on the marketplace that do this already. I have searched for this but cannot find any.



## Answer 24217

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-15
- score: 2

Assuming that users have to click on a link somewhere or submit a form to email you, you may be able to take an advantage of a thing called a recipient delimiter, which Gmail plays well with.

basically all you have to do is change all links that point to your email to something like

`youraddress+support@domain.com`. This is NOT a separate email address and it will STILL go to 

`youraddress@domain.com`, however, you will now be able to set up a Gmail filter and sort anything that comes to `youraddress+support@domain.com` into a separate tag(folder). This does wonders. 

Also, check out a little feature in Gmail labs called Multiple Inbox. It will allow you to separate `youraddress@domain.com` from `youraddress+support@domain.com`, but still be able to view both at the same time in your Inbox page.

This will do what you need. I have the same setup at work to separate trouble tickets from the regular mail.


## Answer 24218

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-08-19
- score: 0

@solefad: what Saif is (I think) referring to is that (in Google Apps) you can have multiple aliases which all point to the same account. In that way, the sender believes they are emailing support@yourdomain.com when at the Google Apps end that is just an alias for joe@yourdomain.com BUT allows easy filtering by To: address.


## Answer 24219

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-04-29
- score: 0

<p><strong>With just Google Apps</strong> (i.e. GMail on your own domain name) I don't know of any way to build a 'real' ticketing system.</p>

<p><strong>The simplest thing you can do</strong> is use just plain Google mail, with Google's own conversation tracking based on subject line, together with a keyboard text expander (like <a href="http://lifehacker.com/#!238306/lifehacker-code-texter-windows" rel="nofollow">Texter</a>, <a href="http://lifehacker.com/#!5749631/the-mac-text-expansion-face-off" rel="nofollow">Snippets</a>, there are many) to insert frequently used texts -- "thanks for writing", pointers to your website FAQ, et cetera.</p>

<p><strong>You can also use one of the real support handling applications</strong> which integrate with email via POP3 -- f.x. <a href="http://www.fogcreek.com/fogbugz/" rel="nofollow">FogBugz</a>, <a href="http://tenderapp.com/" rel="nofollow">Tender</a>, <a href="http://www.zendesk.com" rel="nofollow">ZenDesk</a> et cetera. These generally give you online FAQ's, canned email responses, as well as robust email conversation tracking (i.e. the unique ID given to each mail, which allows you to keep all emails with a given customer in one view).</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
