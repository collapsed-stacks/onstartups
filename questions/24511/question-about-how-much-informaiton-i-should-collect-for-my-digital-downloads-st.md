## Question about how much informaiton I should collect for my digital downloads store. Paypal is the only payment gateway!

- posted by: [Andy Carlson](https://stackexchange.com/users/-1/10270-andy-carlson) on 2011-05-06
- tagged: `payments`, `ecommerce`
- score: 2

Paypal is the only payment gateway!
so, my current system only collects seller's PayPal email addressed and create buttons based on that email address. 
since its all digital downloads, there will be no shipping or anything.
Should I still collect their names and mailing addresses?


## Answer 24513

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-05-06
- score: 1

The exact nature of what you need will depend on your country/state etc, also on what you are selling. 

First thing to realise while most users do use their email address for PayPal purchases a PayPal userId does not always have to be an email address. So you may wish if you ever want to communicate with your purchaser you will find it handy to have their real email. 

Given that you are collecting some information, knowing who your customers are is always helpful especially if you plan on contacting them, therefore collecting their name or company name (though you can often get this direct from PayPal via the IPN response) will help with your marketing and support. Simply being able to answer a support query with hi fred, can often disarm a situation.

Selling on the web, means selling to the entire world and this opens up a whole heap of tax issues especially as you grow, so from right at the start it's worth knowing where your customers are and as you grow whos charged what sales tax etc. If you don't have this data from the start putting it in later is going to be a fudge.

Here is what we consider a minimum amount of data collection

- first name
- last name
- email
- Country
- Post/ZipCode

With a post code or Zip Code the state/region/city can be worked out if needs be.

When building payment flows, it's important not to add to many obstacles for the client but equally important not to put to many obstacles in for you. At minimum you should be able to:

- Uniquely identify a customer/transaction
- Be able to contact the customer through a mechanism other then paypal
- Know where your customers are based

Digital product protection through PayPal is very much in the buyers favour so from a support angle alone it's worth being in a position to assist users and in this case knowledge is power. Of course with the same information, you can fine tune your site and product offerings, lots of visits from france how about offering a page in French for example. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
