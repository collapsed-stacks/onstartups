## Looking for payment system with licensing (key delivering) for .NET software

- posted by: [Miki22](https://stackexchange.com/users/-1/11492-miki22) on 2011-06-24
- tagged: `payments`, `license`
- score: 6

I developed .NET application and planning to sell it on monthly/yearly subscription plans.
At first I found that Plimus has licensing system and everything else that I need, but when I finally decided to test it I found that they have many bugs in their system and it's imposible to use licensing system with recurring payments.

Can you recommend some other payment processor that can accept paypal but also direct credit cards
and that has all fancy options like discounts coupons, recurring payment and most important license key deliver system that can control customers license based on monthly payments.

Thanks,
Nikola


## Answer 26727

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-06-24
- score: 2

<p>I can confirm Plimus is really awful for license key management. The email exchange we had with their technical support recently regarding those bugs make me think they don't have the staff needed to make a professional API.</p>

<p>We are still using it, but plan to move away as soon as possible.</p>

<p>That said, I highly suggest you to have a look at <a href="http://recurly.com/" rel="nofollow">Recurly</a>. This is an amazing platform. The only reason why we don't use yet is that they don't support <a href="http://www.ogone.be/" rel="nofollow">Ogone</a>, our payment gateway.</p>

<p>Recurly provides a <a href="http://docs.recurly.com/transparent-post/basics/" rel="nofollow">professional &amp; flexible API</a> that will allow you to host your own serial key generation tool.</p>



## Answer 26728

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-06-24
- score: 2

<p>I'm founder of the company that makes <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a>, a hassle free licensing and online activation system. That is, LimeLM is hardware locked licensing that integrates with all programming languages (.NET, Java, C++, etc., etc.) and allows for advanced functionality like recurring billing for desktop apps (like you're looking for) among other things. There are lots of ways you can do recurring billing in your apps, and we have an <a href="http://wyday.com/limelm/help/saas-and-time-limited-licensing/" rel="nofollow">article talking about monthly update subscription</a>.</p>

<p>Obviously you don't have to do SaaS licensing that limits updates, but that's the most popular option. You can choose to limit your application outright based on their subscription status.</p>

<p>But to address your question more directly, we have multiple fully-written payment integration examples that deliver product keys the instant an order is processed. See: <a href="http://wyday.com/limelm/help/how-to-generate-product-keys-after-order/" rel="nofollow">How to generate product keys after an order</a>.</p>

<p>In that article we talk about delivering product keys whether your payment platform is PayPal, Moneybookers, or Authorize.Net (i.e. direct credit card payment). Or you can enable all the payment platforms and have a payment selection screen where the user can choose their favorite payment method:</p>

<p><img src="http://i.stack.imgur.com/SJYUn.png" alt="enter image description here"></p>

<p>The actual example code we have is written for 3 languages so you can choose whatever works best for integrating with your website workflow. That is, the example code we have is written in PHP and ASP.NET (C# &amp; VB.NET) -- just set a few configuration options and drop the code (in whichever language) into your website.</p>

<p>You're not limited to PayPal, Moneybookers, or Authorize.Net -- those are just the examples we've written. We have customers that integrate <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a> with all sorts of other payment platforms (Cleverbridge, Plimus, FastSpring, RegNow, etc., etc.). You're not limited to PHP &amp; ASP.NET either.</p>

<p>We can help you get up and running by walking you through everything you need (coupon processing, handling renewals, etc., etc.). Just shoot me an email.</p>

<h2>Hackers, crackers, and thieves</h2>

<p>Since you brought up cracking let me quote my own catch-phrase:</p>

<blockquote>
  <p><strong>If it exists on a computer it can be cracked.</strong></p>
</blockquote>

<p>There are lots of companies that sell snake oil (wrappers, obfuscation, in memory virtual compilers, etc., etc., etc.) but these don't add <em>any</em> extra protection whatsoever. The best these snake oils can do is add a few minutes to the time it takes to crack your app. For an in-depth study of this point see this study: <a href="http://www.wisdom.weizmann.ac.il/~oded/p_obfuscate.html" rel="nofollow">On the (Im)possibility of Obfuscating Programs</a>.</p>

<p>This raises the question: "If all licensing is crackable what's the point of having it at all?" The answer is this: <strong>casual piracy</strong>.</p>

<p>Casual piracy (that is, a person or company using the same product key over and over again) is a greater threat to your business than crackers. The Business Software Alliance has done studies on piracy within business and I believe the most recent worldwide percentage is 48.9% of all software is pirated (it's lower in some regions and much higher in other). So you should always use hardware-locked licensing (like <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a> or something you build in-house) rather than just simple "serial" protection.</p>

<p>I can go into what hardware-locked licensing means if you want but it's probably easiest to give examples: Microsoft Windows Activation or Microsoft Office Activation. That is, a customer can on install your software on a finite number of computers. If you were to build it yourself you'd make a "fingerprint" of the computer (an ID generated from the components of the computer) and you'd use public-key encryption on your servers to cryptographically sign the message that your app would then use to verify the activation. (I can go into further details if you want, but this answer is getting a bit lengthy).</p>

<h3>Dealing with cracked software on the web</h3>

<p>The way you handle crackers is to find all pirated versions of your software on the web and send DMCA notices. A very high percentage (> 90%) of these hosting sites remove illegal files based on DMCA requests. But it's a whack-a-mole proposition. That is, when you get 20 sites to remove your files, 20 more pop up the next week. </p>

<p>We've thought about this problem too, which is why we created <a href="http://wyday.com/pirate-poacher/" rel="nofollow">Pirate Poacher</a>. This is a service we offer (free for LimeLM customers) that handles the tracking &amp; removing of pirated versions of your software for you.</p>

<p>Tell me if this helps.</p>



## Answer 27041

- posted by: [logicnp](https://stackexchange.com/users/-1/11650-logicnp) on 2011-07-02
- score: 0

<p>DISCLAIMER - We are the developers of <a href="http://www.ssware.com/cryptolicensing/cryptolicensing_net.htm" rel="nofollow">CryptoLicensing</a>.</p>

<p>Do not mix up your payment processor and licensing. Most payment processors today have the ability to do an HTTP POST to a URL of your choice with information about the order and customer.  Your page can then generate licenses and deliver it to the customer.</p>

<p>Our own product CryptoLicensing has ready-to-use e-commerce pages for a variety of payment processors including Plimus, Shareit, Paypal, etc. When the payment processor makes the POST to these pages, a new license is generated using the CryptoLicensing API and sent to the customer.</p>

<p>You can customize this as per your needs. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
