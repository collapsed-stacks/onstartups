## On an e-commerce site, how do you attribute a sale to PPC if a visitor comes from PPC but then returns to buy through another website?

- posted by: [Nikolay Piryankov](https://stackexchange.com/users/-1/8046-nikolay-piryankov) on 2011-09-22
- tagged: `google`, `adwords`, `conversion`, `ppc`
- score: 1

Can we use cookies and if so how do we install this? What software could track this kind of conversion scenario?


## Answer 30452

- posted by: [Jennifer Simonds](https://stackexchange.com/users/-1/13461-jennifer-simonds) on 2011-09-22
- score: 1

Our site has a homegrown affiliate program. I set a 30-day cookie when they land on the site from the clickthru. The value of the cookie identifies the affiliate they came from; for a PPC ad campaign it would identify which campaign they came from.

Later when they order something from the site, we simply check if that cookie (still) exists. If it does, I write a row to a "clickthrus" table in the DB, and then a sales reporting page later queries that table for building its statistics on demand.



## Answer 30457

- posted by: [JonDiPietro](https://stackexchange.com/users/-1/11642-jondipietro) on 2011-09-22
- score: 0

<p>Google released <a href="http://analytics.blogspot.com/2011/08/introducing-multi-channel-funnels.html" rel="nofollow">multi-channel funnels</a> last month. It will track all of these various channels.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
