## Passing a payment from buyer to seller, and taking a transaction fee?

- posted by: [J.V.](https://stackexchange.com/users/-1/22398-j-v) on 2013-01-04
- tagged: `ecommerce`, `payment-gateway`
- score: 0

I'm mulling over a business idea, and the part of it that I can't wrap my brain around is the payment processing part of it.  Here's a simple example, not really my idea, but an easier example:

I have a consignment shop site, where people post items, and other people buy them.  As the site's owner, I'd like a cut of each sale, and want to take 2% of the sale price as a transaction fee.

How would I go about doing that?  The only way I know is using something like PayPal, having the original payment go to me, and then I pay the seller (minus my fee), but that seems like it would rack up a lot of PayPal transaction fees.

Can someone clue me in on a better way to do this?  It seems like a pretty standard business model.  Thanks!


## Answer 45458

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-01-04
- score: 0

<p>What you are looking for is a marketplace solution.  In your example, Paypal would only be able to receive the payment - establishing the connection between the seller and buyer would be on your side - and (depending on location) there are fiduciary responsibilities associated with holding and transferring that money (PCI, etc.)</p>

<p>Depending on the scope of your project, you can consider <a href="https://payments.amazon.com/sdui/sdui/business?sn=devfps/marketplace" rel="nofollow">amazon FPS marketplace</a>, <a href="https://www.balancedpayments.com/" rel="nofollow">balancedpayments</a> or <a href="http://www.bancbox.com/how-it-works" rel="nofollow">bancbox</a>.  There are others. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
