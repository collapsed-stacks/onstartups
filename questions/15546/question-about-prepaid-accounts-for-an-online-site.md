## Question about prepaid accounts for an online site

- posted by: [kSeudo](https://stackexchange.com/users/-1/4989-kseudo) on 2010-10-25
- tagged: `legal`, `donations`
- score: 1

I am in the early stages of developing a site that tries to provide a direct way of rewarding photographers who provide good material. Its a small idea but I want to implement it and see how the users like it.

The approach I want to take is thus: 

- A person signs up to my site <br>
- They deposit money to their account (typically 10 $)<br>
- Upon seeing something they like on the site they can reward the original creator with a donation (eg 20 cents) <br>
- The original creator can then cash out, should they receive enough tips (eg they earn 10$ from 100 tips of 10 cent).<br>

I would be using a eMoney payment provider like Paypal to handle all the deposit/Withdraw transactions but I would handle the donations.

My question is what are the legal implications for a system like this? 

It has been suggested to me that I would have to be a financial institution to do this which is beyond my means and seems like overkill for such a small site. I guess the concern here is money laundering/illegal abuse but I think these concerns can be mitigated with good design.

Also, I am aware that Paypal can chargeback on any transaction. This would be really bad for me as I would have to ask for money back that has been donated or take the hit myself. I was going to implement a solution that required that any monies deposited must remain in the system for at least 45 days (the length of time for paypal requires) before it can be withdrawn. This adds inconvenience to my user base but would cover me from a malicious abuse of my system.

Can anyone offer me some wisdom here?
Thanks guys.


## Answer 15551

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-10-25
- score: 1

This sounds like something one would find in David Silver's book "Smart Startups". The idea is good but in reality it is not that easy to launch a brand new site, ask people to sign-up and then ask them to deposit money to give away to other users. 

Also, you're talking about photographers, which means they would have to upload decent quality images. Do you have a limit per user? Image size restrictions? Just do a basic math:

 - One image, say 800x600 in full color could be up to 100 kB;
 - Photographers take a lot of pictures. Say a user uploaded 20 shots;
 - Let's assume you've got 1000 of them;
 - Now multiply by 1000 visitors that just happen to wonder in;

100kB x 20 x 1000 x 1000

Multiply all this and you should be concerned with the bandwidth and storage capacity as well as the fees involved rather than the PayPal fees.

Sorry, don't mean to rain on your parade, just want to make sure you are aware of all the aspects on this venture.

Good luck.


## Answer 15563

- posted by: [xiaohouzi79](https://stackexchange.com/users/-1/4868-xiaohouzi79) on 2010-10-25
- score: 0

One suggestion is to have your users purchase something like credits rather than it representing $10.00, they could purchase 100 credits for $10.00.

Credits could be paid for by credit cards only so you don't need to worry about PayPal and people emptying their account without you knowing.

Another suggestion is to set a minimum withdraw level for photographers e.g. 1000 credits, the same as Google Adsense to reduce the number of transaction costs and to increase engagement (in this way they will likely keep working until they reach the 1000 credits if they already have some).

You should also search on this site for "alternatives to paypal". There are many good questions and answers that could help you lower your costs and some of the alternatives provide protection for the seller as well as the buyer.


## Answer 19322

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-01-24
- score: 0

If I have you right, you're expecting that the typical case is that withdrawals can only be triggered after lots of 'tips'.

At any point in time you have

1. Deposits, not yet allocated
2. Deposits, allocated to accounts below the withdrawal threshold
3. Deposits, allocated to accounts above the withdrawal threshold
3. Withdrawals

Your risk is that withdrawals exceed deposits, as you suffer chargebacks - and you pay out more than was put in.

You have two levels of structural protection here.

First, there's a buffer formed by the (1), (2) and some of (3). And secondly, the service you are selling is to pay a tip - that is, the digital goods have been delivered in the act of completion.

But you also have a potential problem. If you are not explicitly charging, but making the service viable out of the float you get from depositors, each chargeback is on assumption a loss.

You could address that a few ways.

*You could charge.* If you take a small percentage to cover this situation, in essence you are self-insuring. This seems a very natural solution to me.

*You could adapt the processes.* For instance, if you held all tips out of an initial deposit in reserve for 45 days, the photographers would sometimes see their balance broken down into an amount available (if it meets the threshold) plus an expected additional amount. And if your service is successful, you can tweak this process as you get to know the risks better.

*You could vitualize.* If money translates into a virtual currency, with a variable relationship to cash (a) you have a stronger case that the transaction took place at the time of deposit, (b) you have more latitude to build in a margin. For instance, if $10 buys me 50 credits, that I can use to give out smiles (1 credit), thumbs-up (3 credits), applause (10 credits) and whatever, and $25 gets 150 credits - as you'll see, as soon as there's the mildest complexity you have some room to manoeuvre within which you can cover the payment risk.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
