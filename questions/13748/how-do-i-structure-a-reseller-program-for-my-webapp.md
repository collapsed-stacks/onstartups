## How do I structure a reseller program for my webapp?

- posted by: [user3348](https://stackexchange.com/users/-1/3348-user3348) on 2010-08-28
- tagged: `resellers`, `affiliate`
- score: 3

I have been recently approached by someone, who wants to be a reseller for my webapp, blogVault.
One of the things he mentioned was that, he wanted to co-brand it, so that he can mark up and charge his clients. Now I had typically imagined it to be a situation where I had a relationship with the customer directly. What are the ways in which I can approach this situation? Is there a limit I should set on the markup this person can add?

One other concern I have here is that, there will be certain people, who will actually be paying more for the service, just because they did not directly visit my site. Can this be a problem?

Here is a link to my pricing page, to help answer the second question as mine is not a very expensive application.
[http://blogvault.net/home/pricing][1]


  [1]: http://blogvault.net/home/pricing


## Answer 13754

- posted by: [Jeff Epstein](https://stackexchange.com/users/-1/3666-jeff-epstein) on 2010-08-28
- score: 4

Consider creating a revenue share reseller program.  Allow the reseller to make a commission of your choice.  

This is simply a revenue share, which has several benefits:

 - All your customers are paying the *same* price
 - You maintain control over your product and pricing
 - You remain the primary point of contact 

If the reseller can prove they can resell your product at a *much higher* price, you probably need to revisit your pricing strategy.

Good luck!


## Answer 13752

- posted by: [BhargavPatel](https://stackexchange.com/users/-1/3998-bhargavpatel) on 2010-08-28
- score: 0

Alright, first of all resellers are a really good choice. They take the hard work away from you. They are kind of like sales persons. They go out, talk about your product, and get you customers. Think of them as living, breathing marketing campaigns. 

Since your app wasn't built for having resellers, it is not a good idea to let people do this. BUT, given that he can get you more customers, you can give him access to your database and all that and let him mark up for you.

This, by no means is safe. You can't even have any legal way to make sure he doesn't go berserk and mess up all your databases. *Thats the problem*. There isn't a solution but there is a workaround!

You tell him, alright I let you resell the application. I am not giving you rights to access our database, nor am I giving you a way to do so. You simply get customers, you can charge them however you like, but you have to give us the original price of the product. The rest you charge is yours. Once you get the customer, you let us know and send us a payment and we'll tailor everything to your needs.


That was a workaround 1, I just thought of another one while I was typing that. You can make another database (heck, even on a different server) give him access to that and let him add/subtract users like that. You can pull that data from the other server if you wish, but this workaround can get hairy if you get more resellers (which I think you should get).

I suggest you use Workaround 1 or make a solution (add a resellers feature). Also, another thing that you might have to watch out for if you automated all this (with workaround 2 and a solution), you might be getting ripped off. They can make as many accounts they want for themselves. And in long term, you will loose money from them. This is why Workaround 1 is best because he/she has to pay upfront. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
