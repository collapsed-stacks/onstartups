## How does Hubspot get Google statistics?

- posted by: [Dan](https://stackexchange.com/users/-1/1600-dan) on 2010-01-15
- tagged: `data`
- score: 1

Put your website into [Website Grader][1].  The free report they come back with has:

- Google pagerank
- Google indexed pages
- Last Google crawl date
- Traffic rank (from Alexa)
- Inbound links (matches neither Alexa nor Google links: operator)

How does Website Grader get this info?  Are they screen scraping?  Is it possible to get this information under a commercial license?

Do people have experiences to share about using screen-scraped data for their businesses?


  [1]: http://websitegrader.com


## Answer 6587

- posted by: [Dheer Gupta](https://stackexchange.com/users/-1/2052-dheer-gupta) on 2010-01-15
- score: 1

<p>Most of this data is easily retrievable using various APIs, ex. <a href="http://groups.google.com/group/google-ajax-search-api?hl=en" rel="nofollow">Google Ajax Search API</a>.</p>

<p>Furthermore, the links: method is not very accurate, rather the better way is to fetch the indexed pages, number; hint: the one found in Google webmaster tools.</p>

<p>Furthermore, I dont think a user initiated report request would anyways get classified as screen-scraping. though I am in no way qualified to comment on the legal aspects.</p>

<p>Also, perhaps you should take the technical/programming aspect of the question over to Stackoverflow.</p>

<p>Cheers!!</p>



## Answer 6589

- posted by: [Romy Misra](https://stackexchange.com/users/-1/2079-romy-misra) on 2010-01-15
- score: 0

It's interesting to see how they still get Page Rank. Page rank is no longer available publicly on the API and Google blocked SeoMoz from using Page rank data for their tool.

The rest is available from the various API's publicly. The links on Hubspot's report is from Yahoo Site Explorer.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
