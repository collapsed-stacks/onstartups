## New startup - how to handle billing?

- posted by: [Wayne M](https://stackexchange.com/users/-1/1455-wayne-m) on 2009-11-19
- tagged: `saas`, `payments`
- score: 10

My subscription-based application is going to be written in Ruby on Rails; I have two routes I can go as far as billing is concerned:

1. I can use a hosted service that takes care of managing the subscriptions for me, such as [Spreedly](http://www.spreedly.com), [Recurly](http://www.recurly.com), or [Chargify](http://www.chargify.com).  My understanding is that these services will handle all of the customer signup details, handle the month-to-month billing and make sure the money goes into my account.

2. I can purchase the [SaaS RailsKit](http://www.railskits.com/saas) which seems to do the same thing except I'm responsible for setting it up myself; it provides the framework to talk to the payment gateway but nothing else.

Since this is my first ever startup and I'm fairly new to the idea, would I be better off "outsourcing" this capabilty to a company that knows what they're doing instead of trying to do it myself?  The downside of course is that there is a monthly fee involved with using a hosted service, and this reduces my profit, but the additional features they provide may be worth the cost.

Any suggestions?


## Answer 3854

- posted by: [Brian Swanson](https://stackexchange.com/users/-1/1150-brian-swanson) on 2009-11-19
- score: 8

It's always best to stay focused as close to your core business as possible, especially when you're first starting up.  If the costs associated with outsourcing your subscription/payment processing is not too costly, it would likely be your best bet.  

You'll have enough challenges and headaches when launching your business, that the last thing you'll want to be dealing with is some bug/error in your custom subscription/payment processing code...

Later when the business is doing well, you can decide to build your own system, and bring it in house to help improve your profits.




## Answer 3877

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2009-11-20
- score: 6

<p>In general, I'm all in favor of letting other providers handle things that are not core to my business, as Brian and James are saying.</p>

<p><strong>This one does IMHO deserve more attention though.</strong> Customers are core to my business, and customer credit card info is a legally sensitive topic.</p>

<p>Here is a <a href="http://blogs.zdnet.com/SAAS/?p=484">good overview of some larger providers</a> in this space.</p>

<p><strong>Benefits of outsourced subscription management:</strong></p>

<ul>
<li>Short time to market; low capital burn for initial development of your own product.</li>
<li>Heavy <a href="http://en.wikipedia.org/wiki/Payment%5FCard%5FIndustry%5FData%5FSecurity%5FStandard">PCI compliance requirements</a> are handled by someone else (as you don't store credit card info yourself) (and if it's not handled properly, you have a socially acceptable scapegoat in the SaaS subscription provider).</li>
</ul>

<p><strong>Downsides of outsourced subscription management:</strong></p>

<ul>
<li>Integrating subscriptions with your own accounting &amp; invoicing infrastructure is a bit harder when it's off-site.</li>
<li>If you <strong>ever, for any reason, need to switch subscription management provider</strong>, you face some <strong>nasty issues</strong>. They have the credit card info of <em>all</em> your customers, so this means <em>inconveniencing all your customers</em> to re-enter their card info. And arguably, some of your customers will not do this, and will thereby stop being your customers.</li>
</ul>

<p><strong>A decision should be based on:</strong></p>

<ul>
<li>How short on cash are you in the initial development fase; how valuable is short time to market for you.</li>
<li>How well are you set up to handle PCI compliance and secure hosting in general.</li>
<li>Do you see a future need to be very flexible with regards to subscriptions, to have many subscription models and additional charges, or not.</li>
<li>The size of the current and future cash flow; i.e. how big will the subscription providers future cut be.</li>
<li>Most important, the subscription providers staying power, and future business practices (of course very hard to estimate).</li>
</ul>



## Answer 3855

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-11-19
- score: 3

I agree with Brian Swanson that you should look at staying close to your core.

Generally, you should outsource or buy whatever isn't going to be part of the core app, then, as you get excess money and want to stop supporting others, then you can look at writing your own applications and take over the control.

But, if you are going to do that you want to make certain you have a good separation between your app and the solution you start with, so you may want a module that serves as the interface, so that later if you decide to change, you change in one place and your application switches happily.

If you don't design up-front for this, then it will be too expensive to replace these other solutions with your own.


## Answer 3930

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-21
- score: 3

**Consider not having an automated billing system** at first.  Collect the cards yourself and bill yourself.

Sounds retarded?  It's not:

 1. Takes very little time until you have a lot of customers, at which time you can afford to implement a real system.
 1. Gives you a chance to talk to customers directly, which is invaluable.
 1. Gives you a chance to make any billing/pricing changes you want.
 1. At the mid-point between wanting an automated system and manual efforts mounting, an inexpensive admin service can do the bookkeeping for you.
 1. "Automated billing" isn't as automated as you think.  There's always problems you have to resolve manually.


## Answer 3956

- posted by: [Bob Walsh](https://stackexchange.com/users/-1/346-bob-walsh) on 2009-11-21
- score: 3

Subscription billing is a major headache for startups. It's easy to get it wrong (as I did initially). Billing is what Geoffery Moore would call "context" it's not the core of your business. I would definitely use a vendor: I've switched over StartupToDo (a Rails app BTW) to Amazon Simple Pay Subscriptions. Works great worldwide, but you have to be in the U.S. Second alternative is Avangate (does PayPal which Amazon [now a direct competitor to PayPal] does not, you can reside practically anywhere) which I will be implementing soon to support those customers who want PayPal.


## Answer 3940

- posted by: [Benjamin Curtis](https://stackexchange.com/users/-1/1615-benjamin-curtis) on 2009-11-21
- score: 0

<p>Since I'm the creator of the SaaS Rails Kit, I'll chime in. :)  Many people have found the Kit useful to get them launched faster, so it sounds like you are in the sweet spot for what the Kit can do.  </p>

<p>Jason's right, you can certainly get by with a manual process in the beginning, and switch later when you are making real money, or when it starts becoming too tedious.  However, based on my own experience with handling the billing for <a href="http://catchthebest.com/" rel="nofollow">Catch the Best</a> (which was the genesis for the SaaS Rails Kit), it can be a hassle to make that switch later.</p>

<p>If you're looking for plug in and go, both the services you mentioned and the Kit fit the bill: handling account creations/upgrades/cancellations, running the billing every month, etc.  The Kit also has a convenient way to implement tiering (project limits, user limits, etc) for your various price plans inside your app.</p>

<p>Either way, I'd definitely recommend not building it yourself -- life's too short for that drudgery. :)</p>



## Answer 4570

- posted by: [Paul O'Brien](https://stackexchange.com/users/-1/759-paul-o-brien) on 2009-12-03
- score: 0

<p>Frankly, all the answers are right.  Bottom line? Depends on how big a business you are or intend to become</p>

<p>Do you have the resources, or intend yourself, to manage billing, payment processing, customer service, etc.?  Can you benefit from a personal touch with customers via their payment process?</p>

<p>Outsourcing does take most off your plate and sure, it also comes with some cons nor does it handle everything.  But, it comes with other benefits not readily considered such as direct integration with a CRM service, your bookkeeping (<a href="http://outright.com" rel="nofollow">us?</a>), email platform, etc.</p>



## Answer 18679

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-07
- score: 0

Check out www.metanga.com, the application can handle all forms of subscription billing management, work with any payment gateway, and automate your bill close process. They are  a pretty new division of MetraTech.com which is a global leader in the billing space.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
