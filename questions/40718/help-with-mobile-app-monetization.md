## Help with mobile app monetization

- posted by: [SundayMonday](https://stackexchange.com/users/-1/15881-sundaymonday) on 2012-07-21
- tagged: `monetization`, `mobile`
- score: 5

I have a free iOS app that's popular in a modest sense. Daily active user count has been growning steadily: it's approximately doubled over the last 6 months. At the moment it's around 2100 daily active users. I'm trying to monetize the app and I'd like some help as I haven't been successful so far. 

I tried selling the app for $1. That resulted in 3 sales in a day. Normally the app gets 80-100 downloads per day.

I've integrated Apple's iAds and the results are pretty poor. $20 in revenue for 12k impressions over about a week.

I added AdMob ads that I can toggle on/off remotely. However the update hasn't gone live in the store so I don't have any numbers.

I'm currently porting the app to Android because I think there will be lots of users and some decent ad revenue but who knows.

I've considered selling ad space directly to the companies in my particular niche. **Any thoughts on how to monetize an app with this modest but growing traffic?**

Note: I can set an image + link for the ad view remotely. I've considered linking to my other paid apps (should try this) and even selling t-shirts from Zazzle or something.




## Answer 40725

- posted by: [Johannes Rudolph](https://stackexchange.com/users/-1/11487-johannes-rudolph) on 2012-07-22
- score: 5

There's plenty of advice on app monetization floating around, but unfortunately not a whole lot of hard data. 

I don't know how reliable your datasets are, but for te sake of illustration, let's quickly calculate Monthly-Recurring-Revenue (MRR). If you sell at 1$ and substract commission you should receive 0.70$ per sale. 0.70$ * 3 Sales/day * 30 days = 63$ MRR. The ad-based version does currently generate 20$ a week, that's around 80$ MRR.

Ok, current MRR is one thing. You would also need to consider the growth model behind each of those monetization strategies. If you can predict that to some degree and calculate the Net-Present-Value of the Cash-Flows, you would have a pretty solid base to pick a decision.

Skipping this part for lack of data, here are some thoughts and guidelines that might help you pick a decision:

**Usage model:** ***Sticky*** apps tend to be used again and again (like Weather Apps). Usage of ***trendy*** apps quickly levels off after an initial period of heavy usage (most Free games fall into this category). Sticky apps tend to work well with advertising, while trendy apps are more suited to paid/in-app. Based on the data you have shared (12k page views for 2.1k downloads is an average of ~6 per user) it seems your app is sticky.

**Willingness to pay:** Customers have a fixed willingness to pay for a certain kind of app. It's unlikely you can change their mind. You have already done some basic testing (free vs. 1$) so you know a little part of the demand curve - doesn't look to good. But maybe you just have a conversion problem.

**Conversions:** Try offering a paid upgrade. Even if the only bonus feature is to get rid of the ad's (try making them a litte more annoying to motivate people for upgrades). If your app is sticky, this will work well. Make upgrading a seamless experience. I'd recommend In-App-Purchases because they are quite simple to implement and you don't need to build and maintain two versions of the same app. Requires some effort on your part.

**Customer archetype:** You mentioned operating in a niche. Is there anything specific about your typical kind of customer that you need to consider when choosing a monetization strategy? In my experience, In-App-Purchases do only work well with "experienced" customers that have done IAPs before. Can you offer them special incentives to upgrade? 


## Answer 45057

- posted by: [Bubbleware Technology](https://stackexchange.com/users/-1/22112-bubbleware-technology) on 2012-12-15
- score: 1

Honestly, my experience has been that you're better off taking what you've learned from your previous app and using that knowledge to create another app.  

I spent way to much time trying to position, optimize and promote my first app with mild success that had no variance on the success.  I also tried making a paid and lite version to make money off ads.  Max income was up to ~ $20/mo at most.  My second app hit a target niche better and was up to ~$200/mo at peak. 

This is coming from experience building 2 apps personally which are in the marketplace and a handful of apps for fortune 500 companies.  

Also - remember to translate your apps to every language, you never know if it will be a success in another country.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
