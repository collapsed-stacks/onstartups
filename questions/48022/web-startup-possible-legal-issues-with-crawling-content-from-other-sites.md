## Web startup - possible legal issues with crawling content from other sites

- posted by: [arahant](https://stackexchange.com/users/-1/25436-arahant) on 2013-03-15
- tagged: `legal`, `website`
- score: 0

We are building a website which will aggregate listings from various other websites. I would build my website to add extra search filters and other useful tools around this content that the other websites lack.

We will only display the other site's listing's header and short description. The users will be redirected to the listing on the other sites when they click on the header.

Apart from viewing the other sites listings, users can create listings on our website as well. I do not plan to give any preferential treatment to our listings over other site's listings.

We do plan to show ads but they will be shown neatly on one side (like kayak.com) and there will be no ads mixed with the listings.

I assume I can expect Cease and Desist letters from some of these sites. How should I handle them? Will having ads cause issues? What other issues can I expect apart from these 2?

EDIT: I assume robots.txt is an informal deterrent? I can see sites which disallow all content to all user-agents/crawlers but Google still crawls them. 


## Answer 48023

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2013-03-15
- score: 2

Just read the terms of service for the sites you intend to aggregate. Some will prohibit it. Many will require a separate license and/or payment. Some may have useful API to make it easier.

I assume you are going to do something more compelling than Google already does.


## Answer 48024

- posted by: [user239558](https://stackexchange.com/users/-1/14373-user239558) on 2013-03-15
- score: 1

If the content is restricted by a [/robots.txt exclusion](http://www.robotstxt.org/), then read the terms of service *very carefully*.

If the content is not restricted by [/robots.txt](http://www.robotstxt.org/), just go ahead.

Google and other search engines have been through this.  It is impossible for them to manually read all terms of service, that's why we have the robots.txt standard.



## Answer 48077

- posted by: [user25520](https://stackexchange.com/users/-1/25520-user25520) on 2013-03-18
- score: 1

Websites are considered as creative works and are protected by several elements of intellectual property laws. Source code and algorithms are protected by software laws i.e. copyright and patent when applicable. Contents are protected by copyright if they are “originals”. In the European Union, data are protected under computer databases legislation (http://en.wikipedia.org/wiki/Database_right). 

Aggregating listings from various websites could generate conflict with copyright and database protection. A recent example is the case opposing Google to Belgian newspapers with regard to Google news aggregation service (http://news.cnet.com/8301-1023_3-57559146-93/google-settles-copyright-dispute-with-belgium-newspapers). 

You should bear in mind that under copyright laws, reproduction acts that are not expressly authorised by the author are prohibited. You should always refer to the terms and conditions and license agreements provided with a website. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
