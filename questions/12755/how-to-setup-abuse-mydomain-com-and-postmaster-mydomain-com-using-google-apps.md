## How to setup abuse@mydomain.com and postmaster@mydomain.com using Google Apps?

- posted by: [morpheous](https://stackexchange.com/users/-1/3365-morpheous) on 2010-07-14
- tagged: `google-apps`, `email`
- score: 0

I have recently signed up to Google Apps.

I am setting up users for my mail accounts. When I tried to setup the following two user accounts:

 - abuse@mydomain.com
 - postmaster@mydomain.com

I got the rather cryptic error message:  

> Username is reserved for email list
> only


How do I set up these two email addresses using Google apps?


## Answer 12756

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-14
- score: 3

<p>You create them as mail groups (a.k.a. distribution lists), and then add one or more of your regular mail users to the group. In the Admin dashboard; Users and groups --> Groups --> Create new group.</p>

<p>These groups and emails to them are <a href="http://www.google.com/support/a/bin/answer.py?hl=en&amp;answer=33389" rel="nofollow">'shared' with Google</a> in the sense that Google also reads the emails. That's because these addresses are required by industry standards, for technical troubleshooting on mail delivery issues and spam. Not having these addresses could cause <a href="http://www.rfc-ignorant.org/" rel="nofollow">your domain to get blocked as a spammer</a>; and Google takes care of this for you by creating and monitoring these addresses automatically.</p>



## Answer 12766

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-07-14
- score: 0

Probably conflict with "postmaster", it is used for email lists and probably conflict with other Google settings.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
