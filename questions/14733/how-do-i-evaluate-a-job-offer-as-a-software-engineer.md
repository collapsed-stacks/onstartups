## How do I evaluate a job offer as a software engineer?

- posted by: [Wei Hu](https://stackexchange.com/users/-1/4624-wei-hu) on 2010-10-04
- tagged: `stock-options`, `job-offer`
- score: 2

I got a job offer from a startup with about 70-80 engineers. I'm a fresh PhD. I'm getting about 0.01%. What percentage of stock options would be a fair price? They gave me a good base salary upfront, making me feel a little embarrassed to negotiate with them. I know every company is different, and the amount you get varies depending on the maturity of the company. How could I evaluate my stock options, and should I negotiate for more? How could I find out if the company is in series A, B, C, or D (honestly I don't know what that means)?


## Answer 14754

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-04
- score: 4

You can use a discounted cash flow (DCF) analysis to value the benefits you're being offered. The application of DCF to stocks is called the Gordon growth model:

$$P = D\cdot\sum_{i=1}^{\infty}\left(\frac{1+g}{1+k}\right)^{i} = D\cdot\frac{1+g}{k-g}$$

P present value of the stock
<br>D last dividend paid
<br>k discount rate
<br>g dividend growth rate

Because you're working for a start-up, they never paid a dividend. But that doesn't mean you can't use this model. It just means you must make a reasonable guess what this company's earnings will be over the next few years and substitute earnings per share for D in the above formula.

But if you've been offered stock options rather stock grants, the situation is even more complicated. The Black–Scholes formula is typically used to value European call options.

Personally, I don't place any faith in compensation options. They never panned out for me.

In 2005, Bill Gates said, "We probably never should have used stock options...I actually regret we ever used them." Source: *Gates regrets ever using stock options*, http://www.msnbc.msn.com/id/7713133/

(BTW, I second the opinion that you should cross-post this question over at programmers.stackexchange.com)


## Answer 14756

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-10-05
- score: 1

Just ask them how to get more.  Frankly as a business owner I would be happy if an employee had more incentive to make the stock value higher.  

Ask them the same question and say the same things.




## Answer 36303

- posted by: [Chet](https://stackexchange.com/users/-1/5477-chet) on 2012-02-17
- score: 1

<p>To find out what funding round a company is in I like to use <a href="http://crunchbase.com" rel="nofollow">Crunchbase.com</a>. They tend to have fairly up-to-date information on funding rounds--who the investors are, how much they invested, etc... It's not very good about giving real valuations all the time though, you'll have to guess or ask around.</p>

<p>The series are discrete stages of large amounts of funding, usually in the millions. Earlier the series (seed, series A), generally the more risk you take on and the more equity you will receive. After each funding round the investors can take a sizeable chunk, so you will either experience dilution of your shares or else if you come in late, such as a Series C, you won't receive as much equity because hopefully the company has reached more maturity and stability.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
