## best digital currency platform or script?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2011-08-12
- tagged: `currency`
- score: 0

I want to implement digital currency, so people can buy currency with real money and spend it on stuff on my site.

are there any sites like recurly.com but for providing digital currency function to my web app?

I found trialpay....any other alternatives?


## Answer 28737

- posted by: [Karz](https://stackexchange.com/users/-1/12637-karz) on 2011-08-13
- score: 0

Do you think that its secured? Do you think you alone can make currency. Can't users make fake currency like yours?

You have a payment gateway which is safe and risk free and you have a third party person to claim errors. But your idea is not correct. It have many many security issues.

Or you can make digital currency. I hope it will be better than what you said. Many sites uses digital currency called tokens. First users has to purchase tokens and everything in the website is counted with number of tokens.


## Answer 28797

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-08-14
- score: 0

If you use something like PayPal Pro, Authorize .Net or some major payment gateway and collect their money it will take care of doing the currency conversions for you.

So you can have the person buy X (your internet dollars) for $Y USD, but if they were in Australia or the UK and bought it the gateway/banking aspect would do the necessary conversion of currency so you still get the amount of money you wanted.

You could then give them $X (your internet dollars) to use on your site and do with what they please.

So, it's pretty simple. You could do it with PayPal, even Recurly... you just need a little custom code that one of those systems will call back to telling you how much the user bought so you could credit their account with those theoretical internet dollars.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
