## Payment Processing Migration

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-16
- tagged: `payments`, `payment-gateway`
- score: 0

I’m building a SaaS product.  My plan is to use the payment gateway (Authorize.net) & merchant account (First Data) I already have in place for other web-products to process the monthly fees. The new product would operate as part of my existing company. 

My questions are these. What happens if somewhere in the future I decide to split off the new SaaS product as a separate entity requiring new payment gateway and merchant accounts? Will this create a big problem regarding monthly fee processing for existing customers? It wouldn’t be an issue for new clients but I’m not sure how I’d handle existing clients when the payment processing is migrated. Thoughts? 



## Answer 1703

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2009-10-16
- score: 1

I've had to do this a few times.

The good news is that (theoretically) it will be completely transparent to your end users: you just change your Auth.Net API key, and you're good to go.

The bad news is that it's a complete hassle to do because you have to go through the whole process of getting a new bank account, getting merchant processor, getting a new gateway account, etc. And worse, given the current credit markets, you may have a difficult time geting the same deal as before because your the SaaS product is a completely new "person" with no credit history, etc.

This may even create a problem with your end customers (but you'd be aware of it before the switch over), depending on what your billing is: for example, your new SaaS entity may not be allowed to do monthly recurring, etc. It all depends on the current underwriting guidelines and how established your new SaaS entity will be.

For our newest card-accepting company (Inedo Media), we just decided to run everything through another company, and then do intercompany bookkeeping to make the numbers add up. At least until Inedo Media builds up credit and is in business for at least a few years. It's more of a bookkeeping hassle, but... it's not *that* bad.


## Answer 1715

- posted by: [Ade Olonoh](https://stackexchange.com/users/-1/317-ade-olonoh) on 2009-10-16
- score: 1

I had to do this before with moving from one First Data merchant account to another (using the LinkPoint API, not Authorize.Net).  The migration was a pain, but the real headache was that some banks rejected the recurring transaction as fraud once renewal came up under the new merchant account.  

It wasn't a large percentage, but enough that it was a big pain, and some customers had to call their bank to authorize the charge (rather than just updating credit card details).  I'm not sure the details on *why* those charges looked fraudulent, but I imagine there was something that pointed to the fact that the subscription had started with a different merchant account.


## Answer 1720

- posted by: [Cary](https://stackexchange.com/users/-1/937-cary) on 2009-10-17
- score: 1

Kevin,

If you spin off the SaaS entity, why not setup a contract between the new entity and the parent company so that the parent company is submitting payment requests through the existing gateway and account?

This way there is no migration or hassle with credit checks as the established company continues to process payments on behalf of the new entity using existing facilities.

When you settle the existing account you can then transfer funds from the existing bank account to the account of the new entity so that accounting reconciliation is satisfied.

[edit]

I thought of something else you might take into account.  Since you are launching a SaaS, its conceivable that your ecommerce related traffic could quickly increase and with it the requirement to increase your PCI compliance level.  If you don't want to hassle with that you should consider outsourcing the ecommerce bits to a company like Vindicia that provides just the processing and reporting processes and allows you to control the experience.



## Answer 1712

- posted by: [Val Lynn](https://stackexchange.com/users/-1/692-val-lynn) on 2009-10-16
- score: 0

Should you decide to set up another merchant account, get your own Authorize.net account first (ie, do not go through your Merchant Service provider to set this up). This way, you can change merchant service providers without having to set up a new Authorize.net account.

Also be aware of the impending "PCI-Compliance" deadline in the Summer 2010. Find out what you need to do (ie, how much you must pay in cash and time) to be compliant on a yearly basis for each merchant account you have. 

For example, Elavon is charging $175 per year for a Merchant to complete a LONG survey that "certifies" compliance. Lack of certification up to the impending deadline means a $20 per month fee.


## Answer 1816

- posted by: [pbreit](https://stackexchange.com/users/-1/239-pbreit) on 2009-10-18
- score: 0

I would contact AuthorizeNet and confirm that if you ever switch merchant account providers, you will be able to process credit card charges for all of your existing customers without them needing to provide their card information again.


## Answer 1865

- posted by: [Rick Montgomery](https://stackexchange.com/users/-1/974-rick-montgomery) on 2009-10-18
- score: 0

Your first problem is using FirstData! Get rid of them and use Merchants Choice Payment Solutions and your world will be much brighter, efficient, and less expensive.
Common misconception is that you have to go through the merchant servcies provider that your bank refers you to. WRONG!! You can use any processing company you want and bank anywhere you want. MCPS is a breeze! No hassles!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
