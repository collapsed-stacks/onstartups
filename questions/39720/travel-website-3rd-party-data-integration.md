## Travel website - 3rd Party Data Integration

- posted by: [iamjonesy](https://stackexchange.com/users/-1/11837-iamjonesy) on 2012-06-06
- tagged: `website`, `api`, `travel`
- score: 1

I'm creating a travel website that lets users select points of interest for a particular city (a restaurant, museum, etc.). These records are to be displayed on a google map as markers. This I've done already. 

My question is should I integrate with 3rd party data to make creating these markers easier, cleaner (no duplicates), and utilizing data (info, reviews, photos, etc.). If so, can anyone recommend what services are available? 

I want the user to be able to search for the point of interest (POI) and select it from a list. I'd like to be able to lookup information, reviews, photos, etc. too if possible. 

What are other travel websites doing? Did sites like trip advisor, virtual tourist, start with nothing and build their data from scratch?


## Answer 39723

- posted by: [Michael](https://stackexchange.com/users/-1/17905-michael) on 2012-06-06
- score: 1

<p>Yes, I think an integration of third party services here would be very helpful. Google's <a href="https://developers.google.com/maps/documentation/places/" rel="nofollow">Places API</a> or the <a href="http://www.yelp.com/developers/documentation/v2/overview" rel="nofollow">Yelp API</a> may offer what you are searching for.</p>

<p>I also think, that starting with an empty website is not good. You may add the first x points yourself and maybe offer a nice reward for the first other editors of new places. That's how <a href="http://www.qype.com/" rel="nofollow">qype</a> did it. I created 30 or 50 entries there and got an ipod as reward. Of course only the first 100 or 500 users or so got those rewards, so predicting your expenses is very easy.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
