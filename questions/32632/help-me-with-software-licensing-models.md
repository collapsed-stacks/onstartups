## Help me with software licensing models?

- posted by: [lukeluke](https://stackexchange.com/users/-1/14449-lukeluke) on 2011-11-15
- tagged: `licensing`, `software-licensing`
- score: 4

I have developed a portable C++ software library. I would like to discuss how to license that software (license models). Consider that the library price would be  < 5.000 EUR and that it can be used for mass market products (but not only). What I want to do is to license the software for commercial purpose. So, basically, I want to:

1. Sell library and documentation at price X
2. Gain Y% royalties on the net income of a given product.

I know that I should consult a lawyer, but before that I would like to know your personal experiences.

First, is it reasonable to license software for a single product named XYZ (so that if you want to use it for another product, you must buy another license)? Or it is better to license the software for an infinite number of products? Clearly, in the first case, the prices for X would be different (a license for a single product should cost less then a license for an infinite number of products). But the royalties? Should Y be set to a different quantity?

Second: what to do with library updates? Should I make the updates freely available to a licensee or should an update (that contains major updates, not only just bugfixes) be considered as a new product to be licensed again?

Another question is: where can I find resources that on the web on software licensing (what are the most common models, what are the best practices and so on)?



## Answer 32637

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-11-15
- score: 6

<blockquote>
  <p>Another question is: where can i find resources that on the web on software licensing (what are the most common modalities, what are the best practices and so on)?</p>
</blockquote>

<p>This is a good question unfortunately the resources on the web fall into 2 main categories:</p>

<ol>
<li>Whitepapers by licensing companies: dull, biased, marketing-speak with scant useful information. These whitepapers are more interested in selling you something you don’t need rather than informing you about how proper licensing works.</li>
<li>Forums with 1% good information mixed inseparably with the 99% garbage information.</li>
</ol>

<p>You can get some good information from Whitepapers and some good information from forums. But you really have to have either [a] a great BS detector or [b] lots of experience using/creating licensing to be able to tell the good info from the garbage (to put it nicely).</p>

<p>That being said, I'm finishing writing a free eBook on building, buying, and using licensing. It's currently in a "near final draft" form (lacking illustrations and a pretty layout), but if you email me I can send you a draft (email me at wyatt@wyday.com ).</p>

<p>You're probably thinking <strong>"What qualifies Wyatt to write a book about licensing?"</strong> The answer is that I'm founder of the company that makes <strong><a href="http://wyday.com/limelm/">LimeLM</a></strong> an online-activation (a.k.a. hardware-locked) licensing solution for Windows, Mac, and Linux. The ebook that I'm writing isn't some thinly veiled whitepaper selling LimeLM. It's an attempt at curing the huge amount of ignorance about licensing that exists.</p>

<p>We'll have the free ebook available on our site in a few months, but like I said if you want a draft copy to look over just email me.</p>

<h2>Types of licensing</h2>

<p>The types licensing fall into 3 general groups:</p>

<ol>
<li>Serial only licensing</li>
<li>Hardware-locked licensing (online activation, USB dongles, floating licenses, etc.)</li>
<li>"Snake oil"</li>
</ol>

<p>Quick aside: the point of licensing <em>isn't</em> to stop crackers from cracking your software. <strong>The point of licensing is to increase your revenue by preventing casual piracy</strong> (using serials over and over again). There is real money to be made by stopping casual piracy.</p>

<h2>1. Serial only licensing</h2>

<p>"Serial" licensing is where you have a product key like "ABCD-EFGH-IJKL-MNOP-..." and that's it. A user or company can use the product key over and over and there's nothing you can do about it.</p>

<p>For almost every case I recommend avoid "serial only licensing" -- use hardware-locked licensing instead. Hardware-locked licensing like online activation gives your absolute control over how your software is used and you can truly increase your revenue by preventing casual piracy.</p>

<p>However you mentioned the one case where "serial only licensing" is the only good choice: when you're making a software component that's used by developers within their own apps.</p>

<ul>
<li><strong>Advantages</strong>: It's simple for you to build and simple for the customer to use.</li>
<li><strong>Disadvantages</strong>: You have absolutely no control over how many times a company/user uses your software. You will lose a considerable amount of revenue using "serial-only" licensing.</li>
</ul>

<h2>2. Hardware-locked licensing (online activation, USB dongles, etc.)</h2>

<p>As I mentioned above, this is the best type of licensing for 99% percent of the cases. There are lots of types of hardware-locked licensing but the most popular variation is "online activation" (like Windows Activation or MS Office activation). The Reader's Digest version of proper online activation is:</p>

<ul>
<li>Customer enters a serial.</li>
<li>Serial + the computer's unique "fingerprint" is sent to an activation server.</li>
<li>If the server allows the activation then the Serial + fingerprint are cryptographically signed and sent back to the user.</li>
</ul>

<p>The last 2 point are huge topics and it takes a lot of work to get it right but, as I said, it's the condensed version. I can explain them in-depth if you want.</p>

<ul>
<li><strong>Advantages</strong>: You have complete control over how many times your customer uses your software. This can mean a significant increase in revenue.</li>
<li><strong>Disadvantages</strong>: It's hard to build this licensing in-house and there are only a few 3rd party companies that do hardware-locked licensing well. (LimeLM is one of the few that does hardware-locked licensing well -- but you can email me and I'll send you a list of competitors we respect).</li>
</ul>

<h2>3. "Snake oil"</h2>

<p>This is a huge category. An awful lot of 3rd party licensing is snake oil. Things like "anti-debuggers", "in memory encryption", and other nonsense sound like good ideas, but in practice they hurt your bottom line.</p>

<p>I can go into this in depth if you want. But this answer is becoming War &amp; Peace, so I'll just leave that perfunctory note for now.</p>

<hr>

<blockquote>
  <p>First, is reasonable to license a software for a single product named XYZ (so that if you want to use it for another product, you must buy another license)? Or it is better to license the software for an infinite number of products? Clearly, in the first case, the prices for X would be different (a license for a single product should cost less then a license for an infinite number of products). But the royalties? Should Y be set to a different quantity?</p>
</blockquote>

<p>This is a huge question. Like I said above, in your case you should use "serial only" licensing (because you're making a developer component). This means the only way you have to enforce your agreements is by taking their word for it.</p>

<p>I know that's not the answer you want. Sorry. The licensing options for developer components are truly limited.</p>

<blockquote>
  <p>Gain Y% royalties on the net income of a given product.</p>
</blockquote>

<p>That's a tough sell. It's easier to sell a very expensive product that's royalty free than to sell a cheap product with royalties. Tracking &amp; collecting royalties will be a huge pain in the ass for you &amp; your customers. I can guarantee you that any company that sees that your product has royalties complicating it will first think "can we build this in-house?". And unless your product has some secret sauce, they will almost always answer "yes, we can build this in-house".</p>

<p>If I were you I would think twice about the royalty model.</p>

<hr>

<blockquote>
  <p>Second: <strong>what to do with library updates?</strong> Should i make the updates freely available to a licensee or should an update (that contains major updates, not only just bugfixes) be considered as a new product to be licensed again?</p>
</blockquote>

<p>If I were you I would ask this as a separate question on this site. You'll probably get better answers to it.</p>

<p>My advice: never ever offer "free updates forever". Serious buyers will run away from companies that make such a declaration. You're basically declaring "We'll support this product for about 2 years and then we'll realize we made a huge mistake and either (a) stop supporting it or (b) go back on our promise and have paid upgrade."</p>

<p>Short answer: just do paid upgrades from the start. It's better for your bottom line and knowledgeable customers will take you seriously.</p>



## Answer 32672

- posted by: [BMitch](https://stackexchange.com/users/-1/11142-bmitch) on 2011-11-16
- score: 0

I prefer a license for a one time initial fee plus annual maintenance for a specific set of features. Price the license for a defined usage (number of machines, users, transactions, etc). Clients should get bug fixes and enhancements for those features as long as they pay the annual maintenance. When you expand the product to a new set of features, that would be an additional initial and annual maintenance fee.

The result is a long term business model that's cash flow positive. Otherwise, you're promising something you can't actually provide and your customers will know it. The upfront fee should make you some profit or at least break even from the upfront development, if you hit your sales targets. The maintenance fees should more than cover your operating expenses going forward. This way, if a customer stops paying the maintenance fees, your business is still sustainable.


## Answer 32677

- posted by: [user9982](https://stackexchange.com/users/-1/9982-user9982) on 2011-11-16
- score: 0

I know one area where royalties do seem a good choice - 3d engine licensing (which basically is a library + tools), with the most famous example:
http://www.udk.com/licensing
You should take a look at their scheme and decide how it applies to your market (you didn't mention what it is).

They want 99$ upfront (some kind of dummy fee really, to pay for bandwith perhaps?) and 25% royalties on all revenue over 50 000$ generated by all your products which use their technology. This is a great plan as the revenue threshold is just about the level where there may be some real income (revenue minus development costs) and it is abstract enough to lure more people into learning their technology. They deliberately filter out those developers who earn less because it would be realistically difficult to get those royalties out of them. And your license restrictions are worth something only if you can enforce them in practice (hence Wyatt's answer, although from another angle).

As to the lawyer part - no, I don't think you need a lawyer at this stage. You can anylyze existing licensing schemes and EULAs of similar products. They do seem daunting but there is nothing you can't understand. Probably your final EULA will consist from parts of other EULAs with only small modifications (mine does). 

The part to remember is still that license restrictions are worth something only if you have a good chance of enforcing them, via technical or other means. If you can't enforce something from the majority of users of your library, then perhaps it's better to act generous and give it up.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
