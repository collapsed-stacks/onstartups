## What are the ways to sell desktop applications

- posted by: [blez](https://stackexchange.com/users/-1/14175-blez) on 2011-11-02
- tagged: `software`, `payments`, `selling`, `registration`, `online`
- score: 5

I'm figuring the ways to sell software online. I want a service that is easy to use. PayPal is good, but I'm not sure if most of the people have PayPal. Also Fortumo is a good service, it works in most of the countries, by sending payed SMS. Are there other ways? And what's the most common way?

If PayPal is the best, can someone please provide me a service that uses PayPal to send serial keys from a database. Or something similar.



## Answer 32182

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-11-02
- score: 4

<p>From reading your question and the comment you made on another answer it seems like you're looking for either a completely licensing + payment solutions or you're looking for a payment solution that works with your own home-made licensing. I'll cover both options.</p>

<h2>Licensing + Payment processor</h2>

<p>I'm founder of the company that makes <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a> -- a licensing solution for Windows, Mac, and Linux. We actually have pre-made scripts that you can upload to your website that gives your user multiple options for payment. See: <a href="http://wyday.com/limelm/help/how-to-generate-product-keys-after-order/" rel="nofollow">How to generate product keys after an order</a>. We show how you can use one (or all) of the following payment providers:</p>

<ul>
<li>FastSpring</li>
<li>MoneyBookers (a.k.a. Skrill, a.k.a. the PayPal of Europe)</li>
<li>PayPal</li>
<li>Authorize.Net</li>
</ul>

<p>Here's what it would look like on your site:</p>

<p><img src="http://i.stack.imgur.com/gJI9H.png" alt="enter image description here"></p>

<h2>Home-made licensing + Payment processor</h2>

<p>The second option is to build it yourself.</p>

<ul>
<li>PayPal actually has the best documentation and code samples. See the <a href="https://www.paypal.com/ipn" rel="nofollow">PayPal IPN (Instant Payment Notification)</a> article.</li>
<li>Authorize.Net also has some <a href="http://developer.authorize.net/downloads/samplecode" rel="nofollow">pretty extensive code samples</a>.</li>
<li>MoneyBookers is a bit weak on the code samples, but I <a href="http://wyday.com/blog/2011/automate-moneybookers-skrill-using-status_url-ipn-php-asp-net/" rel="nofollow">wrote a blog post that covers 99% of what you need to do</a>.</li>
</ul>



## Answer 32170

- posted by: [Amenti](https://stackexchange.com/users/-1/9272-amenti) on 2011-11-02
- score: 2

<p>There are several payment providers like:</p>

<ul>
<li><a href="http://www.fastspring.com/" rel="nofollow">FastSpring</a></li>
<li><a href="http://www.cleverbridge.com/corporate/" rel="nofollow">CleverBridge</a></li>
<li><a href="http://www.shareit.com/" rel="nofollow">ShareIt</a></li>
</ul>

<p>They usually handle all the pain of different payment types, serial number distribution and so on for you and you never have to store customer data  which is important in itself.</p>

<p>I found FastSpring very transparent, easy to use and they provided good customer support so far.</p>



## Answer 32206

- posted by: [Steven at FastSpring](https://stackexchange.com/users/-1/14199-steven-at-fastspring) on 2011-11-03
- score: 2

Steven here from FastSpring.  

I just wanted to reach out and let you know that we accept multiple payment options including PayPal and all major credit cards, and we support a wide range of currencies.

We also support a variety of ways to distribute license keys.  If you're looking for a do-it-yourself solution, it's possible we could call your database to distribute the codes to your buyers upon purchase.  We can also pull from a provided list, or accept a JavaScript algorithm.

However, if you're looking for something out-of-the-box, Wyatt provides a great solution above, and we do also have built in integration with Software Passport, Soraco's QLM, ByteShield, Aquatic Prime, and CocoaFOB.

Feel free to contact me for further questions/details.

-Steven


## Answer 32171

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2011-11-02
- score: 1

Not sure what exactly you are asking, but I wrote a simple php script to email license keys after a paypal payment was made.  There are quite a number of resources online that will provide the code to show how it is done.

PayPal has an API for this.

If you are not a developer I am sure you could pay someone to do it for you - probably for less than $1000 and likely even cheaper than that


## Answer 32213

- posted by: [aoporto](https://stackexchange.com/users/-1/11579-aoporto) on 2011-11-03
- score: 0

E-junkie integrates with PayPal and lets you provide license keys: http://www.e-junkie.com/ej/help.selling-codes.htm



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
