## Where to get a Paid Software/Code Review

- posted by: [clifgray](https://stackexchange.com/users/-1/21414-clifgray) on 2012-12-04
- tagged: `software`, `code`, `review`
- score: 2

I have written a pretty extensive webapp and it is going to go live in the next fews weeks and before I really publicize it I want to get some professionals to review it for optimization and best practices.  How can I find software engineers who would be willing to do this?

Just to give some specifics that may be helpful, my site is on Google App Engine and written in Python and it is tough to find someone with extensive experience in that area.


## Answer 44782

- posted by: [Kekito](https://stackexchange.com/users/-1/5898-kekito) on 2012-12-05
- score: 1

I'd consider using Freelancer or Elance.  There is a wide variety of quality of work that you can get there so you are better off picking someone more expensive with a great reputation.  It should still be far cheaper than hiring a good person in the U.S.

For example, you could probably hire someone to give you feedback for $20/hour so for $200 you could get a lot of good advice.


## Answer 44785

- posted by: [Ulflander](https://stackexchange.com/users/-1/21874-ulflander) on 2012-12-05
- score: 1

Given your comment, if you need to optimize your DB queries, and secure your server on the other hand, you probably need two people.

First about the server security: most of coders will not have skills/knowledge for truly securing a whole server (well configured firewall, file rights, uninstall of unwanted packages/apps, compilation of last versions of used packages, ssh access limitations, and many more depending on what your app do). 

Concerning your DB queries, it depends on how big is your app, but it would have been better to think about optimizations at the beginning, because optimizing the queries may require code rewriting. Anyway, as you're here now, try to get a freelancer specialized in such tasks.

In fact I think you don't need a code review, but a system administrator and a database engineer. That's not the same at all.

So I would answer as @Kekito, adding odesk.com to the list of freelancers sites. Be very aware of who you hire: I had myself the best and the worst experiences using freelancers using this sites. Be sure to fully understand what you ask to them, in order to check in detail their work, given the fact you won't know them at the beginning.

In my opinion, for such things it would be better to hire people not too far from you, in order to work with them and follow carefully what they do - to control first, but above all to keep full control on your server/code once they're gone.



## Answer 44791

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2012-12-05
- score: 1

You probably only need to worry about the "low hanging fruit" for now, getting a consultant for this might be overkill.

Unless you are hugely successful on launch, performance probably isn't going to be a big deal.  I would say security in a similar boat, but you do need to be more cautious on that side.

I would suggest just finding some articles online about "common mistakes" or a basic guide that will let you tidy things up yourself.

I don't know much about Python but this looks like it might be handy for security:

http://www.pythonsecurity.org/

Here is one for performance:

http://wiki.python.org/moin/PythonSpeed/PerformanceTips

I don't know the details of your situation, but make sure you aren't worrying too much about solving problems you don't have yet.  If you are getting close to launch I am sure you have plenty of good things to worry about, focus your attention there.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
