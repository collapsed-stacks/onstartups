## Releasing software in different countries

- posted by: [SmartCompanySoftware](https://stackexchange.com/users/-1/1629-smartcompanysoftware) on 2010-01-05
- tagged: `software`, `strategy`
- score: 1

I'm writing a software application that will be used by fostering and adoption agencies/organizations that I plan to sell in English speaking countries (at first). The application is a desktop application which is specialized and therefore I will be charging for the software, support, and maybe training (in the form of videos or in person). I don't expect it to be software that you simply download, install and off you go.

I expect each country to have slightly different (regulatory) requirements and sets of rules for recording data and although I don't expect there to be huge differences, they will be different enough to affect some screen designs and database tables. There will also be issues with how I reach my customers in different countries from my current location.

I'm an experienced software developer, but I've not written software that can be used in different countries before, so I'm trying to figure how best to proceed.

Currently, I'm writing for the UK market, but would like to sell the application in the US, Canada and Australia. I want to build in international support early on, rather than leave it until later as I expect to target different countries, so it makes sense to factor that in to the design now.

I'm not looking for technical answers, I just want to hear peoples ideas and potential strategies.

 - Do I have one program that can be used by all?
 - Do I have different programs for each country? (this will have a maintenance overhead)
 - Do I concentrate on one market first or try and target more than one market now?

The easiest solution for me at the moment is to target one market (UK) and structure everything around that and once that is up and running, then start to break it out into separate applications or make modifications for each country. Maybe I'm thinking too far ahead about different countries and I should address that later?

What are your thoughts?


## Answer 6001

- posted by: [phaedrus](https://stackexchange.com/users/-1/250-phaedrus) on 2010-01-05
- score: 0

I would also prefer to start early to build relationships in various markets. I would favor non-cash basis for marketing and sales relationships, such as shares and revenue-sharing agreements. Besides an expanded market, this also mitigates the risk associated with just one market. 

For development, it would be good to talk with system integrators in that market.  

Overall, the horizontal expansion (in terms of markets) has to be balanced with the vertical depth. As soon as I have a validated prototype, I'd start with the horizontal expansion, particularly since it would take quite some time.


## Answer 6008

- posted by: [Fernando Martins](https://stackexchange.com/users/-1/1778-fernando-martins) on 2010-01-05
- score: 0

Adrian, I also have a software "problem" similar to yours.

Here's what we've (me and my partners) done:

1. Kick-off and concentrate in one country at first. This dramatically reduces the cost of sales, support and maintenance. The support and maintenance is specially high for early versions where some bugs must be killed and a new version must be deployed as fast as possible.

2. In my case the same software suits all countries, but I did got special requests from some customers. If you don't know your answer yet, you should be prepared for the worst case scenario, since most probably the rules differ from country to country, plus some agencies will probably request some customization. This is another point for 1., it will increase your support and maintenance cost even more.

3. If you're going to have live support (like phone calls), you should account for the different countries time zones. This may imply you having someone around-the-clock that speaks all native languages from the working hours of each country. If you don't have live support, you still may need different language speakers if you plan to go out from English speaker countries.

4. Like in 3., documentation also needs to be localized. This may be easier than support, since the support people may translate it or you can get a translation service, there are many companies specialized in software translation out there.

5. Selling on other countries may require different techniques and probably someone native. Having a partnership may be a strategy, it may even reduce your support cost if your partner assumes the local support.


## Answer 6009

- posted by: [Peter Olsson](https://stackexchange.com/users/-1/2161-peter-olsson) on 2010-01-05
- score: 0

I would concentrate the development resources on the market(s) you know first. You need a couple of customers before your software turns into an application (rather than building custom solutions for each customer). It is a lot easier to find the customers willing to work with you in a market you know.

It does take time to find good partners in other countries so start looking for them right away. Discuss if their markets matches the markets you already know. Any competitors etc? You will need both the information and the contacts in the future.

I wouldn't worry too much about how to structure your application. The answer will probably be obvious once you know all (or most of) the differences. If all forms and all reports differ (different data requirements) you will have to go with different applications rather than different settings.

If you get an opportunity to expand into a market early (the right partner, more than one customer etc) - take the chance. It will diversify your development, but the it is probably worth it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
