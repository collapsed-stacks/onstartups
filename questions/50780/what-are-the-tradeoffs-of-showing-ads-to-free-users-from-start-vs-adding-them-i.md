## What are the tradeoffs of showing ads to free users from start vs. adding them in later?

- posted by: [rbwhitaker](https://stackexchange.com/users/-1/15024-rbwhitaker) on 2013-09-04
- tagged: `business-model`, `freemium`
- score: 1

Suppose I have a web application where the intention is ultimately to go the freemium route, with some users paying for extra features, and others having a smaller set of features for free, while being shown ads. In the early days, there would be no premium version available, so everyone would be on the free version until more functionality gets built.

(For the record, I have no delusions of ad-supported software making me filthy rich. I'm very aware that ads don't usually bring in vast sums of money, but I'm hoping that it can help to offset the costs of what could be a fairly storage and bandwidth intensive application.)

In the early days, I'm more interested in getting early adopters than in getting income, and as such, it may be better to go ad-free to start. However, having no ads may set the expectation for people. Later on, when the free accounts become ad-supported, it may backfire, with people frustrated with "all of these ads popping up all the time."

So my question is, **what are the consequences and trade-offs (good and bad) of having the free accounts in a freemium model be ad-supported straight from the get-go vs. having no ads initially, then adding them in later?** I'm not asking anyone to tell me what I should do, specifically, just to guide me on the various points and counterpoints to consider when making this decision for myself.


## Answer 50785

- posted by: [john 4d5](https://stackexchange.com/users/-1/21439-john-4d5) on 2013-09-04
- score: 2

As you want to scale, the **better strategy is adding advertisements latter.**

Your web application will be more attractive / user friendly.

If you deliver value for your users, after gaining a good volume, you can add the advertisements. **If you are able to create and deliver that value and the users can feel it, do not worry that much about frustration/initial expectation, they won't stop using your app because of the ADs**.

**Giant Internet companies did and do the same strategy.**
Facebook was launched in 2004, but it was 2008 when the team had the conclusion that advertising would be the main source of monetization, then, Facebook made many changes to its advertising model with the aim of achieving profitability. And it keeps changing every month.

Youtube started advertising just one year after its creation, and continued to add different forms of ADs as time goes by, some of them are very recent. The same applies for other products like Gmail and so on.

**Scale your website, make the users use it and feel the values of it, then you do not need to be afraid of adding advertisement.**


## Answer 50793

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2013-09-05
- score: 1

We all understand the freemium trade-off. So if that's your route, **show ads from the get-go**.

But *you may not want to start serving your ads from a network*.

It's usually obvious when an ad is from an app that's new and has few users - you're given a lot of lousy ads and ones that are just ubquitous, where big-hitting apps are serving ads that want to connect with that community. So, given that there are only cents at stake, go find an internal ad serving library or roll your own. (By internal, I just mean one that serves images and links you control, rather than one that connects to an ad network.) 

Now find some nice ads that fit your demographic and aspirations, and make sure you can find a link that takes the consumer to a viable endpoint (i.e. don't copy a link that is part of an ad platform's monetization workflow) for the brand concerned. You don't need lots, just enough that a user sees different ads from time to time.

Of course, if anyone at the brand gets upset that you're showing their ads in a way that could get them consumers and giving them any clicks for free, you're only too happy to stop, right?

So, *why go to all these lengths*?

1. When you make a change, it makes a difference. So if you start without ads even though you know will some day, you're choosing to disturb your existing users, because they never saw ads in your app before. In other words, in the success case (you grew enough to want the ad revenues or/and the premium upsell dollars), you have guaranteed a step backwards.

2. If ads are there from the start, there's no friction in the discovery or the install process. Maybe a few users will drop off when they see the ads exist in your free app. That's fine, because you didn't want those users, anyway, and having them unsustainably was an ego boost not an achievement.

3. From day one, you have the opportunity to have a paid app with one immediate benefit - no ads. You can introduce it whenever you like, you can A/B test, you have more than doubled your capacity to learn.

4. You force yourself to get good at the advertising trade-off - how to give ads sufficient prominence that you see revenues (by the clicks or by the premium upsell); while avoiding damaging the user experience that creates the value of your app for users.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
