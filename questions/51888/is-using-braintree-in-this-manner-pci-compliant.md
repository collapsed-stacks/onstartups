## Is using BrainTree in this manner PCI-compliant?

- posted by: [Nathan Osman](https://stackexchange.com/users/-1/25951-nathan-osman) on 2013-11-26
- tagged: `payments`
- score: 0

<p>According to the instructions on <a href="https://www.braintreepayments.com/developers" rel="nofollow">BrainTree's website</a>, in order to integrate their payment solution with my Python application, all I need to do is:</p>

<ol>
<li>Sign Up</li>
<li>Server Side Integration</li>
<li>Client Side Encryption</li>
</ol>

<p>I noticed that step 3 contains the following snippet of text:</p>

<blockquote>
  <p>PCI compliance will be a breeze.</p>
</blockquote>

<p>Does this mean that using BrainTree in this way <em>is</em> PCI-compliant or that I am still under some sort of obligation or restriction? (I'm not terribly familiar with PCI-compliance, I'm afraid.)</p>



## Answer 51989

- posted by: [Ivan Plenty](https://stackexchange.com/users/-1/29891-ivan-plenty) on 2013-12-03
- score: 1

<p>I've worked in IT security for a while.  If you use BrainTree with server integration, you still will have to get a separate PCI compliance audit for your site, but relative to other PCI audits yours would "be a breeze" (i.e. easy).  You likely will just have to fill out the self-service questionnaire, pay the fee, and wait 2 weeks for someone to rubber-stamp your approval.  You then will have to do this every 1 - 3 years, depending on a lot of factors.</p>

<p>The reason why you have to submit the paperwork is that the customer's credit card data is going through your servers.  BrainTree is guaranteeing that the credit card data is encrypted, which is why the audit process is a 'breeze,' but PCI scopes in any server that touches the card data.  There are rules where some data can never be stored, some has to be encrypted, and some only should be encrypted.</p>

<p>If you want to avoid the PCI audit business altogether, pick a payment provider where none of the cardholder data ever touches your server.  Some good options include going to a hosted payment gateway page or using 100% JavaScript (e.g. stripe.js).</p>



## Answer 51895

- posted by: [Liam Dolman](https://stackexchange.com/users/-1/27824-liam-dolman) on 2013-11-26
- score: 0

<p>I think your question would be better answered at <a href="http://webapps.stackexchange.com/">http://webapps.stackexchange.com/</a> or <a href="http://serverfault.com/">http://serverfault.com/</a> where the users will be more familiar with your issue.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
