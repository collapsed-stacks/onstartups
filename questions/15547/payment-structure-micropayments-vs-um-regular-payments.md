## Payment structure (Micropayments vs um, regular payments)

- posted by: [Adam](https://stackexchange.com/users/-1/4272-adam) on 2010-10-25
- tagged: `payments`, `micro-payment`, `billing`
- score: 2

So this question has to do with customer perception on billing.

We're looking at the benefits of [micropayments][1] vs regular [payments][2].

Our business will have a series of charges from $1 to $5.  When initially setting up a session, there should be anywhere from 10 to 100 of these $1 charges along with a $5 charge.  I was thinking a shopping cart style combination of these charges to group them all, and then using the standard payment method.  

The problem comes with users adding additional charges as their session progresses.  Add something here, $1, add something there, $1.  Obviously, Micropayments are built for those kinds of charges, so it would make sense to use them.

As a consumer, would you rather get micro-charged (more, smaller charges), have a $10 minimum for a check out (and avoid micropayments), or have a fee added for carts < $10?

Thanks!

  [1]: https://www.paypalobjects.com/IntegrationCenter/ic_micropayments.html
  [2]: https://merchant.paypal.com/cgi-bin/marketingweb?cmd=_render-content&content_ID=merchant/wp_standard


## Answer 15552

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-10-25
- score: 3

It's not a question of whether or not your customer will like micropayments. The real question is, **can your business afford to use micropayments?**

Every transaction has an overhead cost associated with it. In general the lower the item cost, the higher the **percentage** lost to overhead. 

For example, if you sell software for $100 and have your own merchant account, a $100 sale might cost you $1.50 (1.5%). If you sell low priced items that cost $1.00 each, and sell 100 of them how much will you actually take in? Many micropayment processors charge 30% or even more! So after 100 $1.00 sales you net $70. Compare that to $98.50 for a single purchase with your own merchant account.

The most common way around this problem is to sell "credits" or something like that. You sell the customer a $10, or $25 "credit" and then subtract your micropayments from that base amount until it is all used up.



## Answer 15548

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2010-10-25
- score: 0

Micropayments don't work - try it open any news website or pick up a newspaper, now imagine you have to pay 10 cents per article, go over the titles and think "is this article worth paying for? is it's just filler content that's a waste of money or is it a good article I really need to read?".

This is very stressful and not a good user experience - and you are going to subject your customers to this when you set up your account? unless you are offering something that can't be replaced you will lose a lot of customers that way.

Try to group all those charges into logical groups of options that go together - selecting one $20 charge is better (less stressful, more pleasant) than 3 $5 changes and that in turn better that 10 $1 changes - note you can charge more while making it a better experience for the user!

Don't set a minimum price, that way you will make the people who didn't reach the minimum feel like you are reaping them off - you can set up things so that the cheapest package is $10 to avoid the technical side micropayments (just look around, why do you think the most common price for the cheapest plan for most SaaS apps in $9/month?)

And if all those changes are made at the same time combine them into one charge, it's so much easier to pay one time via credit cards or paypla that it's just stupid to force your customers to use micropayments)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
