## How do sellers get paid online?

- posted by: [Shawn Mclean](https://stackexchange.com/users/-1/4854-shawn-mclean) on 2011-09-15
- tagged: `payments`, `merchant-account`
- score: 1

If I'm setting up a system where people can sell stuff online. I'm planning on having my own merchant account and setting up my own payment system.

The problem I ran into is how to I send money from my merchant account to others. The only thing I have used so far is paypal to receive money, what other ways are there to receive money online? Can people use their local bank accounts? Savings accounts? Should I worry that my merchant gateway API wont support certain banks? Am I going to need to store my user's bank account information?


## Answer 30152

- posted by: [xpda](https://stackexchange.com/users/-1/13101-xpda) on 2011-09-16
- score: 1

There are three ways you might want to consider, and possibly use them all.

- Paypal and similar systems

- Credit Cards -- you can transfer money both into and out of credit and debit card accounts. Paypal can handle this if you have trouble setting up your own credit card accounts.

- Direct Bank Transfers -- transfer money into or out of someone's bank account, similar to a direct deposit or a monthly payment.

If you use Paypal only, you won't need to store the customer's financial info. This releases you from a lot of security worries and liability. You can also avoid storing the customer data by making them re-enter it every time, but this goes against the philosophy of satisfying the customer.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
