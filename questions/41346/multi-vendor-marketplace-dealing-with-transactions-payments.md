## Multi-vendor marketplace-Dealing with transactions & Payments

- posted by: [DougC](https://stackexchange.com/users/-1/19242-dougc) on 2012-08-14
- tagged: `payments`, `ecommerce`, `credit-cards`, `payment-gateway`, `marketplace`
- score: 1

I'm a few weeks into developing a multi-vendor, business to business website. Here is my issue: 

We could potentially have a single user purchasing from multiple sellers at one time.  

We are looking for a solution to hosting that transaction, and so far have only come up with paypal.  While this is an option, there are some limitations, obscure fees etc... that make it rather unattractive for us and our potential user base.  We simply take a transaction fee so the bulk of the sale price is our user's money.  

**Does anyone have recommendations on handling transactions for a marketplace site like this?**

Any help would be *seriously appreciated*!



## Answer 41356

- posted by: [JeffS](https://stackexchange.com/users/-1/15873-jeffs) on 2012-08-15
- score: 1

You could

1. Charge everything to your own merchant account, and forward most of the money to the vendors yourself (you can use ACH or similar to handle this). So long as your vendors trust you, this would work well

2. Connect every single vendor's merchant account to your own gateway, or force them all to get separate merchant accounts with your gateway. Then whenever a user places an order, you bill them all separately on behalf of each vendor. The Vendor then owes you fees. Samurai by FeeFighters and BrainTree are both gateways that would make this relatively simple.

3. Use an adaptive payments like solution. Paypal has the most well known one of these.

4. Abandon using credit cards altogether. Dwolla, or even handling this yourself, with ACH payments are both options.




## Answer 45000

- posted by: [kleine2](https://stackexchange.com/users/-1/13626-kleine2) on 2012-12-13
- score: 1

<p>In the past when I researched this I found this:
<a href="https://payments.amazon.com/sdui/sdui/helpTab/Amazon-Simple-Pay/Integrating-with-Amazon-Simple-Pay/Amazon-Simple-Pay-Marketplace" rel="nofollow">Amazon Simple Pay</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
