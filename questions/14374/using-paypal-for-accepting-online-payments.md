## Using Paypal for accepting online payments

- posted by: [rem](https://stackexchange.com/users/-1/2715-rem) on 2010-09-24
- tagged: `payments`, `ecommerce`
- score: 8

Reading posts on this site I came accross the strong advice for any serious business to stay away from Paypal as an instrument for accepting online payments. On the other hand lots and lots of online businesses use it.

What are pros and cons of Paypal as a payment gateway provider?  


## Answer 14392

- posted by: [Aiden Bell](https://stackexchange.com/users/-1/4310-aiden-bell) on 2010-09-24
- score: 5

<p>In addition:</p>

<p>Pros = Easy of integration, PCI-compliance offloading, liability shifting, saner cashflow, no merchant account required</p>

<p>Cons = I have heard PayPal can (and do) lock accounts without warning, so regular 'emptying' is required. IMHO for high value items, it can look amateurish. However, PayPal can add integrity/security/peace-of-mind to smaller sites' customers.</p>

<p>I would also look into things like <a href="http://www.sagepay.com/" rel="nofollow">SagePay</a> and <a href="http://www.sagepay.com/products_services/sage_pay_go/integration" rel="nofollow">their products</a>, <a href="http://www.fastspring.com/" rel="nofollow">FastSpring</a> or a new contender like <a href="http://www.braintreepaymentsolutions.com" rel="nofollow">BrainTree</a>.</p>

<p>I have never heard good things from PayPal in terms of business users. They seem good at taking money off consumers but bad at giving it to businesses. I would look at the alternatives and try and find one with an SLA.</p>

<p>Depends <strong>very highly</strong> on the perceived quality, broadness or ambitions of your offerings. I would have no problem using PayPal for a niche e-commerce site selling something obscure, it is one of the few options they have. A larger (or trying to be) store with high quality web-design etch would raise an eyebrow about why they were using PayPal; </p>

<p>You can always <strong>change-as-you-grow</strong> if you build your setup in a modular way or use something like Magento that allows this. Good if you want to get cashflow going without the overheads of a highly integrated payment system.</p>

<p>If it were me, and I didn't have the option of a real MA then I wouldn't use PayPal, I have read far too many horror stories (but I am sure other payment service providers have them too). <a href="http://answers.onstartups.com/questions/12894/accept-credit-card-payment-within-your-site">This answers.onstartups.com question</a> seems to have a happy customer for Authorize.net</p>



## Answer 14385

- posted by: [Dr. Geoff](https://stackexchange.com/users/-1/4419-dr-geoff) on 2010-09-24
- score: 2

Pros = Brand familiarity and trust (Paypal explicit)

Con = High service fees. Also for anyone in the know a slight downgrading of your brand because of the amateurish nature of businesses that use Paypal over their own merchant processing system. 


## Answer 14402

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2010-09-25
- score: 2

I've used Paypal for over 6 years in my last startup and used authorize.net as a standard credit card processor.

First, you need to understand that Paypal has two functions. 

 - Consumers can use Paypal as a regular processor of credit card purchases similar to authorize.net and other processors. 
 - Consumers can buy using their paypal account without pulling out a credit card and typing their information. I'm like Karl, there are certain purchases that I'm too lazy to go and get my credit card and type in all the info, in that respect Paypal is a win.

Paypal can be a pain. 
 - If you have to talk to them, prepare to stay on hold for a while
 - Their policies are their policies. If you don't like them, tough.
 - I've had problems with people trying to use a credit card that's also used by the person as their paypal account payment method, and paypal declining.
 - Paypal itself has a limited number of countries it operates in. I think that if you use their credit card handling, that works fine.

Overall, I'd say that my experience with Paypal was similar to the one with Authorize.net. 

I never had money arbitrarily withheld by papal, and their dispute resolution was, as a rule, reasonable.

I've heard good things about FastSpring from several people, but have never used them personally.



## Answer 14393

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-24
- score: 1

Here are some of the issues we've heard from clients who switched to FastSpring from PayPal:
http://tinyurl.com/oxbs9r

No doubt there are plenty of happy PayPal customers as well, this is however from those who have had some issues.








## Answer 14395

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-24
- score: 1

Depending on the level of engagement of your users another consideration is what is easiest for the customer. 

For a small purchase that I am on the fence about, it's a real plus if they offer PayPal, since I am lazy and I know I dont have to type in any information beyond my password. If it's a credit card form or some payment processor I have never heard of I might move on.

Of course if the customer is already engaged and really wants whatever you are selling, or has invested time into configuration then they may not mind jumping over those extra hoops.


## Answer 14452

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2010-09-26
- score: 1

I used PayPal in the past, I've switched a few years ago and never looked back (to [FastSpring](http://www.fastspring.com) that I am extremely happy with), here are my personal experiences:

1. PayPal support is completely useless, they can't do anything you can't do yourself and they don't know anything you can't read on the site yourself.

2. They have policies, sometimes you will have problems with those policies, sometimes they will block you or delay money transfers, sometimes they demand you do something that take a week before you can complete a money transfer - and there's absolutely nothing you can do about it (and as I wrote in point 1 above talking to their support is completely useless) 

3. PayPal will not handle anything around the actual money transfer (for example collection VAT from EU buyers)

4. PayPal will not handle fulfillment (in my case sending license keys) - but there are 3rd party services that do that (I've heard good things about [eJunkie](http://www.e-junkie.com/))

I've also heard horror stories about PayPal freezing accounts without warning but that hasn't happened to me (fortunately).

On the other hand they have extremely low fees and are without a doubt the cheapest option for international money transfers



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
