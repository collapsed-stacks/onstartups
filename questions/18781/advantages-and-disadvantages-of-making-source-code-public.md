## Advantages and Disadvantages of Making Source Code Public

- posted by: [user6488](https://stackexchange.com/users/-1/6488-user6488) on 2011-01-10
- tagged: `competition`, `open-source`, `webapp`
- score: 6

I like the idea of open source collaboration and making our code for our application we are building public on github.  This would allow people to give their input and even allow certain parts of the application to be built faster. 

I worry there is a risk in someone using the code to build a competing app. 

We can't trademark the business model, but would opening it up make it much easier to copycat us and start competing?  Anyone with a big enough budget could easily build out an app like this, but that doesn't mean that they would embark on the time and cost of doing so.  Would it enable it to be done that much easier? 


## Answer 18805

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-01-11
- score: 7

<p>This is an interesting question. It's hard to know the right answer for you without more details about your product, however I'm inclined to say you shouldn't open source your project. I only say this because the <em>reasons</em> you want to open source your app aren't realistic:</p>

<blockquote>
  <p>I like the idea of open source collaboration and making our code for our application we are building public on github.</p>
</blockquote>

<p>Unfortunately most open source projects live or die based on the work of the founding team (whether it's one person or many). In other words, the biggest contributions you'll get is small bugfixes and maybe minor functionality additions. No one will help build your business for you.</p>

<h2>Reason to open source your app</h2>

<p>If you can split your product into separate components you could open source bits of your app to great success. Without knowing the specifics of your app I can't tell you how <em>you</em> should split your app. Instead I'll explain how we open sourced about 2/3 of our product and attracted large customers because of it:</p>

<p>At our company we take a hybrid approach for our updater suite, <a href="http://wyday.com/wybuild/">wyBuild</a>. There are 3 parts to the app:</p>

<ol>
<li><a href="http://wyday.com/wybuild/">wyBuild</a>: design and build the updates [<strong>closed source</strong>]</li>
<li><a href="http://wyday.com/wyupdate/">wyUpdate</a>: the actual updater program that our customers include with their app [<strong>open source, BSD</strong>]</li>
<li><a href="http://wyday.com/wybuild/help/automatic-updates/">The AutomaticUpdater</a>: an optional component that our customers can include with their app that automates the entire update process [<strong>open source, LGPL</strong>]</li>
</ol>

<p>Because the "parts that did the updating" were completely open source we have been able to get large orders from Fortune 500 companies. Invariably the reason these companies end up purchasing wyBuild is that the CTOs first encountered the source code. I sincerely doubt we could have attracted some of these larger clients if our product was completely closed source. At least not without a couple of million dollars more in our advertising budget.</p>

<h2>To open source or not to open source...</h2>

<p><strong>It depends on what type of app your making.</strong> There <em>are</em> valid (and profitable) business cases for open sourcing your app; our story is a single anecdote, but there are similar cases at both small and large companies.</p>



## Answer 18782

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2011-01-10
- score: 6

One big disadvantage is if you make your source code public under an open/free software license, you will be very unlikely to ever make money from it. Don't listen to the open source zealots who naively reference a couple of open source projects that made some money. I've been there and done it, it doesn't work for 99.99% of projects.


## Answer 18784

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2011-01-10
- score: 3

By releasing your code to the public (code that you have paid good money to design, develop and debug) you are saving your competition time and money to get to the market.  There has to be a very good reason to do that.  Prior to going that route be sure you are leaving yourself some competitive advantage.  Some examples where releasing code makes sense:

* Your product is a loss-leader and you are looking to drive traffic to your site to buy another (possibly vertically-integrated) product.

* If your product has an API, releasing the library as open source will make integration easier for your customers.  

* Releasing cryptographic algorithms to the public is security industry standard for instilling confidence in your product (because those components become more secure through peer review).

* If you are selling a server-side service, you can consider making the client open-source so that contributions by the developer community can drive demands for the service.




## Answer 18797

- posted by: [Giles Thomas](https://stackexchange.com/users/-1/1547-giles-thomas) on 2011-01-11
- score: 2

<p>As Oleg says, you lose something by going open source, so you have to be very clear on the reasons.  As David says, there have been very few companies that have made serious money by open-sourcing everything.  However, you have the option of open-sourcing some of your software but not all of it.  Some examples:</p>

<ul>
<li><p>Like Oleg says, a security company might publish the crypto algorithm but not the rest of their software -- that is, the key management, user interface, and so on.  Even better, given how hard crypto is to code correctly, they might open-source a slow version and keep private the optimised version.  </p></li>
<li><p>At my company, our main product (<a href="http://www.resolversystems.com/products/resolver-one/" rel="nofollow">Resolver One, an IronPython spreadsheet</a>) is closed-source, but we open-sourced a library that we created for it (<a href="http://www.resolversystems.com/products/ironclad/" rel="nofollow">Ironclad</a>, which lets you call normal Python libraries from IronPython) so that we could get contributions from other people and more rapidly gain coverage of the complete Python standard library.</p></li>
<li><p>One software consultancy of my acquaintance created and maintains a fairly well-known piece of open source software, a set of very useful utilities for a particular kind of processing.  They then have their own proprietary wrapper around these libraries that is even better than the open source version, and they use the proprietary versions when working with their clients.  The fact that they are the experts in the OS version is good marketing, and the wrappers make them faster to code stuff than their competition.</p></li>
</ul>

<p>I guess the summary is: listen to Oleg and only open-source stuff if you have a clear idea of what you're aiming to achieve by doing so, and then make sure you open-source specifically only those parts of your application that you want to open-source.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
