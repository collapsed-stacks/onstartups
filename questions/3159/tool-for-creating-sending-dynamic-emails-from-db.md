## Tool for creating/sending dynamic emails from DB

- posted by: [Justyn](https://stackexchange.com/users/-1/605-justyn) on 2009-11-05
- tagged: `email`, `database`
- score: 1

I'm looking for a tool or code library that will allow me to create and send emails with dynamic information from our MySQL database. For example, sending a digest email with new connections, alerts, that sort of thing.

Any suggestions?


## Answer 3168

- posted by: [user1084](https://stackexchange.com/users/-1/1084-user1084) on 2009-11-06
- score: 1

<p>What framework are you normally using to interface to your database? The specific framework and language will heavily influence how you go about this. If you're a developer yourself perhaps you can put this together (though, you probably wouldn't be asking this question then!). For example, if you were using Python, Perl or Ruby, it would probably be a very straight forward task for a programmer to achieve something like this for you.</p>

<p>Is this for internal use (ie. site/server stats &amp; alerts) or as a marketing/newsletter purpose for your customers? All of the major scripting languages have email libraries that will easily do the former. Do you need to completely automate the process? Then sounds again like a server-side script + cron job will be the way to go. Do you need fancy HTML emails, or is plain-text fine? (Again with the script + cron.)</p>

<p>If you need a desktop/end-user solution, OpenOffice's database app can (I think) connect to a MySQL database, and from there you could build a mail-merge system as Jesper suggests, using the other components of the OO suite. It would still be worth finding an OO expert to help you do this though.</p>

<p>The other route would be getting a developer (yourself, employee, freelancer) to write a Thunderbird or Outlook plugin that would interface a MySQL db, pull out the required info, and merging into your mail. Beware that if you do large bulk-emails like thus you may need to talk to your provider to avoid being flagged as a potential spammer.</p>

<p>Good luck!</p>

<p><strong>UPDATE:</strong></p>

<p>Justyn, <a href="http://www.google.com/search?client=safari&amp;rls=en-us&amp;q=send%20multipart%20html%20email%20from%20php&amp;ie=UTF-8&amp;oe=UTF-8" rel="nofollow">Googling</a> for 'send multipart html email from php' gives a few interesting prospects, but the best and most up to date info is on <a href="http://stackoverflow.com/search?q=php%20mail" rel="nofollow">Stackoverflow</a> (for which this site, OnStartups, shares the same engine). If your developers need help on email and PHP, or other problems with implementing the email system, it will be the best place to go.</p>

<p>It should be relatively straight forward to code some PHP that will allow you to:</p>

<ol>
<li>Create a HTML email template containing fields that will be filled in with whatever server/system stats or database info you need. (You may need to tie these into command line tools if you want server stats.)</li>
<li>Construct a database query that selects which users should be sent the email.</li>
<li>Schedule automatic and repeat emailing of the template with appropriate fields filled.</li>
</ol>

<p>All the best!</p>



## Answer 3160

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2009-11-05
- score: 0

I don't know how well Microsoft Office likes MySQL -- if Office can work with MySQL, then you can do this via Excel, Word and Word's Mail Merge functionality.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
