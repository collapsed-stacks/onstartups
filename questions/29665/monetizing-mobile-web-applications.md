## Monetizing Mobile Web Applications

- posted by: [Shane Fulmer](https://stackexchange.com/users/-1/6675-shane-fulmer) on 2011-09-05
- tagged: `mobile-apps`, `mobile-payments`
- score: 2

What is the best way to accept payments in a mobile web application? Am I pretty much stuck with Paypal or Google Checkout, and having them take 30 cents for every transaction?


## Answer 40800

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-07-24
- score: 2

<p>If you're talking about a native app that needs to be in the "store" (IOS/App Store, Android/Play) there are platform restrictions to consider. Apple wants you to use their store for most uses (and takes a 30% cut).  There are companies like <a href="https://www.parse.com" rel="nofollow">parse</a> that make the <a href="http://blog.parse.com/2012/07/24/in-app-purchase/" rel="nofollow">in-app purchase</a> handling process simpler.  </p>

<p>HTML5 apps are browser based and free of these restrictions.  I'd second SpoiledTechie's advice to take a look at <a href="http://stripe.com" rel="nofollow">stripe</a> or <a href="http://recurly.com/" rel="nofollow">recurly</a> / <a href="https://www.braintreepayments.com/" rel="nofollow">braintree</a> for recurring revenue (read:subscription) plans. </p>



## Answer 35300

- posted by: [pdjota](https://stackexchange.com/users/-1/1355-pdjota) on 2012-01-26
- score: 1

<p>We integrate our application through a payment gateway such as <a href="http://www.authorize.net/" rel="nofollow">Authorize.net</a> so the customers can use their credit card directly. Most technology stacks have some type of library to integrate payments with them.</p>



## Answer 42166

- posted by: [RonGa](https://stackexchange.com/users/-1/218-ronga) on 2012-09-23
- score: 0

<p>what kind of application?  </p>

<p>While I don't have all the information, I have been using <a href="http://www.zooz.com" rel="nofollow">ZooZ</a> on native iOS and Android apps (for selling physical merchandise, not virtual goods, which Apple and Google have a monopoly on). I know they also support HTML5 web apps and I highly recommend them. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
