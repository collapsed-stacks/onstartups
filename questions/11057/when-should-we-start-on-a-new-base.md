## When should we start on a new base?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-05-11
- tagged: `development`, `beta`, `market`
- score: 1

we have recently launched a Beta version of our site. This version is currently online in public Beta, but the concept has evolved and change and our developer are about to implement those changes. There are visual, usability and core functions changes. My question is should we start the site in a new version, on new basis to avoid messy code and duplication of functions? Alternatively, should we have planned our site in perspective of doing those change to core features Without having to Restart from the scratch?

We do those change because after 2 months online, we have updated our concept from user feedback and because we are an agile team. Our main hesitation is the time that will take to start from scratch. We have worked 8 months with 1 1/2 developers to have the current online version. We now have two developers, experiences, a lot of script and functions already developed, this will accelerate things?

Did we do something wrong or is it a normal situation for a web startup?
This is normal to always ask for change and think of update to fit the market?
Do you have any advice?

Thanks alot


## Answer 11059

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-11
- score: 3

<p>Gosselin07, there is no way to answer your question based on a post on a discussion forum... To answer, a good architect with deep knowledge of the programming language you're using would have to deep dive into your codebase.</p>

<p>But in general, my take is it's almost never a good idea to rewrite a codebase from scratch. Joel Spolsky wrote a <a href="http://www.joelonsoftware.com/articles/fog0000000069.html" rel="nofollow">classical piece on rewriting codebases</a>, which I think you should read.</p>



## Answer 11058

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-05-11
- score: 1

Depends a lot on your technology and how good your architecture is in general. Sadly, 9% chance that the answer is "it sucks, architecture wise" and you get problems now with things getting more complicated all over the place.

Tell us a little more of what you did use ;) YOu have proper IDE's with refactoring support? A proper web framework separating logic and presentation and unit tests for all the logic modules?


## Answer 11074

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-05-12
- score: 1

All codebases are full of cruft; don't believe otherwise.

Just go forth and do what your customers want.  Chase revenue.  You can clean up some stuff later and the rest... that's software development, welcome!


## Answer 11060

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-05-11
- score: 0

Regardless of what you want to call it, if you rebuild from scratch, you've got another beta. You've learned a lot from the previous trial and gained user input, but it won't be truly tested until you get it in front of the users. Do you really want to put them through that again? You're agile; change should be easy ;)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
