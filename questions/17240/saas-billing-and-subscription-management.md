## SaaS: Billing and Subscription Management

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2010-11-30
- tagged: `billing`
- score: 2

What are some cost effective solutions that can provide secure billing/membership management for a SaaS with varying subscription options ? I am looking for something like aMember, but I think it's quite expensive.

I really would not like to store any type of CC data, and prefer to use the backend system of the payment processor.

In addition, what is your choice for credit card processing ? In the past, Paypal payments were easily reversed due to chargebacks, etc. Should Paypal still be accepted ? Anyone use AlertPay (I heard that they call to verify orders) ?




## Answer 17243

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-11-30
- score: 4

AlertPay = Great for adult sites.
Paypal = Great for small sites where you dont have more than 3k in transactions.

Real Merchant Account with your choice of gateway, is your best bet.
If you use the Authorize.net Gateway, you can tokenize your transactions, thus not having to store credit card data.

You can also use a service like CheddarGetter to manage the transaction workload, but there are fees involved.  I find its best to build your own solution.

Another Plus on having your own merchant account is that you can eventually (with a good track record, and decent sales) apply for interchange plus pricing, where you pay a flat fee above what Visa & MC charge.  This will save you a TON of money that can be better spent on advertising if your sales are 50k + per month.




## Answer 18677

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-07
- score: 0

www.Metanga.com is a subsidiary or MetraTech.com which does the billing for Microsoft Azure and BPOS. We offer a reasonably priced SaaS billing solution that can scale to the enterprise level. We can work with any merchant provider you might have, include an online catalog, offer CRM functionality, and provide a customer self-service portal for reviewing bills. Check us out and download a data sheet.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
