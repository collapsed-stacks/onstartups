## What is the best free/open source php based newletter system?

- posted by: [Lenn Dolling](https://stackexchange.com/users/-1/10445-lenn-dolling) on 2011-06-25
- tagged: `contact`, `newsletter`, `cms`
- score: 1

Over time I have used a bunch of email newsletter managers and seems like everyyear I am using something new.  I am worried that I have missed a really good option out there that has been right under my nose.

I know PHPlist well and but still find it very limited.

Please offer some choices that have more power.




## Answer 26755

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-06-25
- score: 2

I think PHPList is the best list programm in PHP so far. I don't like it myself to be honest. 

The problem with PHP is it has a in-built time out which cannot be modified with most hosters. It might occur that after 100 seconds of sending your emails the php process gets killed by the system. Then you have a problem. 100 seconds are not too much if you send thousands of e-mails. PHPlist has some mechanisms to deal this out, you'll need to check in detail if that works for you.

That being said, you could use Dada mail which is written in Perl and should be installable on a good bunch of webhosts:
 
  - http://dadamailproject.com/

The general problem of mailinglists is that your hoster might refuse to send so much e-mails at one time. Even when you use your own POP3 account you might have problems. This is one of the reasons people go to huge providers like:

  - http://www.yourmailinglistprovider.com
  - http://mailchimp.com/

Depending on how many users you want to use one of them.

Finally I must say I have searched for a long time for various mailinglists myself. I even wrote my own mailinglist program in PHP. It is ugly like hell but it helps me doing my stuff. It is not so overloaded as the PHPlist stuff.

If my lists ever grow, I will for sure use this open source software on my own server (root rights required):

  - http://www.gnu.org/software/mailman/index.html

or use one of the mentioned providers above.

Oh, and if you ever find a better solution then the ones I mentioned, I would love to hear and learn from you :-)

Cheers,
Christian


## Answer 26813

- posted by: [Herr K](https://stackexchange.com/users/-1/3855-herr-k) on 2011-06-27
- score: 0

Well, i researched many many systems, even commercial paid once, ended up writing my own (very primitive) email system, which also fit's right into my system :)  

I would recommend such a way too.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
