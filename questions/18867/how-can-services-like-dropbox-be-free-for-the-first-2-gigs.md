## How can services like Dropbox be free for the first 2 gigs?

- posted by: [John Wright](https://stackexchange.com/users/-1/6545-john-wright) on 2011-01-12
- tagged: `cost`
- score: 4

I know that Dropbox sits on top of S3.  I want to provide a service that offers the first 2 gigs of storage free.  How are services like Dropbox and Evernote able to pay their data storage bills after offering so much free space to so many users?  Is that all paid for via ads?  Are there tricks to keeping the costs low?


## Answer 18871

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-01-12
- score: 11

<p>Almost all businesses have marketing expenses. The companies using this model view the direct expenses for serving their free users as a marketing expense, and make sure they benefit from their free users on growth, word-of-mouth marketing, network effects, etc.</p>

<p>The model is called "freemium". <a href="http://www.longtail.com/the_long_tail/free/" rel="nofollow">Chris Anderson's book "Free"</a> has lots of good information on the topic. You can also browse the <a href="http://answers.onstartups.com/questions/tagged/freemium">freemium tag here</a>.</p>



## Answer 18870

- posted by: [Mike Scott](https://stackexchange.com/users/-1/6167-mike-scott) on 2011-01-12
- score: 1

The main trick is that if 1,000 customers have copies of the same file, you only store it once rather than 1,000 times. But this can be difficult to combine with strong encryption. Apart from that, I think it's the paying customers rather than the ads that bring in the revenue. I'm not sure that Dropbox does use S3, but even if it does, a free user should only cost around 20 or 30 cents per month.


## Answer 18881

- posted by: [vellad](https://stackexchange.com/users/-1/4779-vellad) on 2011-01-12
- score: 1

As Jesper mentioned - it's similar to cross-subsidization.  If say (for example) only 20% of the Dropbox customers actually opt to pay then they are subsidizing the other 80%.

This is also how some online backup companies work - such as mozy.com and carbonite.com (they offer unlimited space plans).  They know that only a small percentage of customers will actually upload enough data so that they are making a loss on that particular customer - most of the customers upload much less data. The customers that upload much less data are therefore subsidizing the non-profitable customers.

Why would mozy or carbonite do that? Simple - the marketing messaging phrase 'unlimited backup' is very powerful and people choose that option and so they get many (and many) more customers.




## Answer 18883

- posted by: [jezmck](https://stackexchange.com/users/-1/6550-jezmck) on 2011-01-12
- score: 1

<p>Short answer: <a href="http://en.wikipedia.org/wiki/Loss_leader" rel="nofollow">Loss-Leader</a></p>



## Answer 18886

- posted by: [Chris](https://stackexchange.com/users/-1/6553-chris) on 2011-01-12
- score: 1

<p>If you listen to This Week in Startups episode 101 <a href="http://thisweekin.com/thisweekin-startups/this-week-in-startups-101-phil-libin-founder-of-evernote-com/" rel="nofollow">http://thisweekin.com/thisweekin-startups/this-week-in-startups-101-phil-libin-founder-of-evernote-com/</a> you can hear Evernote founder Phil Libin talk about conversion rates and the freemium model. It starts at minute 17.</p>

<p>He says that currently the conversion rates for Evernote members overall is 3% but that this figure is meaningless. In the first month only 0.5% will go for a paid account but the longer they stay with the service the more likely they are to sign up. For people who have been with the service for over 2 1/2 years 20% are paying customers.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
