## What is the best pricing model for a service based on requests?

- posted by: [yojimbo](https://stackexchange.com/users/-1/11366-yojimbo) on 2012-03-28
- tagged: `pricing`, `payments`, `saas`, `uk`
- score: 1

I have a product for monitoring specific areas of content within webpages and notifying the customer when changes occur to this content and what they are. (E.g. monitor the latest stories on a news website page, but ignore all other content on the page.) The product is run an online service.

At the moment I have one customer (although they are intending to use it on 10Ks of links) so the pricing mechanism is at an early stage. I would like to figure out the best way to do it before we go about automating the billing and payment aspects.

Currently we charge per request to check the content, and we charge more for requests that need to be checked within shorter time windows. Since Users may be performing 1000s of requests daily, according to different schedules, and also manually requested through the interface, this can lead to quite complicated billing calculations.

First, should I translate the pricing into credits, where for example a slow request costs 1 credit and a fast request costs 2 credits?

Is this going to make is a bit easier to understand for the user?
Would it potentially make them spend more money?   

Second, would I better to institute a tiered subscription system or a pay as you go system?

There needs to be some form of bulk discounting so either;

£X for 0-1000 credits per month
£Y for 1001-10000 credits per month
£Z for 10001-100000 credits per month

if you go over the limit for your level you have to upgrade

OR

£X per credit and you have to keep topping up the credits, but you get a discount if you buy more than N credits at a time.

The issues I am trying to consider are:

 - making it clear and simple for the users

 - encouraging users to use the service as much as possible

 - making any payment system easy to implement (I think it will be easier to get customers to pre-pay than bill them variable amounts monthly. This will also be better for cashflow)

 - allow easy reporting of charges and minimise queries about this

As I am based in the UK, I also need to deal with VAT correctly and in a way that is not confusing to users from different countries.


## Answer 37668

- posted by: [Karlson](https://stackexchange.com/users/-1/15252-karlson) on 2012-03-28
- score: 2

I think you're on the right track but you should not make it "credits" but do a simple model like:

**Prepayment:**

 - £10 per 1000 requests per month
 - £45 per 5000 requests per month
 - £90 per 10000 requests per month

**Overages:**  After going through the prepaid amount you pay:

 - £0.015/request

And if you are really nice you can then calculate and bundle based on the prepayment strategy.  The simpler the payment model the easier it is for your customers and you to understand and say yay or nay to.  And you can fairly easy calculate your potential revenue stream.




## Answer 37996

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2012-04-09
- score: 1

Your first question shouldn't be about detailed pricing structures but about what's driving value for your users. For instance, I'm not sure whether your point about distinguishing fast and slow requests points to value for your customer or/and cost to you.

In general, the pricing structure should align closely to how you create value for customers, and pricing levels in the early stages should mainly be driven by the kind of customers you want to take on and your capacity to service them.

It's always a tension for a startup - when do you try and get the pricing right? It sounds to me as though you have a proposition that's going to appeal to a very specific niche, and that should mean it's possible to do 'right-pricing' early - which is probably when you sign your second customer!

There's a strong school of thought that pricing is just like any other optimization exercise - something to do continually, by testing. In my experience, that's a valid approach for broad appeal, easy sign-up, low initial value services, but I doubt that matches where you are now. 


## Answer 37676

- posted by: [Nick Stevens](https://stackexchange.com/users/-1/15902-nick-stevens) on 2012-03-28
- score: 0

I'd suggest taking a look at any successful companies that provide api based services and comparing their pricing models. Whatever you do, Make it simple and transparent.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
