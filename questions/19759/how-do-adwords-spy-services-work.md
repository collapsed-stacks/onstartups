## How do AdWords spy services work?

- posted by: [Tony_Henrich](https://stackexchange.com/users/-1/5619-tony-henrich) on 2011-02-03
- tagged: `advertising`, `competition`, `adwords`
- score: 5

There are several services like SpyFu, AdBeat & ispionage which advertise they can provide the keywords, budget, ad copy and other information which competitors use in different ad networks like Google, Bing.. etc. This seems like inside information.

1- How do these services get their information? Do they monitor the ads for extended periods of time and figure stuff out?

2- Are there any open source projects which are based on similar functionality?

 


## Answer 19796

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-02-04
- score: 2

Most use some sort of bot to scrape results, which monitors a set of keywords and see's what ad's appear. They are very much just a "guessing tool" as unless they have a genuinely massive crawler system with regional presence they are just seeing regional ads for the area the crawler is in. They are also ratcheting up the number of impressions over the period of time they are running, so maybe in some ad system increasing the Cost especially as ad's with low click through rates tend to get lower quality scores resulting in higher clicks, the longer the period of time the more likely they are to get a relative basic picture of competitors. Very much an industry he with the largest database of keywords and searches will have in theory the best chance of being closest in the guessing game.


You may find this article http://www.seoptimise.com/blog/2008/09/4-ways-fool-your-competitors-using-spyfu.html of some use to you. As for open source alternatives, their are plenty of scrapers out their that can be used.


## Answer 19891

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2011-02-07
- score: 0

- Prepare a list of words and phrases. Some Natural Language Processing knowledge is required here. 
- Extract from Google what phrases have higher advertising costs. 
- Sort by advertising cost and regularly search Google for most expensive phrases.
- Scrap search results and fill in database.
- Make some model that allows to predict exact result based on sparse sample.
- Predict for all phrases and words.

... or something similar.

Some services collect data directly from Internet users via toolbars that spy on search results.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
