## SaaS, should we pick the payment options or let the customer?

- posted by: [Delboud](https://stackexchange.com/users/-1/19533-delboud) on 2012-09-03
- tagged: `marketing`, `payments`, `saas`, `payment-gateway`
- score: 3

Working on a new B2C SaaS will allow our customers to accept payments online from their customers. 

Currently we're trying to decided whether its better to have a list of payment gateways for our customers to use or is it better for use to go with the best choice from our research.

If its a list of gateways, our site is more modular, but not sure if its needed. In addition gateways(including merchant accounts) can get confusing without research. The list is currently stripe, authorize.net, braintree, paypal and a few others.

On the other had we can do research, choose the best quality option with fair pricing and call it a day but, in that case we may seem that we have customization fit for different people needs and wants.

Majority of or audience have no current system like the one we are making so the knowledge of these gateways are pretty limited. I assume that if they did research they will go for the cheapest.

Which seems like the better path to take?


## Answer 41804

- posted by: [Grzegorz](https://stackexchange.com/users/-1/19509-grzegorz) on 2012-09-04
- score: 1

I suggest to start with one gateway (best in your opinion), and then optionally add suggested gateways by your customers. In this approach in first step you could reduce effort to integrate (development, testing, support) only with one option.


## Answer 41821

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-09-05
- score: 0

There are tons of gateways. To hard to support them all unless you use something like http://www.nsoftware.com/  products which allow you to integrate with their API/DLL and they take care of the actual specifics for the processor.

However, I would implement PayPal and Authorize .Net because they are the most popular & Stripe because they are huge up and comer and $0/mo which gives your user no excuse not to use them. (Except if they are not in the US)





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
