## Show competitors prices on e-commerce site, legal issues?

- posted by: [James](https://stackexchange.com/users/-1/10239-james) on 2011-05-04
- tagged: `marketing`, `website`, `sales`, `ecommerce`
- score: 3

I am starting an ecommerce site selling electronics in the UK. I belive I can compete with price against others in this field, and was considering have a 'price compare' table on the product pages which I know other retailers stock.

  I wondered if anyone could help me address my concerns:

 1. Can I legally do this in the UK. (I will be showing the date and time prices were scraped.)
 2. Can I use their logo without their permission, or should I just use their name.
 3. I want to use my main competitors only, would I get in trouble for excluding a competitor if they had lower prices than myself?

  If I was not the lowest priced for the product, I would have pointers saying 'Have your checked their shipping prices too?' or 'Do they offer an equal customer service?' to avoid just passing competitors 'warmed up' customers.

Thank you very much for your help!


## Answer 24480

- posted by: [edralph](https://stackexchange.com/users/-1/9362-edralph) on 2011-05-05
- score: 3

**Can I legally scrape prices...**  it depends on whether you are contravening their terms and conditions of use.  If they don't have anything on their website saying that you cannot use automated 'crawlers' then you're ok for a while, but it would only be a matter of time before they saw your website, saw you were showing their higher prices and they ask their IT guys 'how the heck do they do that?'  The IT guys tell them 'it's just a spider that is going around scraping prices from every single product page on our website', the management says 'how do we stop them', and the IT guys say '1. block the crawlers IP address, 2. block it on the user-agent string of the crawler, 3. block it on the basis of non-human activity (load balancers/WAF devices can do this)'.  So you run the risk of very quickly running out of a scalable means of scraping their prices.

**Can I use their logo without their permission...**  if they don't like what you are doing (probably) they'll send you a cease and desist.  They could get their lawyers to get heavy with you even if you just used their company name on your website (it'll be a registered trademark).  So just using their name instead of the logo won't get you out of hot water.  Sorry.

**Get into trouble for excluding a competitor...**  only in the eyes of the visitors using your site.  Earning trust and reputation is about being honest and open - if they suspect you are deliberately trying to exclude prices of a competitor because actually they are lower, your credibility will soon drop and they'll leave your site.

Hope that helps.


## Answer 24528

- posted by: [Andy Carlson](https://stackexchange.com/users/-1/10270-andy-carlson) on 2011-05-06
- score: 0

I would avoid mentioning or showing their exact name or logo on your website. First of all, there are so many IP lawyers out there who are willing to make a buck on any case.
Your competitor might hire one of them and harass you.
If you have a lot of money to dispute that lawsuit, go ahead and do it.
Otherwise, just use other way to indicate that you are talking about your competitor so that people can figure out who you are talking about.



## Answer 29644

- posted by: [Mike](https://stackexchange.com/users/-1/11945-mike) on 2011-09-03
- score: 0

I think the question should be: Should I include my competitors price and/or name?

There are a lot of potential problems that can come up when you're doing this. You could be increasing their brand awareness, you could inadvertently upset a potential customer enough to get them to go to your competition who doesn't agree with your practices. This is a more important consideration if you're the market leader.

I personally don't see an issue if you're listing prices coming from your competitor(s) without naming them, but if you include their name/logo, you may be giving them free advertising (This all assumes they don't have robots.txt explicitly disallow you from doing it).

In regards to your more legal question. I hate to say it, but you really need to seek a lawyer who specializes in this area as your local laws may be different from the laws in my country. Get them to check the law that applies to reviews (particular in cases that you are reviewing a competitor) and possible problems with trademark infringement since you are possibly looking at profiting on their brand/trademark.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
