## How to display complex pricing in a friendly way

- posted by: [Alex C](https://stackexchange.com/users/-1/9310-alex-c) on 2012-12-08
- tagged: `pricing`, `saas`
- score: 2

I'm launching an online service which is designed to bring together a lot of different services into one package, all manageable online.

The problem I've got is how to handle the pricing. The price structure is as follows:

- Service A is a service which runs for a month, it is priced at one of 4 price points depending on how many resources are required. In addition, there are two optional extras which can be added on for a fixed monthly fee.

- Service B & C are services with a fixed monthly fee, and then a 'per unit' cost.

- Service D just has a fixed monthly cost

- Service E (which is storage which underlies all the other services) is priced per GB.

Any monthly fees (including add-ons) are invoiced monthly in advance, and usage is deducted from a pre-paid deposit balance.

Are there any 'best practices' for this kind of thing? Would I just be better putting together packages which include all the services (at varying levels)?

The closest example I can think of would be cable services - e.g offering television, phone and broadband with varying levels of packages and some parts of the service billed in arrears based on actual usage.


## Answer 44869

- posted by: [Jeremy](https://stackexchange.com/users/-1/21978-jeremy) on 2012-12-08
- score: 5

If your business model is to bring all of these services together into one package, then you're going to have to come up with a unified pricing plan.

I'm not sure that this happens so often that there's a "best practice" here, but in general you should stay away from complicated pricing.

I don't recall seeing any successful B2B start up with a pricing plan based on more than one attribute. I've seen tiered pricing, consumption pricing, etc.

On a more general note, however, nobody's going to use your service if they can't reasonably predict how much they're going to have to pay, and as a potential customer, your pricing strategy above is way over the line.


## Answer 44877

- posted by: [danie7L T](https://stackexchange.com/users/-1/19409-danie7l-t) on 2012-12-08
- score: 0

A "dynamic pricing table" on top of the regular one could improve the overall understanding of the packages.

An HTML/JavaScript form with multiple choice questions corresponding to the services and sub-services you offer with "real-time" price adjusting seems to me the better way to guide the client. 
That way he can "play" with the system and get a better picture of the price/services balance. 


## Answer 44878

- posted by: [BrianAdkins](https://stackexchange.com/users/-1/21412-brianadkins) on 2012-12-08
- score: 0

I've dealt with many b2b companies with non-simple pricing schemes... Usually email service providers that can have both flat monthly tiers and per-email tiers. Then they then offer other options such as archiving (per GB), static IP addresses (per server), etc. 

I think the key is to make things as simple as possible for 80% of your customer base while allowing more complex customers some flexibility.   This could come in the form of pre-packing the most popular combinations of your services. 

Example: 
WPEngine's pricing certainly 'seems' simple enough, but if you look deeper, there are lots of options.  Some options are even hidden such as the fact that they'll tack one 1 more installation to a plan for $15/mo (I think). 

http://wpengine.com/pricing

For 'complex' customers, a dead-easy cost calculator could help.   Make it obvious with messaging such as "don't see exactly what you need, build your own custom plan here"





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
