## Building a service around external APIs

- posted by: [Leonid Mirsky](https://stackexchange.com/users/-1/12527-leonid-mirsky) on 2011-09-16
- tagged: `strategy`, `api`
- score: 1

I am thinking about building a service around some other company APIs. However, prior of diving into some code, I would like to evaluate all the strategic aspects of such a "one way partnership".

Some aspects I thought about:

1. My service uptime is totally dependent on the third party API, this means that I won't be able to provide a best service I might want to.

2. As far as I know, APIs are subject to rapid changes, so basically I can find myself updating my code more than I intended to (or even find myself running against the clock).

Can someone share, from his experience, some thoughts on this subject? What are the main things I should take into consideration? Are there some services which can help me with these concerns?


## Answer 30157

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-09-16
- score: 0

<p><strong>Impact of change</strong>.</p>

<p>It would depend on your archetecture, the abstractions you place between "your world and theirs". </p>

<p>If the form changes, but the function remains the same (ie, facebook still has a social graph but you use SQL OR XML services OR Rest/JSON OR the next big magic thing). </p>

<p>If you can manage this key issue in your design, then YES you will be rewriting your integration piece with them several times over BUT with the right design it shouldn't impact 10% of your application (which is the I/O piece).</p>

<p><strong>Number of "suppliers"</strong></p>

<p>Is there only 1 "supplier" or could you have several "eg News feed from Twitter AND Facebook" </p>

<p>If your aggragating several services together (say, all freight carriers into one API for requesting and tracking freight OR Extracting banking summary data securely OR whatever) </p>

<p>While Joels, nickels infront of the steamroller can be accurate ... </p>

<ul>
<li>For well established businesses this is very important to be able to integrate into a stream ... if you have done it, they don't have to.</li>
<li>For single sources like facebook or Twitter, they can either compete against you or buy you, make it obvious which choice they should make by hard function to perfect, marketshare takes too long to aquire on your own, your know the space better than them ... simply easier to buy yours and your on a winner.</li>
<li>If you tie several APIs together like <a href="http://ifttt.com/" rel="nofollow">ifttt</a> then an create something bigger then your both cementing your suppliers position and creating your own place in the market.</li>
</ul>

<p><strong>Revenue model</strong>.</p>

<p><strong>From the supplier</strong> who is also paying you for the transaction then you may be in trouble, their plans change, your out ... if your volumes high enough then make hay while the sun shines. </p>

<p><strong>From the general public paying for your service</strong>. This is better because your then if you get traction your a viable buyout target.</p>

<p><strong>From advertising</strong>. If you can get a high enough volume, or can segment your market well for the advertiser then your in luck.</p>

<p><strong>From a group of businesses</strong>. If a range of busineses are paying for you to "provide your piece of the puzzle", provided it isn't their core business they will usually be happy to pay you to deal with it IF your cheaper/safer than them doing it.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
