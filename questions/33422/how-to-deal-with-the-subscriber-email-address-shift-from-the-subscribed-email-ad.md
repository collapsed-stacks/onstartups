## How to deal with the subscriber email address shift from the subscribed email address to a new one?

- posted by: [web2jeet](https://stackexchange.com/users/-1/13186-web2jeet) on 2011-12-07
- tagged: `strategy`, `subscriptions`, `users`, `email-marketing`
- score: 0

How to deal with the subscriber email address  shift from the subscribed email address to a new one?


example :  Mr.A subscribed on www.example.com by using mr.a@yahoo.com, however, now he tend to shift on his another email address which is Mr.a_newemailadd@yahoo.com

**The shift from the registered email address will be a hindrance for the website, just because the user tends to be more active on his new email address.** 


## Answer 35998

- posted by: [Mike Cellini](https://stackexchange.com/users/-1/12503-mike-cellini) on 2012-02-10
- score: 1

You can't necessarily know if a user subscribes with two different email addresses. Two different users could have identical or nearly identical information. Perhaps the user changed jobs and now subscribed with his new work email. Duplicate subscriptions or what appear to be duplicate subscriptions could happen for many reasons, and you'll never know which ones matter. That said...

When you're doing email marketing you have to assume a certain number of your email addresses are effectively worthless. Users who register may simply ignore the emails. Users could register with a "spam" address used only to catch all things he doesn't care that much about.  A user could change email addresses and not re-register. A user could change email addresses and re-register.

The point is, in all these scenarios there is at least one email address that is effectively meaningless... and you'll never know which ones they are. If you're trying to figure out an expected ROI or participation embed a link in a few marketing emails, and see the average number of hits. Make sure the link is only available through email, maybe even providing a guid int he querystring and only count unique hits of the guid. After a few times of this you can learn about how much of your userbase really cares about the emails.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
