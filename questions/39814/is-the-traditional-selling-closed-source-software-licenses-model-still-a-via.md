## Is the traditional 'selling (closed source) software licenses' model still a viable business model?

- posted by: [Mark](https://stackexchange.com/users/-1/18336-mark) on 2012-06-10
- tagged: `business-model`, `open-source`, `software-licensing`
- score: 0

I have developed a library that I would like to license to customers in the traditional way: users are paying for a license for a closed source library which allows them to use the library for a certain period.

With the recent trend towards open source software I have my doubts if customers would still be willing to pay for a license for closed source software. (Actually, I would prefer not to use closed source software myself because I usually consider open source software of better quality and it avoids vendor lock in.)   

When I would release my library as open source, there are ways to generate revenue from the software like support and consulting but I am not sure if this would be a viable business model in the long run. Someone else could just take the code base and start offering support for it and most users would just use the code without ever paying for support or consulting.

The question I have in specific is if someone ever had to take decision to sell closed source licenses or choose some another business model for a start-up and how that decision turned out for them.

In addition, I wonder if the traditional 'paying for a software license' business model is not disappearing altogether because of the trend towards open source, saas, and advertising based business models on one hand and piracy on the other hand.




## Answer 39818

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2012-06-10
- score: 4

> With the recent trend towards open source software I have my doubts if customers would 
> still be willing to pay for a license for closed source software.

Whow, I was not aware that all the companies selling licenses are now bankrupt. How comes?

MANY companies make a LOT of money with closed source software.

> Actually, I would prefer not to use closed source software myself because I usually 
> consider open source software of better quality and it avoids vendor lock in

Both hogwash arguments, sorry.

First, nothing in open source says it is good quality PER SE. Many are, but then many commercial software offerings are good quality also. Yes, open source gives you the code, but so does some closed source (you can get the code as part of the license, I have that here for some libraries) and vendor lock in you also have with open source because IF it gets abandoned, then sorry, I am NOT going to maintain that on top of my work, I replace it.

> Someone else could just take the code base and start offering support for it and most 
> users would just use the code without ever paying for support or

Are you that bad or so crappy in your requirements? Normally, if you are the developer, you are the person knowing your code base best. There IS an advantage, some projects make good money with that. You can also dual license - viral GPL for free, paid commercial license which does not require the user to share HIS code with the world if he sells it. That is something many open source projects do, too.

> In addition, I wonder if the traditional 'paying for a software license' business model 
> consulting. is not disappearing altogether because of the trend towards open
> source, saas, and advertising based business models on one hand and
> piracy on the other hand.

Ah, sorry - you can not sell a pirated copy here. If you build a product and use a pirated copy, that is nasty - this is not copying for your own use, you are betraying your customer. So, that is out.

Otherwise, sorry, I am not aware of Microsoft, Oracle etc just giving their revenue away right now. There is a free model for people that are not valuing their time or have limited needs, and there is often a quite expensive commercial offering for users with high needs. In the last project we paid hundreds of thousands of dollars for licenses and it was irrelevant - we burned about 800,000 for people every month, for way more than a year, some hundred thousand did not even show up.

The model is NOT going away, it is valid. Whether it is valid for you depends a LOT on what you are talking about. I personally have quite a lot of commercial stuff simply becase it is better than possible open source alternatives I could get my hands on and I am willing to pay money to make money. I live in the .NET world, but my commercials (outside MS) are things like Infragistics (UI control framework, with source provided), MemProfile and other tools.

BUT: You know little about the world works, I think:

> users are paying for a license for a closed source library which allows them to use the 
> library for a certain period.

This is not "the traditional way", there is not a single purchase offer I am aware of that works like that.

ALL licenses are perpetual. You are allowed to use as long as you want, for libraries often with redistribution rights (90% of the cases). What you are NOT getting forever are UPDATES, but if you get a version, and CAN technically use it in 10 years, you are free to do so. Not a single library I know of has limited time usage rights.

Your main problem is that while closed source gets you better cash (which is good), you still must know how the world works (doubts here) and - well - get sales channels set up. That is a LOT of work. A LOT. It depends a lot on WHAT you are talking about, and you do not say, except it is "a library".


## Answer 39817

- posted by: [noway](https://stackexchange.com/users/-1/18054-noway) on 2012-06-10
- score: 3

The traditional model is still viable, and if you look at the top earning software vendors they are all doing this, Microsoft, Oracle, IBM etc.

However, your decision should be based on your market, your software and abilities of your company.

For example, if you are developing a CRM solution, where many products and vendors are competing, you should go for open source.

On the other hand, if you are developing an enterprise level application, have good sales channels etc. closed source may be a better profitable option.


## Answer 39878

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2012-06-12
- score: 1

<p>I have many years direct experience of both open and closed sourced software in the company I founded. Let's be very clear, <strong>open</strong> source is not a viable business model in the majority of cases. This generation seems to somehow think open source has overrun closed, except in a few, generally very mainstream projects, it's made virtually no inroads at all.</p>

<p>The next argument is dual GPL/commercial license. No, that doesn't work either, the majority of developers simply don't understand basic licensing, and yes, I've interviewed developers extensively on the subject.</p>

<p>Your question is somewhat confused. You've developed a library (and that's what we produce) but then you mention SaaS. Libraries aren't delivered by SaaS, they are always given directly to the developers.</p>

<p>I can give you one constructive piece of advice, and this is based on 6 years experience analysing the market for our library. I mentioned developers don't generally understand licensing, but they do understand "free for non-commercial use". So we recently took our closed source library (which sells very well) and put it on <a href="https://github.com/jgraph/mxgraph" rel="nofollow">github</a> under a <a href="http://creativecommons.org/licenses/by-nc-sa/3.0/" rel="nofollow">non-commercial use license</a>.</p>

<p>This has not impacted revenues at all, companies that wish to comply always will. Those that don't would never have any intention of buying. Free for non-commercial use is not technical "open source", however, the source is publicly there.</p>

<p>As for why you think open source avoids "avoids vendor lock in", I simply don't understand why you would think this. The cost of integrating a library far exceeds the cost of licensing them, you are "locked" into whatever you use regardless of cost or source availability.</p>



## Answer 39881

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2012-06-12
- score: 1

The open source and closed source markets work in very different ways.

**Closed source providers**

 - Retain control of their product

 - Need to understand the value they're creating

 - Have to be good at selling at whatever level they decide to go in at (CTO? Dev team? Individual developer?)

 - Must keep a close eye on competitors

 - (Unless they're large) have to be willing to write contracts that give key (or even all) customers rights in the source under certain circumstances

 - Have a straightforward business model (sell more = make more money)

 - Manifest success and failure by growing and going out of business (respectively)

**Open source providers**, on the other hand,

 - Are one of potentially many stakeholders in the product they create

 - Don't need to understand the value they're creating with the capabilities they deliver

 - Need to be good at marketing and social media and adequate at selling

 - Should track competitors but don't need to obsess

 - Can use licenses developed and refined by others to protect the specific IP position they want

 - Have a complex business model (no direct relationship between use of the product and revenues / profits)

 - Have no single markers for success and failure

It's straightforward (though it can be expensive) to go from a closed source to an open source model; it's virtually impossible to go the other way.

So for me, if you are very clear what value you are creating, for whom, and reached by what means - default to closed source. You may succeed or fail, you will both know which is happening and have a throw of the dice left, and you can manage the legacy.

And if you want scale to generate profit in proportion, you have no realistic alternative to closed source. (Not that it's impossible to achieve this in open source, but the successes tend to be very individual, there's no formula for success.)

In other cases, there are likely to be pros and cons either way. You'll likely resolve those best by engaging with prospective customers, partners and investors.


## Answer 39828

- posted by: [james](https://stackexchange.com/users/-1/5800-james) on 2012-06-11
- score: 0

There are lots of customers still buying licenses. And open source is not a recent trend, it's been around for a few decades. 

It depends on your library and your market. We've bought quite a few components/libraries over the years. Many products have a price for the library and a higher price for the source code option. We typically buy the source code (even at five times the price of the library) because it means we can control our own future if the supplier drops the product and reduces the risk for us. 

If you have a polished, complete library with documentation and examples, and have a good message on your website, you will be able to sell it. 

Is there a particular reason you are going to time-limit the license? "use the library for a certain period"  I doubt anyone will add a library to their product if it has a time limit on it. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
