## Credit card processing for startup

- posted by: [ReadyToCompete](https://stackexchange.com/users/-1/21156-readytocompete) on 2012-10-15
- tagged: `credit-cards`
- score: 6

What are the options available for online credit card processing?  I have developed a website where I need to charge credit card.  I will not be interested in storing credit card information.  I know there are online credit card processor out there like paypal, google, wepay.  I have those options and they typically charge somewhere 3-4% credit card processing fees.  

Our direct competitor charges 3% credit card processing fees when their user buys events tickets.  If I use paypal/google/wepay, it cost me around 3.5% for credit card processing fees(and if I add my commission on top of that it goes above 3.5%).

Is there any options out there that charges less than 3% credit card processing fees or I would have to come up with my own credit card processing (using merchant and gateway account)?

Updated: 
I was wondering how competitor can do credit card processing in 3% fees?  I am sure they are making some profit on that as well so their actual cost is lower than 3%.


## Answer 43646

- posted by: [CDD](https://stackexchange.com/users/-1/20086-cdd) on 2012-10-15
- score: 2

Th only other reference I have is Square, which charges a flat 2.0 or 2.5%. Then again, that is in-person transactions. As "LittleADav" already stated, online transactions are considered a lot more risky (or at least card companies say they are, so they can charge a premium), which results in that higher percentage fee. 

It would be nice to push your customers to alternative methods, but the truth is Paypal is still seen as a shady service to some, and checks/money orders are even less welcome among certain customers. 

My advice: try to beat your competitor on something other than a half percentage difference in end cost. As the previous commenter said, try to strike a deal by bouncing proposals between card providers (Intuit, PayPal, Google, WePay, etc). You should be able to get the cost down a little bit, probably closer to 3%. 

In the end, getting your own merchant account is going to be the best way to go, especially if you get large enough, or really require the margin to stay competitive!


## Answer 43644

- posted by: [littleadv](https://stackexchange.com/users/-1/13808-littleadv) on 2012-10-15
- score: 0

Even with your own credit card processing I doubt you can reduce that significantly. Internet purchases are high risk, that's why the processors charge high commissions. Shop around, bargain with the sales people for the processors, and you may be able to reduce it a bit. You can also try to encourage your customers to use alternative methods (paypal, check/money order, etc).


## Answer 43715

- posted by: [dreeves](https://stackexchange.com/users/-1/5701-dreeves) on 2012-10-18
- score: 0

I can't say enough good things about [Stripe](http://stripe.com ).
Here are some glowing things we said about it publicly before: [weusethat.com/beeminder](http://weusethat.com/beeminder ). That also links to a long love letter to Stripe from [Patrick McKenzie](http://www.kalzumeus.com/ ), who you should definitely listen to.

Note that as of 2012, Stripe is only in the US and Canada (though you can accept payments from anyone anywhere). They are working hard on expanding.


## Answer 43733

- posted by: [Dustin Kendall](https://stackexchange.com/users/-1/12316-dustin-kendall) on 2012-10-19
- score: 0

<p>Take a look at <a href="https://www.braintreepayments.com/" rel="nofollow" title="Braintree">Braintree</a>.  We're currently evaluating them and really liking what we see.</p>



## Answer 43737

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2012-10-19
- score: 0

When it comes to credit card processing fees, there are so many variables there. I have paid anywhere between 1% all the way to 4%. American Express and Discover Card charge the highest fees and even if you are processing $2MM per month, they will not negotiate. There are tricks to get some gift cards etc. from them, but you can't do it without having processed $100K+ through them.

Even within Visa and Mastercard there are, I believe, 6 tiers. Cheapest cards to process are non-reward cards and the most expensive ones are the corporate cards, which are considered highest charge-back risk. We are talking about 1% difference between the cheapest and the most expensive to process.

And because credit cards will be keyed in and not present, that increases your discount rate too.

Until you process $100K or $200K without chargebacks, you will not have as much bargaining power. You will need to start somewhere to get the track record.

Also, very important you have the right D&B record and industry classification. Your rate difference can be huge, if you get the wrong code for your business, since risk premium is all based on risk of charge-back.

Bottom line: find the right broker (if you can't, go to my profile and get in touch with me, I will give you contact for my guy) and they will navigate you through it. 

P.S. I usually choose Authorize.net for the virtual terminal, because I can API into it and many systems tie into it very nicely.






---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
