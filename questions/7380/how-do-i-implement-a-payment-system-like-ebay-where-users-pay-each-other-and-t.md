## How do I implement a payment system like ebay (where users pay each other) and the site takes a cut?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-31
- tagged: `payments`
- score: 2

Is paypal the only way to do it? Would the best way be to take the payment from the payer, take a cut, and then give money to the payee? Seems like I'd lose a lot in the two paypal payments


## Answer 7400

- posted by: [Bob Walsh](https://stackexchange.com/users/-1/346-bob-walsh) on 2010-01-31
- score: 3

Check into Amazon Payments. They have an API, flexible payments, specifically designed so you can create a marketplace where A sells x to B for a dollar, and you get 10% (10 cents)

Only catch - have to have a US bank account at this point.


## Answer 7404

- posted by: [Olivier Lalonde](https://stackexchange.com/users/-1/1030-olivier-lalonde) on 2010-01-31
- score: 1

<p>You should apply directly for a <a href="http://en.wikipedia.org/wiki/Merchant%5Faccount" rel="nofollow">merchant account</a> instead of going through a 3rd party processor like Paypal. There is a great article on the subject on Sitepoint: <a href="http://sitepoint.com/article/merchant-account-review" rel="nofollow">http://sitepoint.com/article/merchant-account-review</a>.</p>



## Answer 7388

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2010-01-31
- score: 0

If you're planning on using Paypal for the actual processing, then it would fairly pointless to create your system - why wouldn't sites just use Paypal directly, and save themselves the cost of using your system. 

If you're planning on replacing Paypal with an alternate system, then you have to look at working with various payment portals for accepting various forms of payment, becoming PCI-compliant for storing customer data, figuring out a way to differentiate yourself from Paypal (or any of the dozens of alternatives already out there).


## Answer 36319

- posted by: [Anagio](https://stackexchange.com/users/-1/14857-anagio) on 2012-02-17
- score: 0

CS-Cart vendor edition lets you create a market place which lets users signup sell their goods and you get a percentage



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
