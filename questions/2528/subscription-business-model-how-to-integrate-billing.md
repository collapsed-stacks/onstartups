## subscription business model, how to integrate billing?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-27
- tagged: `payments`
- score: 3

with subscription based models, where clients are billed on a monthly basis, how do i make this happen on my site ?

so a client signs up, and is taken to paypal or google checkout , and they are now billed monthly ?


what if you have different subscription models ?

like professional, corporate, enterprise. 

pro would cost like 100 per month
corp would cost like 300 per month
enterprise would cost like 1000 per month.


how to deal with clients changing back and forth from each subscription model.


## Answer 2531

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-27
- score: 2

<p>You will store the billing information in google checkout or paypal, for example, and just set it up for recurring billing.</p>

<p>You don't want to store the billing info, as there is a great deal of security you need to ensure it is done properly, but for google this is in beta, as they explain on their site:
<a href="http://checkout.google.com/support/sell/bin/answer.py?hl=en&amp;answer=63440" rel="nofollow">http://checkout.google.com/support/sell/bin/answer.py?hl=en&amp;answer=63440</a></p>



## Answer 2538

- posted by: [Ade Olonoh](https://stackexchange.com/users/-1/317-ade-olonoh) on 2009-10-27
- score: 2

<p>First read through <a href="http://answers.onstartups.com/questions/1819/when-to-use-merchant-account-instead-of-paypal" rel="nofollow">this thread</a> for discussion about using PayPal or Google Checkout.</p>

<p>If you decide to go with a merchant account, take a look at <a href="https://cheddargetter.com/" rel="nofollow">CheddarGetter</a> and <a href="http://chargify.com/" rel="nofollow">Chargify</a>.  Each service manages the billing process and customer subscription details -- should be much easier than trying to roll your own.</p>



## Answer 2550

- posted by: [anthon](https://stackexchange.com/users/-1/238-anthon) on 2009-10-27
- score: 0

2 others to look at:

www.ariasystems.com

www.zuora.com

Both have fairly robust subscription processing offerings.



## Answer 2591

- posted by: [Paul O'Brien](https://stackexchange.com/users/-1/759-paul-o-brien) on 2009-10-27
- score: 0

<p>For a recurring revenue model, check out <a href="http://chargify.com" rel="nofollow">chargify</a>
Yes, PayPal and Checkout are the big guns that simplify your own merchant account but Chargify was designed for subscription billing and is really simple to use</p>



## Answer 18678

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-07
- score: 0

One of the best priced SaaS billing options is www.Metanga.com. They can support small businesses but also can scale to enterprise billing situations.


## Answer 29258

- posted by: [lrussell](https://stackexchange.com/users/-1/12709-lrussell) on 2011-08-25
- score: 0

<p><a href="http://recurly.com/" rel="nofollow">Recurly</a> is another service similar to those suggested.</p>



## Answer 29263

- posted by: [user2306](https://stackexchange.com/users/-1/2306-user2306) on 2011-08-25
- score: 0

For simple websites, I'd recommend Paypal subscriptions.


## Answer 29264

- posted by: [Nicko](https://stackexchange.com/users/-1/7870-nicko) on 2011-08-25
- score: 0

I currently use Chargify, and it's good.  I'm interested in Braintree as well.  Accel Partners just invested in Braintree, but Chargify was able to secure a large investment by Mark Cuban.  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
