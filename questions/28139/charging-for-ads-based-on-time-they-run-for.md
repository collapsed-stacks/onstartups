## Charging for ads based on time they run for?

- posted by: [Derek Kwok](https://stackexchange.com/users/-1/12337-derek-kwok) on 2011-07-30
- tagged: `advertising`, `business-model`
- score: 0

I was wondering if there is such a thing as "Pay Per Date Run"? - as opposed to Pay Per Click or Pay Per Impression. For example: paying for an ad to run on week 31 - August 1st to August 7th for x dollars. 

If people have already implemented such a system, how does bidding work? (e.g. bidding for week 31 of advertisement placement). What about not going with bidding and negotiating with people looking to advertise directly? Are there other forms of price determination for ads?

**Motivation:**

The website targets a very niche market and only a specific group of people will be browsing, so the advertisements placed on this website is applicable to all of the website's audience.

I don't mind if it yields less revenue than going with PPC or other forms of advertisement. 

Our startup is looking for a very simple method to monetize a website and would like to build an in-house advertising framework. We want to stay away from going to third party for PPC.


## Answer 28148

- posted by: [Jay Neely](https://stackexchange.com/users/-1/1801-jay-neely) on 2011-07-30
- score: 3

<p><a href="http://www.reddit.com/ad_inq/" rel="nofollow">Reddit's self-serve advertising</a> resembles what you're describing. Advertisers bid a dollar amount per day they want their advertisement to run. On each day, the bids from all advertisers for that day is totaled, and impressions are allotted proportionately. So if:</p>

<ul>
<li>Advertiser 1 bids $20 for Monday </li>
<li>Advertiser 2 bids $40 each for Monday and Wednesday  </li>
<li>Advertiser 3 bids $40 each for Monday, Tuesday, and Wednesday</li>
</ul>

<p>Then: </p>

<ul>
<li>Monday - Advertiser 1 gets 20% of all impressions, Advertiser 2 gets 40%, Advertiser 3 gets 40%.</li>
<li>Tuesday - Advertiser 3 gets 100% of all advertising impressions</li>
<li>Wednesday - Advertiser 2 gets 50% of all impressions, Advertiser 3 gets the other 50%</li>
</ul>



## Answer 28232

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-08-02
- score: 1

I think a lot of bloggers and podcasters do this. For example we bought a one-week sponsorship of the [Daring Fireball](http://daringfireball.net/) blog for $5500. I'm pretty sure that the owner of that site just started with a price he picked at random and then he quietly increases it whenever he feels like his "inventory" (of weeks) is sold out, and lowers it if he thinks he can't sell inventory.

Essentially what you'll get if you try this is a few advertisers kicking the tires and expecting a very good return on investment.

You have to be careful about really using an auction. The price might get so high that nobody finds advertising worthwhile. When this happens, you'll still get a few experimental advertisers, but they'll never come back. You'll think that you're charging the PERFECT amount because you've got a selection of different advertisers every week, all paying top dollar, but in reality, every single one of them is getting disappointed by the results. So while you think you're building a great business, you're actually just running through every possible advertiser "burning" them on your model.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
