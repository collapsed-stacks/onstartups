## Payment systems for sites like ebay

- posted by: [Shawn Mclean](https://stackexchange.com/users/-1/4854-shawn-mclean) on 2011-09-08
- tagged: `payments`
- score: 0

I'm building an item mediator portal, something like ebay where people can sell stuff and other people buy it. What payment gateway or systems out there to use that does this? What I want to do is have the sellers connect their account to the system to receive money and the buyers just pay with credit card OR from their account. I'm also taking a percentage of the items sold.

How would I go about setting up the logistics and what 3rd party system would I be using?


## Answer 29828

- posted by: [Seth Rogers](https://stackexchange.com/users/-1/13038-seth-rogers) on 2011-09-08
- score: 1

<p>This question has been touched on several times before; a quick search on this site may help you solve your dilemma. Also, a few popular payment processors are explained in <a href="http://discuss.joelonsoftware.com/default.asp?W1341" rel="nofollow">Business of Software</a> written by Joel Spolsky including a comparison of "pure" vs. "traditional" payment processors.</p>



## Answer 32382

- posted by: [sk24iam](https://stackexchange.com/users/-1/4660-sk24iam) on 2011-11-08
- score: 1

The best way to do this would be to setup a payment processor to accept credit cards for the items being sold.  From there, you would have to program your website to create a balance for the seller which would include the amoutn of the sold item minus the fees your site deducts.  The final step would be to deposit a seller's funds to them either through ACH or paypal.  

So essentially...

Buyer pays with credit card >>>  You

You subtract seller fees

You transfer balance through ACH or Paypal >>> Seller




An example of a company you would use is cdgcommerce.com which will set you up with a merchant account and gateway such as authorize.net

Your coder would have to build all of this into the code to properly deduct your commission fees.  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
