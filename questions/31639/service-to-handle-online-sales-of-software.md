## Service to handle online sales of software

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2011-10-19
- tagged: `software`, `selling`, `order`
- score: 5

I am selling a little niche app on the app store. http:www.finaltouchapp.com

For several reasons I also want to sell it directly from the web page. Are there any out of the box solutions that you can plug into your site or do I have to create it from scratch with paypal etc.?

Edit

Thanks for all the answers

I also found:

http://pulleyapp.com/

http://www.fetchapp.com/


## Answer 31643

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-10-19
- score: 5

<p>This is a good question -- it's smart that you're looking to selling your software on your own website. Now you get to keep a bigger cut of the app price.</p>

<p>Keith's answer is right about the steps if you want to build it yourself. Or a more broad overview of what you need is this:</p>

<ul>
<li><strong>A payment provider</strong>: It doesn't need to be a merchant account, but rather it can be anything like FastSpring, PayPal, or any one of the thousands of payment providers. There are some big hurdles for getting a merchant account (rather than something like FastSpring). One downside to a merchant account is that you need to maintain PCI compliance. This can be expensive.</li>
<li><strong>A licensing system</strong>: Since you'll be operating outside of the Mac app store you'll need to add your own licensing to your software. You can either build this yourself or purchase from a third party.</li>
</ul>

<p>I'm founder of the company that makes <a href="http://wyday.com/limelm/">LimeLM</a> -- a licensing solution for Mac, Windows, and Linux. We have <a href="http://wyday.com/limelm/help/how-to-generate-product-keys-after-order/">articles and some "drop in" code</a> written for Authorize.NET, PayPal, MoneyBookers, and FastSpring. You can just take the code, modify the price and a few other configuration options, then upload it to your website.</p>

<p>Our customers prefer the FastSpring option (see: <a href="http://wyday.com/limelm/help/automate-license-generation-with-fastspring/">Automate license generation with FastSpring</a>) because they have to add 0 code to their own website. You can just paste the license generation code directly into your FastSpring dashboard and add a link to the checkout page on your website. This way a customer can just checkout through FastSpring and get their product key emailed to them immediately.</p>

<p>We have a <a href="http://wyday.com/limelm/signup/">free plan</a> if you just want to kick the proverbial tires before you commit. Also, <a href="https://www.fastspring.com/signup.php">FastSpring has a "sandbox" account</a> that you can try out as well. So, if you're looking for a ready-made solution then FastSpring+LimeLM is a good place to start.</p>

<p>Tell me if this helps.</p>



## Answer 31640

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2011-10-19
- score: 1

<p>When you consider Apple is taking 1/3, it is worth considering the costs to sell your software directly through your own web site.</p>

<p>There are several online services that will help you, <a href="http://www.esellerate.net/" rel="nofollow">esellerate</a> is a big player, and <a href="http://www.kagi.com" rel="nofollow">Kagi</a> is an oldie and of course there's <a href="https://www.paypal.com/" rel="nofollow">PayPal</a>. These services come with a price. Sometimes a really steep price.</p>

<p>In the long run, it's not tough to build your own and save money. There's 3 components in a build your own solution:</p>

<ol>
<li><p><strong>Merchant Account</strong>.
It's actually pretty easy to setup a merchant account (usually through your bank). Chase Bank is really small business friendly these days with super competitive merchant accounts. We use Chase and Authorize.net for processing, costing us well under 4% net per transaction.</p></li>
<li><p><strong>Processing payments from your web site</strong>.
There's a bunch of e-commerce plugins for your web site at a very low cost.</p></li>
<li><p><strong>Registering/distributing purchased software</strong>.
You can go with auto generated license keys with free downloads. Some of the plugins for e-commerce include license generation code that you can incorporate into your software to activate it as purchased. Some plugins also provide a link to  the software (somewhat similar to Apple) so there's no serial number/activation codes involved.</p></li>
</ol>



## Answer 31647

- posted by: [Kekito](https://stackexchange.com/users/-1/5898-kekito) on 2011-10-20
- score: 1

<p>I use <a href="http://bitbuffet.com/" rel="nofollow">bitbuffet.com</a>.  They provide an easy way to securely sell files and get paid via PayPal.  They don't do anything to help you with license keys and the like, but it is cheap and easy to use.  Also, the money from sales goes directly to your PayPal account.</p>

<p>There a number of companies that provide similar services as well.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
