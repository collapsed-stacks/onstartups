## Will Open-Sourcing my SaaS solution positively impact revenue?

- posted by: [A T](https://stackexchange.com/users/-1/15651-a-t) on 2012-01-16
- tagged: `sales`, `saas`, `revenue`, `open-source`, `software-licensing`
- score: 4

I have yet to go public with my SaaS startup, and am considering releasing it under an open-source license.

Below are some thoughts I've collated in answer to this question:

No
==

 1. As competitors could just download our project and sell at a more competitive monthly rate 
 2. As companies could just setup there own build and not pay us

Yes
===

 1. As the developer community will like the license (good publicity)
 2. As this will solve customer skepticism such as: “What if you’re not around in a year” will be combated with we're open-source, so you can e.g.; get others to host
 3. Since others will fix bugs and enhance our service with us 
 4. Because small businesses will be outpriced from infrastructure or skillset needed
 5. Because large businesses will want the support (someone to blame/ring-up!)

----------
What are your thoughts: **will Open-Sourcing my SaaS solution positively impact revenue?**


## Answer 34870

- posted by: [dnbrv](https://stackexchange.com/users/-1/15284-dnbrv) on 2012-01-16
- score: 2

The open-source business model works only if the product requires extensive configuration support and/or training. If the product is neither, you will be out of money and out of business faster than you expect. Thus, sticking to the regular tiered subscription model will generate more guaranteed revenue.


## Answer 34890

- posted by: [SpamapS](https://stackexchange.com/users/-1/15665-spamaps) on 2012-01-17
- score: 2

If your product is novel, and you believe that you will be able to profit greatly from each innovative step that you take early in the process, then open source doesn't make much sense. There's no entrenched player that you're trying to catch up to, so you don't need to enlist the help of others.

The only reason to open source something when you are in a position to profit off each and every investment in the code base would be that it is not part of your core competency, and you know that it will not evolve and grow with other advances in technology. This is basically how Unix became dominant when produced by AT&T (Unix's license and the market was in such a state that it was basically like open source for the time, which is why for instance BSD Unix evolved out of said code base), because they did not want to be in the OS business. If they had productized it, some other OS would have made the necessary innovations to bring cross-platform computing and the resultant benefits to the computing world.

If, however, the advantage that you have over your competition is access to data in a timely manner, or extremely high caliber service, and you need to differentiate yourself from your competition, then it makes some sense to open source the bits that you want your users to be able to improve for themselves.

Personally I think in the SaaS world, this is often better accomplished through having a strong, well documented public API. Look at the success of Amazon's Web Services as a perfect example for that.


## Answer 34863

- posted by: [Tom Squires](https://stackexchange.com/users/-1/11392-tom-squires) on 2012-01-16
- score: 0

Possibly. Red hat and quite a few other companies make plenty of money using the open source model (charging for premium support and enhancements). Being free to try should greatly improve your early adoption. 

Its not a standard model however and you rely very heavily on the larger companies adopting your software as they are the ones who will give you the big support contracts.

Since we dont have the information to asses your product or your customers, I suggest you do some market research and based on the profile of your customers make the choice. Unless there is strong evidence to suggest there is a commercial advantage with going open source I suggest you stay closed. Its much easier to open something up later down the line than try to re-close an open product.


## Answer 34864

- posted by: [jbcolmenares](https://stackexchange.com/users/-1/14024-jbcolmenares) on 2012-01-16
- score: 0

I'm in the same or similar spot as you. I'm trying to answer the following questions:

- being open source could greatly increment the number of users. If my business model implies viral grow, this can be very usefull. Does my business model fits in a viral grow model? That is, my business model implies that I can make money incrementing the number of users, and that as a consequence of the usage of my product the user will bring more users.

- maybe the answer to the previous question was negative. That is, my "engine of growth" could be more of a paid model, in which case instead of the software I would need to focus on selling the support. That's a whole different business model. It depends more on big companies willing to pay you. And you have to show you can give the support they would need.

There is a lot of ground to cover between this two options. You could implement a very simple open source version, and a more sophisticated closed one for example. But that is dangerous.

How much capital do you have to start? if little, offering support can be challenging or impossible. At least, support for big companies, that are the ones that usually buy support. Another way to go is having a big retention rate, so that customers will keep using your software for a long period of time, and paying for it. This is the option I like more for SaaS, unless you have a very viral product or aimed for very big industries, which means you need lot's of cash to start.
 
I would also agree with Tom in his advice.

Cheers.


## Answer 34873

- posted by: [jrg](https://stackexchange.com/users/-1/12807-jrg) on 2012-01-16
- score: 0

<p>Yes.</p>

<p>Open source it, for a few reasons:</p>

<ul>
<li><p>First, if you open source it, you can get the community involved. If developers think its cool, they'll help. <a href="https://github.com/mojombo/grit" rel="nofollow">Github open sourced their Ruby Git bindings</a>, to great effect.</p></li>
<li><p>It will help you figure out if its really worth it - if developers (in other words, the folks you're trying to reach out to) think its worth contributing to/making better, they will also think its worth using, thus proving your "market value" (probably the wrong word, but it gets the point across)</p></li>
</ul>



## Answer 34882

- posted by: [Mab879](https://stackexchange.com/users/-1/15662-mab879) on 2012-01-16
- score: 0

I would no to the whole app. I would say yes to a part of site, like authentication, JS / CSS elements, etc. 


## Answer 35030

- posted by: [Walter Heck](https://stackexchange.com/users/-1/12983-walter-heck) on 2012-01-21
- score: 0

We open sourced all the building blocks for http://tribily.com, and here are the reasons:

* we believe in openness and transparency as a way of gaining trust. We don't have anything to hide
* we believe that by keeping in mind that everything we create will be open sourced we are more inclined to do things in a 'correct' repeatable way, thus making us end up with a nicer product tech-wise.
* we believe that open sourcing the building blocks to our service is not the same as open sourcing the service. A competitor would still need the know-how and invest the time and money to get to the same point.
* we believe that by releasing all the tech stuff, we keep ourselves competitive and innovating, it is the best way to stay ahead of competition.

So far, it works well although we'd like to see more participation in our released projects.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
