## Question from a start-up ratings site. how does yelp assign price ratings?

- posted by: [user25771](https://stackexchange.com/users/-1/25771-user25771) on 2013-04-05
- tagged: `webapp`, `review`
- score: -1

e.g. restaurants are rated as $/$$ etc.  Menupages.com does the same.

We are building a specific kind of ratings site and want to add this feature.  Just wondering if this is a manual process or a formula based on the avg cost of a meal/room.  Any guidance is much appreciated.


## Answer 48411

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2013-04-05
- score: 0

It is likely to be some ranking formula, based upon an "average" purchase. For example, a hotel will be for one double room, while a restaurant will be for two courses, etc.

If you have a big data-set it is trivial to work out the ranking boundaries, but otherwise you could just assign reasonable ranges and adjust later if necessary.

Alternatively, crown-source it by asking your visitors to vote.


## Answer 48416

- posted by: [happybuddha](https://stackexchange.com/users/-1/25346-happybuddha) on 2013-04-05
- score: 0

<p>They clearly use their own rating/sorting mechanism. There is a lot of info <a href="http://www.yelp.com/faq" rel="nofollow">here</a></p>



## Answer 48417

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-04-05
- score: 0

<p>There is a whole science behind <a href="http://en.wikipedia.org/wiki/Reputation_system" rel="nofollow">reputation systems</a>. Understanding and setting rules about freshness, validity, and attack protection are important if the system is going to be more than a simple graphic. </p>

<p>There is a good oreilly book on <a href="http://shop.oreilly.com/product/9780596159801.do" rel="nofollow">reputation systems</a> by farmer and glass worth reviewing. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
