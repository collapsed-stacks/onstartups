## How to increase mobile ad revenue

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-03-20
- tagged: `android`
- score: 14

I have an Android game in which I've included ads from Millennial Media and Admob. Between these two networks, my fill rate is consistently above 95%. Right now, I'm getting over 45,000 requests for ads per day, and I'm starting to see exponential growth. But, my eCpm for both Millennial and Admob is ridiculously low. Millennial's is $.12 and Admob's is $.01. I've been reading some other posts and it seems like people are getting between $1 and $4 per 1,000 views. How can increase mine? 

Thank you!


## Answer 33531

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-03-20
- score: 7

CPM is about the potential value of a customer.  If your content is about exotic fish, you'll get a higher CPM than content about goldfish.  On the other hand, you should get more impressions for the goldfish content.  You should really be trying to optimize M * CPM, not just M or CPM by itself.


## Answer 33532

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-03-20
- score: 5

I am using a network called MobFox to monetize most of my European & US traffic and I'm seeing terrific results, although the fill-rate is about 60% only.

I have set-up the following structure:

1st request: MobFox (i am using a feature called ecpmcontrol which they provide for developers who want to control their revenue) - overall eCPM about $1,90 for me

2nd request (if mobfox has no ad): iAds (low fill-rate but nice payout)

3rd request: AdMob - although I would recommend you use something like Mobclix or Smaato to backfill your un-filled requests as they have a slightly higher eCPM than Admob.

EDIT: I forgot to mention that your revenue and eCPM will also highly depend on your CTR. Mine is about 0,6% across all my apps.


## Answer 33534

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-26
- score: 4

What is your display time for each ad? We are using 30-60 Seconds. After that it can just be the title. We have games with low eCPMs like what you have reported and ones with 2-4 dollar eCPMs. The type of game seems to make a huge difference. Also for Admob the house ads and exchange ads are put into that fill rate but you are not getting any revenue from them. I would look closer at the reports under all ad types and find the real fill rate. Also do the math what is the revenue per click?


## Answer 36657

- posted by: [MattBuga](https://stackexchange.com/users/-1/16661-mattbuga) on 2012-02-28
- score: 3

Besides increasing traffic or picking up a new demographic (or making sure your ads are being properly optimized in the first place), you can get a better eCPM by shopping around with various ad networks.

If you give them some idea of how some of your stats are doing (current eCPM, traffic, fill rate, CTR...), they can give you an estimate of how others in your bracket are doing under their service before committing to anything. You may also want to consider using different combinations of ad networks as well.


## Answer 33535

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-10-22
- score: 2

<p>I have both <a href="http://www.admob.com/" rel="nofollow">Admob</a> and <a href="http://www.airpush.com/" rel="nofollow">Airpush</a> ads in my app. The Admob ads take up real estate on the screen whereas the Airpush ads are much more developer friendly because there was no modification to any layout files.</p>

<p>The push ads monetize great by sending messages to your notification bar just as Google+ plus and Facebook or Twitter apps do.</p>



## Answer 51464

- posted by: [Kaitlin M](https://stackexchange.com/users/-1/28368-kaitlin-m) on 2013-10-22
- score: 1

<p>I would say to get a higher eCPM you need to be in control of 3 things. Your own integration, which advertisers are showing, and which ad networks are providing them. </p>

<ol>
<li><p>Integration. Are you using the right ad format for your app? In most cases, banners will have a really low eCPM for example. Use something that shows at the right, non-intrusive, time , for example a recommendation to check out a list of new games after a game over screen.</p></li>
<li><p>Advertisers. I am not familiar with all ad networks, but choose one where you can see the eCPM for every advertiser and allocate your traffic only to them.</p></li>
<li><p>Ad networks. You are obviously already trying a few. The easiest way is to use ad network mediation that lets you see which networks are supplying the ads. You might find that 2 networks are supplying ads for the same app, but the eCPM from one is better. It might be the other network is taking a higher cut.</p></li>
</ol>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
