## Options for targeting advertising on iOS devices

- posted by: [MrDatabase](https://stackexchange.com/users/-1/15872-mrdatabase) on 2012-02-14
- tagged: `advertising`, `mobile`, `niche`, `target-market`
- score: 5

I'd like to put targeted ads in my free iOS application. My app serves a relatively niche group (say hobby fisherman). **What's the best ad network to use?**

I've used Admob and Apple's iAds in other applications. The targeting was seemingly non-existant. For example users of a casual game were shown ads for banks, cell service providers and random unrelated apps.

When looking at websites aimed at a similar niche I noticed very relevant ads (from Google/DoubleClick). So I'm wondering which ad networks allow the user to specify a niche or even individual companies for the ads to show.

**Edit**: looks like Adsense keywords can be specified in [Google's DoubleClick iOS SDK][1]


  [1]: https://code.google.com/intl/pt/mobile/afma_ads/docs/ios/doubleclick/#afma-options


## Answer 36386

- posted by: [Merlin](https://stackexchange.com/users/-1/6104-merlin) on 2012-02-20
- score: 3

In case of niche apps, the free is usually not the best way to go (think about it - eCPM you could get with a well positioned app is $1, how many users would you need to earn $3000/month?).

I mostly do niche apps, and if I make one free, I put in in the ads for my other apps / products. I think this is the way it's usually being done.

I'd suggest switching to a paid app.


## Answer 36656

- posted by: [MattBuga](https://stackexchange.com/users/-1/16661-mattbuga) on 2012-02-28
- score: 3

Ad networks use different optimization methods, so it's hard to say.

It may be more important to look towards a more independent ad network who will give you better service and support, since it sounds like you might need some nuanced help or customization with what you're trying to achieve.

I'd recommend researching a few online and seeing what they offer as far as targeting and optimizing ads. You can even use a few ad networks at a time to leverage your inventory to see how things work out.


## Answer 45153

- posted by: [Sven Mohackla](https://stackexchange.com/users/-1/22171-sven-mohackla) on 2012-12-19
- score: 2

I've been working with free apps now for the last 3 years, many of them in top position in Apple appstore, Google play and Windows Phone, with several hundred million impressions per months, here are my 2 cents.

**First off, we start with iOS and Android:**

Choose a ad mediation network rather then a single ad network.
And ad mediation network let's you use several ad networks at the same time.

Some example of ad mediators are:

- [MobClix](http://mobclix.com)
- [MoPub](http://mopub.com) (disclaimer; I am a customer)
- [Burstly](http://burstly.com)
- [AdMob](http://admob.com) (dislaimer; I am a customer)

Now a days many networks cooperate, so for example millenial and other networks are also starting with mediation.

When you chose mediation, there are a couple of things that you should consider.

- Want to be engaged?
Me personally I like to keep a tight tabs on things and monitor the networks
on a daily basis and steer the traffic to the network that I think pays best
for the moment. This of course is very time consuming, but you're in full control of you ad revenue. If you have a lot of monthly impressions and users (I'm talking over 50 million or more) then it can help to get a key account manager at the ad network and negotiate the rates.
Ad networks are of course depending on apps with high volumes, so that they can boost to their advertisers on how good they are. For me mopub.com was a good fit, because I can configure and steer this on my own. Their user interface is not the easiest, but if offers up quite a lot of good configurations and they offer integration with plenty of the big names. Plus that mopub have their own ad exchange that pays pretty well.

- If you don't have the time (I don't need to develop, so I have time to cater for the ad mediation) because you're busy improving on your app to get more customers, then there are the ad mediators that take care of this for you. mobclix.com does pretty much the same thing as mopub, with the difference that they do the optimisation for you. You just setup your app, configure which ad networks you want to use and press play. They mobclix will prioritze the networks for you, in the way that you will get most revenue from it. They also have a functionality for you to optimize yourself if you want to. burstly.com does this as well, but haven't been using their service.

**Windowsphone**

This is a bit tricker, since there aren't that many networks available. And I haven't found any ad mediator for Windowsphone. Let me know if you find any :)
Here I use ad rotator together with Smaato, adduplex and Microsoft pubcenter.

**Worth a mention**

There are some other services that are not exactly "ads", but they are close enough
and are pretty cool.

[Kiip.me](http://kiip.me) - Reward based system. If you have achievements in your app, your customers could get rewards from this network. Pretty cool idea and I want to try this as soon as I have the achievement system in my apps.

[PlayHaven](http://playhaven.com) - This is a pretty cool platform that offers up a lot of great services, so that you don't have to write them yourself. They have cross promotion systems and some other nice features, worth a checkout.

Hope this gives you some good ideas!
Good luck and feel free to ask me questions, I'm in no way a monetization expert, just willing to share my experience and learn something new on the way.

 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
