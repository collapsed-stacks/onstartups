## How do I price my expensive software and charge $100,000 in a presentable way?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-16
- tagged: `sales`, `pricing`, `b2b`, `software-licensing`
- score: 7

We have a software product that increases productivity of engineers and allows them to build/prototype new products. It costs $25,000 to use it for 3 months. A big name company is interested. How do I price and sell this software to them?

For starters, I read this yesterday and strongly recommend it:
[Joel on Software: Camels and Rubber Duckies][1]

Initially, I planned on charging $25,000 for a site license, but then I checked the customer and saw that they have many groups who could potentially use the software. I changed my plan to charge **1-5 seats at $25,000 for 3 months**. It makes $100,000/year. The software is complex and charging $100,000 per year will only cover a portion of our operational costs.

There is another large company who does software with different functionality but similar category, they charge $10,000 - $20,000 a year per seat, which is not too different from my model. They make $100,000/year for 5 seats. 

Since this will be a 5-seat license, when I present the price, I plan to further split this **$25,000/5 seats * 3 months = $1,666 per person-month.**

All of a sudden, the price of $100,000 which is mentioned in Joel's article as ***dearly*** gets very close to the range of ***cheap***, when you look at it as per-seat/per-month.

Going further, for $1,666/per person-month to be a sensible price, I must show that I am saving the customer the engineering costs of at least $1,666/per man-month so that it is well justified.

Maybe as a simple hack, I should increase the number of seats? If I make seats 1-8, it makes: $25,000 / 8 seats * 3 months = $1,041 per man-month. The cost/benefit ratio for $1,041 is easier to justify.

To further improve the perception of cost, I could make the price $999. There you go, now I am presenting the price of $999/man-month, at a minimum 8 seats. In grand total it makes:

**$999 * 8 * 12 = $95,904 per year**, nearly the original of what I expect to charge a year.

Does this sound reasonable?


  [1]: http://www.joelonsoftware.com/articles/CamelsandRubberDuckies.html


## Answer 23536

- posted by: [Bob Murphy](https://stackexchange.com/users/-1/5778-bob-murphy) on 2011-04-17
- score: 9

>We already spent years of engineering work and price was the last issue we thought about.

Yikes! Well, we made the same mistake in my first startup, and I hope yours goes better than that did.

You need to figure out what it's worth to your customers, and price it accordingly. And as a marketer once told us in that startup (and we were damn fools not to listen), you need to know who your customers will be, down to the color of their shoes.

One example of a tool that "increases productivity of engineers" is Coverity. Their static analysis tool is crazy-expensive and crazy-good. They charge per line-of-code-analyzed, and I think one of my recent employers was paying about $500,000 a year for it, but it probably saved them having to hire a half-dozen developers and even more QA staff.

As Brian says, if using your tool will save a company $2500 a month, you can charge some fraction of that. I wouldn't charge 80%, as he suggests - I'd go for 50%. But that's a judgment call.

----------------

As an aside, your hypervisor looks like really cool technology. But it's not clear from your web site what problems it solves - and I've been been involved in ARM-based embedded development for portable devices during the last five years. After thinking, I could figure some things out, but I shouldn't have to.

So you might want to add some sample "use cases" in simple, non-technical language - like, "Company X ran into this problem, and they solved it using our system and doing Y and Z with it."

Also, it appears you're targeting putting this on shipping devices. I can think of some good use cases for that. For instance, a cell phone could use your software to run two Linux instances, one to handle the phone and the radio and the power system, and one to handle applications and the UI. Then if the app handler instance has a problem, just reboot it and the phone will still work. Based on my experience in cell phone development, that could be worth big money to some manufacturers.

For inclusion on shipping devices, you should consider a per-unit-shipped royalty. That will probably need to be negotiated on a case-by-case basis.

In fact, I can only think of one use case that *doesn't* involve shipping on devices, which is to act as kind of a software ICE for ARM. But I think you'd need to add a lot to your offering to succeed in that world; otherwise, people would have to write the ICE-type capabilities themselves.

Do you have any competitors? What do they charge, and how?




## Answer 23531

- posted by: [Brian Karas](https://stackexchange.com/users/-1/8465-brian-karas) on 2011-04-16
- score: 8

It's hard to give a good answer from the vague info you've posted, but I will share one piece of advice when selling anything...

Once you set your price it should be something that you are proud of and can defend easily and without resrorting to crazy examples.  If you can clearly demonstrate that your software proves $2500/mo in value, then charge $2000/mo for it, and when you dis jess the price, present it like it is such a clear value that there is no logical reason to question it.  I don't mean that you should sound arrogant, but confident and slightly casual. 

Only you know all the specifics of your product, market and competition, so we can not give you much more than basic guidance.  


## Answer 23542

- posted by: [Matt](https://stackexchange.com/users/-1/8784-matt) on 2011-04-17
- score: 5

I can sum up my reservations in one word: resistance.

I don't know your market, or your likely competition, but reading your site for 5 minutes I'm not really clear what problems it's solving.  You do mention it as open source and downloadable for free and it seems has been so for some time.

If you're adding a layer to something you're giving away for free and charging $100k a year per seat, you had better be adding some truly spectacular value, or I'll download my own and set one of my team the task of adding a similar layer!

Anyway, what perceptions will a six figure SaaS price lead to, compared to say a $5k per user outright licence for the toolset?  Given your target environment, how will you enforce the monthly usage fee?

So what of perceptions to go with a $100k product?

Do you have a six figure website?  ...sales process?  ...marketing materials?  ...support and documentation?  ...premises?  ...testimonials?  ...company?  ...people?

Seems to me you need to get these to match up, or go into your first two or three sales at a much lower "partner" price so you can gain some use cases and testimonials to show your product truly delivers that level of value.


## Answer 23587

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-04-18
- score: 1

You're absolutely right that you can achieve business advantage by changing the structure and presentation of your pricing. 

However, there's a danger that you may have loaded this wrong.

To simplify what you've said, you have changed a core message from $1.7k per seat per month to $999 per seat per month, within essentially the same initial contract value of c. $100k. And you've also said that the client has many more engineers who could benefit from the software.

So there's a risk that in looking for an easier initial sale, you may actually have damaged your ability to achieve the revenue you could from this client. Because you are creating that lower expectation from the start, you may be setting yourself a price ceiling for additional business from the same client.

My maxim is that the *best* price is the *highest effective* price. If you see that per seat pricing is going to function as a point of reference, you need to challenge yourself to make that figure as high as possible while achieving the sale. 

If you have a higher initial figure, pricing then works for you: it's easy, natural and advantageous for the client if (say) you offer a tapered pricing that reduces the cost of seats above and beyond that first block, possibly attached to additional conditions (longer commitment period, for instance).


## Answer 36258

- posted by: [Nick Stevens](https://stackexchange.com/users/-1/15902-nick-stevens) on 2012-02-16
- score: 0

Talk to the client. LOTS. Understand their problem as it was your own problem. Work out how much this problem costs them. Charge less than that cost.

How much less? That depends on how badly you want their business.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
