## Paypal vs Online payment systems

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-19
- tagged: `website`, `payments`
- score: 2

I've been googling and googling, but can't seem to find a clear answer.  

I'm pondering on just using paypal payment system (which is really simple and fast) on my site or using on site payment (long, tedious, complicated, more pricey if small company).

Does anyone have concrete stats on the user preferences between the above?

Such as buyer preference when both options are available, personal testing, or I even welcome advice.

Thanks.


## Answer 23650

- posted by: [Carson McComas](https://stackexchange.com/users/-1/9422-carson-mccomas) on 2011-04-19
- score: 3

Completely depends on what, and to whom you are selling. Are you selling art to moms, or enterprise software to fortune 500 companies? PayPal would be the right choice for the former group, and a standard merchant processor for the latter. If it's not obvious where you fall on that continuum (and maybe even if it is), I'd start by asking your potential customers.


## Answer 23660

- posted by: [Ankur Jain](https://stackexchange.com/users/-1/6146-ankur-jain) on 2011-04-19
- score: 2

If you're just starting out I would suggest don't look beyond PayPal ( or may be FastSpring).
I have had good experience with both. FastSpring is very quick to set-up and may look more professional.

Integrating on-site payment is a pain and you have to take care of all sorts of security compliances.


## Answer 23661

- posted by: [Rain](https://stackexchange.com/users/-1/9208-rain) on 2011-04-19
- score: 2

Have you looked at the Merchant Pro version of PayPal? It is what I'm in the process of implementing because it really seems to be the best of both worlds.

You can whitelabel the purchase process so even though PayPal is an accepted payment form, it doesn't take the user to a PayPal branded payment page. This is a little bit more work to implement than normal PayPal, but the fact that I can make it look like we're the ones doing the payment processing makes it ideal for our purposes.

Setting up a merchant account is quite a hassle- I'd really recommend starting with PayPal and then migrating to something else based on customer feedback.


## Answer 23658

- posted by: [Tony](https://stackexchange.com/users/-1/9796-tony) on 2011-04-19
- score: 1

I would suggest looking at your customer base first. 

You could perhaps set up your site using PayPal as a payment method since it's the cheaper alternative. Then gather some kind of data/metrics from your logs to determine if users turn away when they hit your payment page. Though this might be because of other factors (price of product), you'll have a general idea. Based on this, you can get a better understanding of your customer base and then decide if going the payment gateway route will benefit you. You'll obviously have to factor in cost of the gateway and all that jazz.

You may even consider factoring in your customer base average age if you have this information... I don't have concrete evidence, but it would seem from past experience that the older generations would rather prefer the standard merchant processor over PayPal.

As for my preference, I would prefer to have PayPal as an option when I buy something. As far as testing goes for PayPal, it's pretty straight forward. They provide a "Sandbox" which allows you to test almost all the functionality that you would encounter if the code was on a production server.


## Answer 23665

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-19
- score: 0

I would say use paypal to start with and switch over to a more flexible and less expensive payment system when you have a steady stream of customers.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
