## Redirect user for payment or let them stay on your site?

- posted by: [user3462](https://stackexchange.com/users/-1/3462-user3462) on 2011-02-21
- tagged: `payments`
- score: 3

I am using Paypal subscription for charging the customers monthly. When they sign up, I have an option of either redirecting them to the Paypal site to enter the credit card details or gather this information on my site. I am not sure which one to use for development.

Pros of redirecting user to Paypal

 - Users trust paypal

Cons of redirecting user to Paypal

 - Choppy user experience. They are
   redirected back and forth.

Pros of gathering credit card information on site

 - Need to purchase a certificate as the
   page needs to be secure (https)

Cons of gathering credit card information on site

 - Users may not trust your site and
   would not like to provide CC info.

Did I miss anything? Any thoughts? thanks

**EDIT: Based on the response, it appears that people are torn between these two choices**


## Answer 20574

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-02-22
- score: 4

My employer did some testing of their own on different payment scenarios and surprisingly a large percentage of users 88% felt safer being redirected to Paypal / other payment gateways than they did entering their own details on a website.

The group made various comments, but all were mostly along the lines of, "I use Paypal when buying on eBay" and "Paypal has payment protection" and "My card details aren't shared with a potentially bad website."

Stick with the redirection, more people trust it than most know.


## Answer 20561

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-02-21
- score: 1

**Pros of redirecting to PayPal**

 1. None


**Cons of redirecting to PayPal**

 2. User is redirected from the place they were trying to buy something from. This sets off red flags in many user's minds
 3. The site the user is redirected to doesn't match the design of your site, another red flag
 4. You don't control the information collected from the customer
 5. Many people don't trust PayPal. (Many do- but the negative and the positive balance out **unless** you are selling to businesses- and here the negatives outweigh the positives.)
 6. Delivery- how is it made once PayPal completes the sale?
 7. You can't even pull a graphic image from your own web site to show on PayPal- unless you have an SSL certificate- otherwise you get security warnings.

**Pros of using your own SSL certificate**

 1. User remains on your site
 2. Your order page **matches** the rest of your web site
 3. You control exactly what information is collected
 4. Your SSL certificate should inspire all the trust you need to complete the sale
 5. Once a sale is complete- your web site delivers the product

**Cons of using your own SSL certificate**

 1. It costs $50 or so a year
 2. Your web host has to be able to support SSL





## Answer 20665

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-02-23
- score: 0

Storing credit Cards is not just a case of "owning" an SSL certificate that is the least of your issues. You are holding peoples Financial Credentials if your site is compromised you might be financially liable for any damages but your reputation would certainly be in taters.

Most Merchant Gateways and Banks and probably more importantly insurance companies expect you to be "compliant" with PCI-DSS this is a standard with levels 1-4 based on transaction amount and volume which is expected to be adhered to at the basic level it's a load of paper work as well as a requirement to have a "secure network" that's not just an SSL certificate and unless you are running in suitable hosting something you will be unlikely to achieve. 

Practically none of this is hard if you have a good infrastructure and system admin who know what they are doing but before even pondering going down this route you need to understand their is a risk and cost associated with Direct Card Processing.

Often when you look at the actual costs of direct card processing via a merchant gateway along side the PCI-DSS work/paperwork/scans and yes the shiny SSL certificate not to mention the indemnity insurance suddenly the loss of the occasional person doesn't always seem to be so bad.

I'm not trying to scare you and if you are a mid sized business with a relatively health turnover (or expect to be) then looking at non hosted solutions may be a wise idea, and many merchant gateways offer PayPal as well as part of their offerings, PayPal also offer a range of offerings other then their standard and Pro services (you may wish to Look at PreApprovals via the Adaptive Payments API)









---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
