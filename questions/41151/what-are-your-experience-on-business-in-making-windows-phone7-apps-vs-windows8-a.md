## What are your experience on business in making windows phone7 apps vs windows8 apps?

- posted by: [Lamin Sanneh](https://stackexchange.com/users/-1/19140-lamin-sanneh) on 2012-08-08
- tagged: `business`, `apps`, `mobile-apps`, `phone`
- score: 2

I am currently making windows phone7 apps. I was wondering whether I am missing on something by not making windows8 my primary development platform. I am considering programming for both somewhere down the road but I was wondering whether I should make the switch instantly.


## Answer 41155

- posted by: [Faster Solutions](https://stackexchange.com/users/-1/19103-faster-solutions) on 2012-08-08
- score: 4

I've written a number of WP7 apps  and have been reasonably successful in the market.  I took the plunge and decided to convert one of the apps over to a W8 Metro app.  There's some stuff you really need to know going forward...

First: Technical

 1. Metro apps are using a subset of .Net 4.5.  Windows Phone uses a version of Silverlight, so these are using entirely different technologies.
 2. Back-end code that talks to services will need to be re-written using the new MS await/async pattern in .Net 4.5.  Any service-driven code in WP7 is not portable
 3. The controls are entirely different.  You'll also need to handle multiple screen-states (Snapped, Filled, Full and Portrait) and there are new design guidelines about giving your app a "Metro" feel.  Your UI will need to be re-written.

So, forget about common code.  It's not going to happen.  Any services you have are fine, but your UI is going to be a complete re-write.

Second: Business

 1. WP7 is basically dead.  In October expect an entirely new range of W8 phones.  Existing users cannot update their WP7 devices to W8.  Anything you write for WP7 will be limited to a market of about 14 million users.
 2. W8 expects a market of 400-500 millions users.  They'll all have access to the app store.  These are just the desktop users.  There may be tablet users but we don't know if the W8 tablets will be a flop or do well.  Even so, 400 million is a big number.

So, if you've decided (like me) to jump on the W8 bandwagon, how do you do it?

 1. Find a MS event that helps WP7 developers transfer their apps to W8.  They've been having these in the UK and US and are invaluable.  You get 2 days of help on W8 by technical experts; more importantly, **you get access to a testing session to get your app into the W8 marketplace before it goes live on October 26**.
 2. Start coding - and designing.  It's a different form factor with an entirely different look and feel.

Hope this helps.


## Answer 41154

- posted by: [Martin](https://stackexchange.com/users/-1/4248-martin) on 2012-08-08
- score: 2

I would stop making Windows Phone 7 apps immediately and move on to Windows 8.

 1. Windows Phone 7 Apps will run on Windows Phone 8, but in legacy mode.  And Windows Phone 7 will not be able to upgrade to Windows Phone 8, so it is basically dead.
 2. More people use Windows than Android and iPhone combined ... so there is a huge marketplace.

Windows Phone 8 comes out in Oct (the 26th I think), so I would try to get some good apps out there and be one of the first to establish yourself.


## Answer 41156

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-08-08
- score: -1

The simple answer to this question is that you are making apps for the wrong market. Here's the breakdown for mobile phone market share as of 1st quarter 2012:

 1. Android: 59%
 2. IOS: 23%
 3. Windows phone: 2.2%

Note that the Windows market share went **down** from 2011. So if you want to bet that Windows phones will cause a massive number of Android and iPhone users to switch to Windows, start making Windows 8 phone software. Otherwise, switch to Android or iPhone development.

If you are stuck in the Windows phone world, note that anything other than Win 8 phones will **quickly** disappear from the market. The average Windows phone contract is over 1 year old, which means the user will be replacing it within a year. And if the choose another Windows phone it will be Win 8.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
