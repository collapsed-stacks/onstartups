## Need suggestions on naming payment options

- posted by: [Ankur Jain](https://stackexchange.com/users/-1/6146-ankur-jain) on 2011-04-20
- tagged: `ideas`, `payments`
- score: 2

We mainly use PayPal as our payment processor on our website. Of late we're seeing that PayPal is having issues with corporate credit cards. Moreover, going forward, PayPal won't accept payments more than $500 in a single transaction (It's due to our country's new regulations) 

So we're planning to integrate another payment processor - let's say XYZ.  

We still wish to keep PayPal as our default payment processor mainly because of the low fee involved per transaction (we're on PayPal's preferred rates) and the tight integration we have set up with it. XYZ though very good but it's a new entrant into the market and has higher per transaction fee involved.(almost 2X of PayPal)

Now we're thinking, how best to name these options when we integrate in our website. 

We thought of two possibilities

#1

![Option1][1]
 
XYZ is not so known so people may be reluctant to even select that. Given that PayPal can also process credit cards, we thought of -

#2

![Option2][2]

Which option you think would look/work better? Do you have any other suggestion?

Thank You!


  [1]: http://i.stack.imgur.com/u5iC9.png
  [2]: http://i.stack.imgur.com/lykSQ.png


## Answer 23732

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-04-20
- score: 2

<p>We faced a similar problem several months ago with our <a href="https://wyday.com/wybuild/buy/" rel="nofollow">wyBuild payment selection screen</a>. What we ended up with was a visual selection of the payment option and we defaulted to our preferred payment method (because it gives us the best rate). As of April 2011, this is what it looks like:</p>

<p><img src="http://i.stack.imgur.com/oCG8O.png" alt="wyBuild payment method selection"></p>

<p>Basically it uses a bit of jQuery magic to switch or hide the payment form based on the payment method.</p>

<p>If you're a <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM user</a> we're actually writing example code for PHP &amp; ASP.NET (C# and VB.NET) that lets you choose from multiple payment options (PayPal, Moneybookers, and Credit cards processed through Authorize.Net) in a similar form. The user can choose their preferred payment option and product keys are automatically send to the user when the order has been successfully charged. We plan to have this example out by the end of next week.</p>

<p>Maybe I'll also write a blog post about how to do it for more "general purpose" charges -- that is, non-software purchases.</p>



## Answer 23777

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-04-21
- score: 0

Another thing that comes to mind in your specific implementation is that if you can know the amount before the payment types are shown, you could skip offering Paypal as a payment option on sales over a certain amount. It would probably be good to have a link like "Why isn't Paypal an option?" on that page.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
