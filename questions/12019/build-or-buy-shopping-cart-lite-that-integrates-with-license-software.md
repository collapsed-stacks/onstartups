## Build or Buy? Shopping cart lite that integrates with license software?

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-06-11
- tagged: `shopping-cart`, `licensing`
- score: 1

So I’m finishing up on my project, a real-time dictionary that works while you type in anything.  I’m now getting to where I’m thinking through the integrating a license key to the buying of the software.  That my software will be at version 1 at release makes me think that I won’t have the features quite right so but want enough protection that it would be an inconvenience to steel it and that if you like the product you’ll buy it. 
 
So I want the minimum shopping cart (not really a cart but a simple buy) and minimum license integration.   Looking at google cart and considering reviewing paypal as well.

I’m thinking for this first version that what I am really looking to achieve is the realization that the product and pricing are valid.  So I am looking for that solution that makes it really easy for a customer to buy.

Suggestions on to buy or to make?




## Answer 12020

- posted by: [Stefanos Tses](https://stackexchange.com/users/-1/3178-stefanos-tses) on 2010-06-11
- score: 1

If you use a payment processor like AvanGate or FastSpring they offer licensing and shopping cart together, so you don't have to build your own.

From my, very recent experience, Paypal is the easiest to integrate but has no licensing as far I know.

I'm using AvanGate on my site and they offer both licensing with product key delivery and other more advanced options. Shopping cart is pretty advanced and has many options in pricing and customization.

Is not that easy to setup as Paypal thought.


## Answer 12030

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-06-11
- score: 1

<p>If you're coding, here's a simple <a href="http://net.tutsplus.com/tutorials/php/using-paypals-instant-payment-notification-with-php/" rel="nofollow">PHP &lt;-> paypal ipn integration tutorial</a>.</p>

<p>If you're not coding, why not use a cms framework like <a href="http://joomla.org" rel="nofollow">joomla</a> and get a <a href="http://extensions.joomla.org/extensions/e-commerce/payment-systems" rel="nofollow">payment plugin</a>?  </p>



## Answer 12635

- posted by: [Jas Panesar](https://stackexchange.com/users/-1/1368-jas-panesar) on 2010-07-09
- score: 1

If you experience any type of growth in your shopping cart experience, you will be re-inventing the wheel, from scratch, no matter how simple it looks now.

If you're using an off-site shopping cart (paypal, shopify, etc) use them and simply integrate and brand.  

Where you end up behind the ball over time is the same hardening/security everyone has to build into every single site.  Building a cart from scratch is an exercise in building some pretty serious technical debt, unless your needs are so special that they can't be fitted or adapted to something already out there.

If your core business is the carts, do it.  If your core business is something else, find something close to the purchasing process you want and automate it some more.

I had good luck doing that with a product called Cartweaver 10 years ago.  It has stayed with me and I've customized and developed it over the years for different projects.  I'm sure you can find your equivalent.

All the best!  Share what you end up doing and why.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
