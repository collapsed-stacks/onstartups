## Google APIs - what's the story with their licensing?

- posted by: [Dr. Phil](https://stackexchange.com/users/-1/2223-dr-phil) on 2010-01-30
- tagged: `api`, `google`, `marketing`, `legal`
- score: 4

My new build package features a link with Google maps. However, having had a look at their terms and conditions, I am unsure exactly where I stand with integrating their tools within my chargeable SaaS package. I am sure a number of you have experience of this and can fill me on on what the actual situation is in the following three scenarios:

1. Users store data including zip codes in my system. I want a 1 click functionality where users can plot that address through google maps (nothing revolutionary!). Can I have a browser within the system that does shows this or do I have to set it up so it opens another tab in the browser? Is this also the case with Analytics? I know Dharmesh integrated with analytics - does this mean he pays a licensing fee
2. As above but want user to be able to plot multiple sites from their address book in my system in google maps (a bit like tripadvisor does in showing where restaurants are in a particular city) - how can you get around this within google's T&Cs?
3. I want to tie into the business address records listed in google maps API within my own interface. Google seem to say that they are ok with this if it available free through your website. Therefore, can I get around this if I take this feature and put a free version of it on my website. Obviously, the user has to pay to buy the rest of the my package but the part that uses their API is available free - does this get around it?

I obviously don't want/can't afford to pay the $10,000 licensing fee that they charge for starters so need to get a totally legal work-around

p.s. I realise no advice given to me constitutes formal legal advice and will not act on it without taking proper legal advice.


## Answer 7466

- posted by: [Sasha](https://stackexchange.com/users/-1/2032-sasha) on 2010-02-02
- score: 3

To make it short - if you are making money on your product which utilizes google maps you have to get license. <br>
We had similar problem and decided not to mess with google. <br>
Instead we found CloudMade.<br>
You can check how it looks in our application
http://www.askyourtargetmarket.com/surveys/16458/statistic/charts?share=dd435f852630d682275018ecd5b84dbc <br>
Switch to "By Location" under "VIEW OPTIONS".


## Answer 7392

- posted by: [PawelA](https://stackexchange.com/users/-1/2318-pawela) on 2010-01-31
- score: 1

We have had a similar issue with our service. This is what is my understanding of their rules:

According to "Google Maps/Google Earth APIs Terms of Service" (http://code.google.com/intl/pl/apis/maps/terms.html)

9.1 Free, Public Accessibility to Your Maps API Implementation. Your Maps API Implementation must be generally accessible to users without charge. You may require users to log in to your Maps API Implementation if you do not require users to pay a fee. Unless you have entered into a separate written agreement with Google or obtained Google's written permission, **your Maps API Implementation must not:**

(a) **require a fee-based subscription or other fee-based restricted access**; or
(b) operate only behind a firewall or only on an internal network (except during the development and testing phase).

the definition of Maps API Implementation is:

7.1 (c) "Maps API Implementation" means a software application or website that uses the Maps APIs to obtain and display Content in conjunction with Your Content, according to these Terms.

As far as I understand, if **any** of payable functionality of your service uses Google Maps API, you are violating their rules. I mean, you can use their API only if all functions connected with Google Maps are 100% free. At least that is how we interpret this in our service.


## Answer 7440

- posted by: [PawelA](https://stackexchange.com/users/-1/2318-pawela) on 2010-02-01
- score: 1

You might also want to look at other APIs. Google MAPs is not the only one accessible. I would also say it is not necessarily the best one in many cases. Please check those:

 - Bing Maps API - http://www.microsoft.com/maps/developers/
 - Yahoo Maps API - http://developer.yahoo.com/maps/
 - MapQuest - http://developer.mapquest.com/



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
