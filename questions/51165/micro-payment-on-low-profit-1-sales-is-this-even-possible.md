## Micro-payment on low profit $1 sales, is this even possible?

- posted by: [m-y](https://stackexchange.com/users/-1/28069-m-y) on 2013-09-28
- tagged: `ecommerce`, `startup-costs`, `credit-cards`, `micro-payment`
- score: 4

<p>I'm a software developer working on an application, so forgive me if this question does not contain the proper terminology...</p>

<p>I'm trying to figure out if what I want to do is even possible to do. I'm looking at creating an eCommerce application that can sell a good for $1.00 USD. The product will only be available within the US, so I'm not worried about international rates.</p>

<p>I'm not 100% sure, but my guess is that my profit will be around 5c per transaction, maybe 4c depending on volume of sales. The part that worries me is I can't seem to find any information online about micropayments of credit cards that would allow this business model to succeed. I'm not sure if I can't find this information because it isn't possible, or because I don't know what to look for.</p>

<p>Everything I find states that I'd be looking at around 5% plus 5c at best for micro transactions... that's 10c per dollar when my profit is 4-5c per dollar. I've also seen some with a lower percentage, but a higher per transaction fee (i.e. 3% plus 25c). Then there is services such as square, which are a flat percentage, but they require physical access to the card.</p>

<p>I realize that if I require that consumers purchase in bulk ($10+) that it would help me out possibly, but I moreover want to know if it's possible to just stick with the $1 sales.</p>

<hr>

<p>Please no comments that I need to increase my profit margin. I simply cannot. Thanks!</p>



## Answer 51232

- posted by: [rbwhitaker](https://stackexchange.com/users/-1/15024-rbwhitaker) on 2013-10-02
- score: 4

<pre><code>Please no comments that I need to increase my profit margin. I simply cannot.
</code></pre>

<p>I know you specifically said not to bring this up, but I think your margin <em>needs</em> to be discussed. <strong>The way I see it, your margin is your first hurdle, and your first big limiting factor, not the payment processor.</strong></p>

<p>I hope you'll forgive me for bringing this up even though you asked that we not, in an attempt to answer your underlying question of whether this is even possible.</p>

<p><strong>You're talking a 4-5% margin. At those levels, it will be nearly impossible to stay afloat.</strong> Running a little math here, let's say you found an ideal payment processor that would do it completely free. 5 cents on every dollar means you need 1 million transactions to make $50,000. </p>

<p>I don't know where you live at, but let's say you're a sole developer in the USA (or an equivalent cost of living). After taxes and business overhead, that leaves you with something like $30,000. I can't imagine any competent software developer that would be willing to work for anything less than that. Most want double or quadruple that. (If you live elsewhere, where the cost of living is less, you can adjust these figures.) </p>

<p>The bottom line is, <strong>you have to ask yourself, "How realistic is it that I'll get at least 1 million transactions per year?"</strong> Only you know your business idea well enough to answer that, but it is a question that has to be asked and then answered honestly.</p>

<p>And of course, that's in an ideal scenario. Reality will likely make the picture worse. Potentially much worse. For starters, if there are two or three of you, you'll need two or three million transactions instead. And of course, a real payment processor won't do this for free. They'll always take a cut of some sort.</p>

<p><strong>Even if you can lump together lots of payments, you'll still be making significantly less profit than I described.</strong> To illustrate, let's say you go with 25 cents + 3%, but can lump together 20 payments into a $20 purchase. Before the payment processor, you have $1 profit. The payment processor, though, will take 85 cents of that. Your share is 15 cents. <em>15 cents on a $20 payment!</em> Your customers will need to sink a grand total of 6.67 million dollars into this for you to get your $50,000 paycheck!</p>

<p><strong>My point here is that I think you <em>have</em> to change your margins - increase what you charge or decrease the cost of acquiring goods - or you need to find an alternative business model, or find a different idea to work on.</strong></p>

<p>The reality is, <strong>the people who do microtransactions like this <em>always</em> have much higher margins</strong> than you're allowing yourself. They're usually selling digital goods, which can be replicated essentially for free. They just have to turn around and pay the producers (musicians, programmers, whatever).</p>



## Answer 51198

- posted by: [Kamal Hassan](https://stackexchange.com/users/-1/27332-kamal-hassan) on 2013-09-30
- score: 2

<p>If these are one-off transactions, I can't see a solution.</p>

<p>If these are repeated transactions, then you can just keep aggregating people's credits or debits until you get enough to be worth charging. Start by getting people to put, e.g., $20 on deposit to take part in the marketplace. Their deposit is their guarantee of payment, so you don't need to take a credit card to guarantee each individual transaction. They pay with 'Greg credits' instead of VISA. Of course, you need people to trust you with their float.</p>

<p>You were a little bit unclear on exactly who owned the marketplace. I hope this helps!</p>



## Answer 51172

- posted by: [Peter Stratton](https://stackexchange.com/users/-1/23696-peter-stratton) on 2013-09-28
- score: 0

<p>Stripe and WePay both charge 30 cents + 2.9% for any successful transaction.  I use Stripe and the smallest transaction size you are allowed to offer is 50 cents.  Not sure about WePay, but they are probably comparable.  I'm not up to speed on the other payment processors out there, since using Stripe is just so painless.  Hope that helps.</p>



## Answer 51231

- posted by: [David Silva Smith](https://stackexchange.com/users/-1/6292-david-silva-smith) on 2013-10-02
- score: 0

<p>Bitcoin has the lowest fees I know of. Two merchants that convert you to USD are <a href="https://coinbase.com/merchants" rel="nofollow">Coinbase</a> 0% and <a href="https://bitpay.com/pricing" rel="nofollow">Bitpay</a> .99%</p>

<p>Might cause issues for you since customers will need to have Bitcoin to purchase your product with.</p>



## Answer 51246

- posted by: [saurabhj](https://stackexchange.com/users/-1/17589-saurabhj) on 2013-10-04
- score: 0

<p>You can take a cue from how companies like AudioJungle charge customers.
They sell sound files - many of them as much as $1.00 (what you are charging).</p>

<p>The way they go about doing this is:</p>

<ul>
<li><p>You can make a one-off purchase from them - but they add an additional $2 to their price. So something that is $1 - they sell for $3</p></li>
<li><p>Or, you can buy a prepaid credit in packs of $10 and above - which they store in your digital wallet. If you pay using your digital wallet, you can purchase stuff for their specified price.</p></li>
</ul>

<p>This seems very fair to me. Otherwise, you will not be able to charge credit cards for customers.</p>

<p><img src="http://i.stack.imgur.com/kPAjk.png" alt="AudioJungle payment optio s"></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
