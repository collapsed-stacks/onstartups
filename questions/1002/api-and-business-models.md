## API and business models

- posted by: [Mahmood Ali](https://stackexchange.com/users/-1/583-mahmood-ali) on 2009-10-12
- tagged: `business-model`, `monetization`
- score: 4

What is your take on content-provider web-service startups (e.g. Yelp) exposing an API to their content?  How does it affect the business model of the service and how can you monetize it?  What benefits does the API add to the services?

On one hand, it's great to have an API that external developers use to make their own mashups and target platforms that the startup doesn't have experiences/resources building (e.g. android, iphone), and get the brand name out.  On the other hand, they make it easier for scrapers to "steal" the content and hinders the typical business model of advertising.



## Answer 1018

- posted by: [raminf](https://stackexchange.com/users/-1/404-raminf) on 2009-10-12
- score: 4

I'm a techie-type so the first thing I do is make sure I have an API in place, then use the same API to build the front-face of the service (without exposing it publicly). I agree with Alain that you don't need to expose it until much later, but if your own app is hitting the same API from the start it gets stress-tested and you can then open it up later with confidence.

As for whether to expose it or not and worries about content, just realize that you'll get your content scraped once you have a public-facing HTML page. There's no way around it. But by offering the API you can throttle and monitor it so it's not abused. 

On the plus side, a well-designed third-party app that ties into your API helps build exposure and credibility (see Twitter, Yelp, Google, or Amazon). If your business model is based on number of registered users, then an API+third-party apps is a cheap way to acquire (and keep) active users. 

If revenue is based on ad-driven pageviews, then you could require in your TOS that third-party apps show all your content (including in-line ads) but don't expect mass adoption from devs unless you're offering a particularly unique service.


## Answer 1015

- posted by: [Alain Raynaud](https://stackexchange.com/users/-1/502-alain-raynaud) on 2009-10-12
- score: 2

APIs are typically something that come very late in your product, say one year after you start showing users.

Developers will not care about your APIs until you have a critical mass of users. So I'd say you have plenty of time to figure out the right strategy. Launch something useful to users first, iterate, then worry about APIs.


## Answer 15297

- posted by: [Eugene Osovetsky](https://stackexchange.com/users/-1/4870-eugene-osovetsky) on 2010-10-19
- score: 1

Opening your data as an API is generally a great idea, but only as long as you do it in a *controlled* way. Some benefits of API exposure:

- People who are willing to write code to use your data can be some of your best potential partners, potential customers, etc. Think about it - they are _really_ interested in your data! Often, the list of people who signed up to use your API is really the primary source of value that the API generates for your business.
- Many APIs have licensing terms that require developers to include links back to your site next to data obtained from your API. You can use this to generate traffic to your site (and charge money for API access for those developers who wnat a fully white-labeled solution)
- Finally, some high-value APIs can be monetized directly (e.g. pay-per-call) 

In any case, you want to maintain control over your API at all times:

 - You may want to control how much data you give out, to prevent someone from just stealing all of your data and just duplicating your site
 - You may want to put a license agreement in place for users of your data
 - You may want to only give the data to someone with a verified identity (e.g. email, telephone, etc), so that you can enforce the license agreement
 - You'll want to know exactly who's using the data (name, company, email, etc)
 - You'll want an easy way to start charging money for API access in case someone's willing to pay (e.g. wants to go beyond your free quota, or wants a special license / white-labeled solution) 




## Answer 1023

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-10-12
- score: 0

Agreed with Alain and Ramin.

One exception is if the API itself is part of how you sell or market the tool.

For example, creating an API so that it can plug into a popular tool, then selling that package as a plugin.  That's an entire business model which necessitates an API, regardless of how else you might display or monetize your application.

Even then Ramin is right about *having* an API and yet not *documenting* it until/unless it makes business sense to maintain and support it.  Where "business sense" means "people give you money for that purpose."


## Answer 1027

- posted by: [randfish](https://stackexchange.com/users/-1/105-randfish) on 2009-10-12
- score: 0

I never worry too much about the data attribution component of the API so long as the issuing site has a solid brand footprint and presence in both the minds of consumers and the rankings of the search engines. In fact, if done properly, an API can bring in dramatically more branding and links (which help with both traffic and search rankings). You just need to be careful about how you do the attribution requirements and have some level of enforcement (which can be as simple as watching how large data consumers are using the API).

BTW - We do this at SEOmoz with our Linkscape API, and by although we're not a big brand by any means, the free API distribution has definitely helped with branding, mindshare and links.


## Answer 15304

- posted by: [viv](https://stackexchange.com/users/-1/2665-viv) on 2010-10-19
- score: 0

API's are a neat way of popularizing your brand. It's more like opening up the back-end, which is not where the success of a web startup lies. However strong your back-end is, if the data isn't shown properly to the user (or) the website lacks in usability aspects, it's going to fail.

> It gets you a lot of inbound links which is good for your site since the credibility of your site in Google's eyes is increased

I don't think it's much of a threat - in fact it's a good thing



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
