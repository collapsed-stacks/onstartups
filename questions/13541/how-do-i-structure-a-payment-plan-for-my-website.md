## How do I structure a payment plan for my website?

- posted by: [user2306](https://stackexchange.com/users/-1/2306-user2306) on 2010-08-19
- tagged: `payments`, `saas`, `website`, `business`
- score: 3

I plan on making my website a paid one and have a question about structuring the payment plan. Think of the website as an ecommerce site selling very low ticketed items (as low as $0.05). Since payment processors such as Paypal have a processing fee per transaction, I can't really make anything if I sell a single item for $0.05.

So, I plan on accepting a minimum of $10 (or multiples thereof) and now have 2 options:

 1. Implement a credit based system and
    sell x credits for $10. Users can
    choose to use 1 credit at a time if
    they wanted to.
 2. Keep it simple and simply reduce the users balance by $0.05 every
    time they buy a single item.

In either case, how do I handle refunds. In the first plan, do I expire unused credits after some time?

Any thoughts?


## Answer 13558

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-08-19
- score: 4

Calling them credits may make it easier for the user and on yourself when displaying balances and giving refunds. You also don't have to display balances or prices in different currencies. It's only a factor when purchasing credits or to cash someone out. 

Promotions like, buy 100 credits before the end of today and get 10 free. 

Expire the credits, but go out of your way to notify users. It could be a way to invite them back to the site.

Not sure what you sell for a nickle. Hopefully there are ways to encourage users to buy in bulk. 


## Answer 13554

- posted by: [Jeff Epstein](https://stackexchange.com/users/-1/3666-jeff-epstein) on 2010-08-19
- score: 1

You want to batch the payments into larger amounts or you will lose money on each "sale."

The credits are a good idea, I do not really see a difference between each option = in a sense, the credits are worth $.05 each and the balance is reduced accordingly.

You can handle refunds however you want.  If the item is $.05 I assume it is a digital item - are refunds necessary?

Expire credits however you want as well.  If you are not 'fair' your users will let you know.  


## Answer 13562

- posted by: [Zuly Gonzalez](https://stackexchange.com/users/-1/2692-zuly-gonzalez) on 2010-08-20
- score: 1

I like the idea of purchasing credits. Mentally it's easier to spend credits than it is to spend real dollars.

I don't like the idea of expiring credits. You're getting the money up front, so the customers have already paid for them. People may be reluctant to participate if they think there's a chance they may lose money. But Jeff did bring up a good point about it being a way to invite customers back to the site. 

Concerning the refund issue, I don't think most normal people would bother going through the trouble of getting back $.05...it's just not worth the time. Also, it will probably end up costing you more to return the $.05 to the customer. That said, I think it's probably a good idea to offer refunds to customers. It's a psychological thing that may result in a paying customer, even if the customer isn't actually going to go through the trouble of getting a refund. It's just nice to know that you can get a refund if you really wanted to. It shows goodwill, and removes a barrier.


## Answer 13555

- posted by: [BhargavPatel](https://stackexchange.com/users/-1/3998-bhargavpatel) on 2010-08-19
- score: 0

I forgot to read all of the post and I started typing but I just noticed that you had the same idea I had... of having minimum balance/deposit. Its a great idea so I 1+ you. 

1st option is much better. Credit system is better just because its cleaner and lets them know how much they can buy without worrying about anything else. Keep it flexible and have multiple plans. Multiple plans meaning, I can buy 5 credits or I can buy 50 credits. 

You can even get more complex, and give your users both options when they signup. But this will require you to do more work.

Try to implement a proper refund policy and warn your customers about the policy before they purchase. I don't agree with Jeff. Even though its 5 cents it matters. If some users can't get a refund, they'll think that was the catch, that you are getting to greedy or worst, you were a fake and are just ripping people off like this. **Put your customers before your revenue, if you have to, lose some money but your customers are your priority. In this social age, you can't afford to get a bad rep.**






## Answer 13631

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2010-08-24
- score: 0

 - Your own credit system will only work if customers anticipate making multiple micropayments to you. i.e. I have to believe that I will purchase $10 worth of stuff within a reasonably short period of time before either the credits expire or you go out of business. (Not saying you will, just looking at it from the customer's viewpoint).

 - Note that Paypal has a micropayments option - 5% + $0.05 per transaction. 

 - Another possibility is a shopping basket with a minimum order charge (say $1 or $5).  Depending upon what you are selling, this might work as an incentive to spend more. 

 - Credit expiry (which keeps accountants happy): >= 1 year is reasonable IMHO. Anything less will leave me worrying whether the credits will expire before I use them, and therefore I won't buy them.




## Answer 24985

- posted by: [Marcin](https://stackexchange.com/users/-1/8798-marcin) on 2011-05-16
- score: 0

If you denominate account credit in abstract credits, then (a) you can refund at a different rate from that which people buy, and (b) you can just have some kind of voucher for sale (such as itunes credit vouchers or whatever). 

(a) Should act as a disincentive for people to cash out too frequently. (b) Is another way of making a profit off their desire to take their cash away.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
