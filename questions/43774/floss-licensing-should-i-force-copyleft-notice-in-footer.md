## FLOSS licensing: should I force copyleft notice in footer?

- posted by: [stackoverflowuser95](https://stackexchange.com/users/-1/21263-stackoverflowuser95) on 2012-10-22
- tagged: `legal`, `recommendations`, `open-source`, `license`, `community`
- score: 1

I'm developing a fairly large web-application with a public-facing JSON REST API, mobile apps for every platform (using AngularJS with Apache Cordova) and specialised e-commerce configurable by users.

Going to take neither a monthly fee nor commission (i.e.: only PayPal's commission will be charged).

I do have a monetisation strategy in mind, but probably won't enact it until (well if!) there are >70,000 unique users.

---

Going to open-source the entire project, but have a double headed question on this:

  1. Should I force projects forking my code to persists a *Powered by* or *Forked from* `[project_name](repo_url)` banner in their website and mobile-app footers? If so, which license should I choose for it?
  2. What are the disadvantages of licensing the project this way?


## Answer 43776

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2012-10-22
- score: 1

You know I'm going to say it, but it depends on what you want to achieve.

1) The BSD license comes the requirement to mention the copyright holder in the documentation or similar. You could tweak it be something more specifically like the advertising you mention. Tweaking the *GPL licenses in such a way is far more difficult, it's very easy to create something legally unenforceable with them unless you know what you're doing.

2) A lot of people think open/free sourcing a project means developers will flock to it. Maybe 10 years ago, yes, forget it now unless you've something pretty unique and you've got good press contacts.

The thing with open/free licensed software is everyone and their dogs are doing it, marketing the thing is hell compared to what it used to be. Put it another way, open sourcing isn't a marketing strategy on its own any more.

Your intended money generating idea is important here, it's hard to say more without knowing what your end business model is intended to look like (who are the paying end users, how much are you going to charge them and what is it you're going to charge them for).



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
