## How does our online startup sell retail and wholesale - separate carts or password protected page for wholesale prices?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- tagged: `website`
- score: 0

We want to sell at retail and wholesale prices on our website. How do you recommend we build the shopping cart so that wholesalers use one cart and retail shoppers use another one?


## Answer 16103

- posted by: [Janis Peisenieks](https://stackexchange.com/users/-1/5241-janis-peisenieks) on 2010-11-05
- score: 1

This will most definitely mean altering your code, but I would go for it.

 1. When entering products, use 2 prices, or some sort of scheme to derive retail prices from wholesale. This will clutter your database a bit more, but will simplify the coding.
 
 2. When registering, have the customer chose the type of account. It usually involves some distinct fields for wholesale, so they should definitely be separated. 
 3. Depending on the type of user logged in, display the appropriate prices and shopping cart. 

I do think, that the cart should stay the same, only the product prices (and the minimum quantity) should change. In my opinion, there is no particular need to create a completely separate cart for this website. 

P.S. I would also follow the advice of Isaac, and do some manual approving. Most wholesalers I've worked with do not allow users to register themselves.


## Answer 17411

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2010-12-05
- score: 1

First, ask yourself whether your wholesale and retail customers need the same experience. If the answer is 'yes,' then one system, two customer types, with verification/approval for wholesale accounts is the way to go. Clearly the default is the retail experience and retail prices.

There are lots of situations where the needs of the two groups are different. For instance,

* If you have an extensive product range
* If you want different behaviours regarding in stock/out of stock etc for the two groups
* If you are marketing products that are designed to be easy alternatives to specific competitor products
* If your retail offering is going to be significantly offer-led
* If you are expecting significant volume orders from wholesale customers

In these cases, I'd always recommend a single product database feeding separate sites. Each needs a shopping cart that's built to work with a separate stock database, but then you have the flexibility to optimise in each domain.


## Answer 15668

- posted by: [Siddhartha Oza](https://stackexchange.com/users/-1/4370-siddhartha-oza) on 2010-10-27
- score: 0

1. provide a separate page for wholesale prices and a separate one for retail.
2. another idea can be to provide coupon codes, which users can apply to get prices in wholesale, before checkout.



## Answer 15671

- posted by: [Isaac Martinez](https://stackexchange.com/users/-1/5077-isaac-martinez) on 2010-10-27
- score: 0

If you are willing to customize the code of the cart you can have users register for wholesale accounts.  These accounts will be manually approved.  Once someone has a wholesale account then you could code the system to recognize the user type and display price accordingly.  On the backend you would need to setup multiple price points to work with the aforementioned functionality.




## Answer 17416

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-12-05
- score: 0

It's true that you *may* want to create separate sites entirely for your retail and wholesale clients.  If you need to give them generally different shopping experiences, this is surely the way to go.  **However**, if you do want it all in one site, you don't necessarily have to dive in to tons of custom code.

Check out [Drupal](http://drupal.org) with [Ubercart](http://dgo.to/ubercart).  A combination of supporting modules will allow you to do most/all of what you need without any/much custom  code.  For example, a while ago I built a site for a distributor that offered the same products to many clients, but different pricing for each.  He could assign a role to each account, giving it access to products with the right prices for that account type.  :)


## Answer 17521

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-08
- score: 0

You only need one cart.  you need a database table for pricing levels.  So you can have 2 levels, retail and wholesale.  For each product you put in the retail and wholesale price in your db.

When your user accesses the site they see retail prices.  If they are logged in and have wholesale access then they get wholesale pricing.

You want to code as little as possible, Having pricing levels give you access to do so. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
