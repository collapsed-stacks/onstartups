## How to write a program for Forex market?

- posted by: [Isaac](https://stackexchange.com/users/-1/9867-isaac) on 2011-04-21
- tagged: `market`, `program`, `stock-exchange`, `trade`
- score: 1

My boss has a jewelry workshop and because of his job he must keep a large money in his account (as some kind of insurance and guarranty for other companies). Recently he heard of trading using softwares and decided to do something with that money. He asked me (as the programmer) to write an Expert Advisor in [Metatrader][1] software that buy and sell gold automatically on Forex exchange market to make some profit.

First of all, I don't know where to start. I read Metatrader API and write some codes which buys and sells on a Demo acoount. But I guess programming knowledge is not enough. Should I read some financial books? How about some statistical knowledge?

Second, it is clear that there is no promised and perfect strategy for making profit (even small) in the exchange market, because the profit of one guy comes from loss of another guys. No matter what strategy you use, some day you will be bad luck guy. 

I seems there is a trade-off between taking the risk and making profit/loss in the exchange market. I hope I would find some strategy that makes a small profit with low risk. 

Just like putting money in the bank that gives you small profit with no-risk, there should be a stategy in the exchange market which gives you a little more profit with a low level of risk.

Do you know any low-risk small-profit strategy for trading in Forex?


  [1]: http://www.metaquotes.net



## Answer 23776

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2011-04-21
- score: 10

Having worked in the field for a couple of years, I can tell you: Algorithmic trading is complex and sometimes unpredictable, prone to gaming by other parties out there on the electronic battlefield and if you don't know what you're doing, you **WILL LOSE MONEY** and your boss will probably not like it. 

The buy/sell API is as easy as picking up the phone and screaming "buy/sell" at your broker. Knowing when to do that and by how much... that's what separates the men from the boys as the saying goes.

I'd be very cautious if I were you. Build trading applications requires **much more than a programmer**. It requires a programmer/trader. If you're not one, you'll lose.


## Answer 23809

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-04-21
- score: 6

To be honest, the other answers here are 100% correct--if you don't know what you're doing here, and from your question it sounds like you don't, you're going to be the fool that everyone else gets rich off of. As Paul Newman said, "If you're playing a poker game and you look around the table and and can't tell who the sucker is, it's you."

But I don't want to send you away without an answer. Essentially, the answer to your question lies in a field called [Portfolio Theory](http://en.wikipedia.org/wiki/Modern_portfolio_theory). Portfolio theory is the mathematical underpinnings of the theory of the relationship between risk and rate of return. There are books about it and it is taught in universities. Most of the people who know how to do it learned it by working on Wall Street, in investment banks, or hedge funds. 

There is no trivially easy answer here ... essentially your question is the same as saying "I want to take my appendix out. It's been hurting. How can I take my appendix out?" And the best answer we can come up with is, "Find a doctor or go to medical school."


## Answer 23797

- posted by: [John MacIntyre](https://stackexchange.com/users/-1/760-john-macintyre) on 2011-04-21
- score: 5

First off, **forex is for trading currencies, not metals**.  If he wants to trade commodities like gold, you should be looking at the futures markets.

Second, **you're swimming with sharks, with laser beams**.  You're going to be up against some of the worlds brightest people who are thinking about this 24 hours a day and have been doing so for 10, 20, 30, 40 years or longer.

I'm not saying it's not possible, but I will say that it sounds like your boss has unrealistic expectations and if you chose to attempt this you've got your work cut out for you.


## Answer 40934

- posted by: [BlueTrin](https://stackexchange.com/users/-1/19008-bluetrin) on 2012-07-31
- score: 4

I am a quantitative analyst in a Tier 1 bank.

What you are asking is totally off-topic for this website. Ideally, you want to be a guru in statistics, econometrics and having trading experience. To be honest, programming is the least important parameter in this venture.

I am not saying you cannot succeed without these skills but many people are under the illusion of being successful while they are trading noise. 

It is very hard to have a real edge against the market and even if you have one to quantify it statistically correctly.

If you still want to pursue your quest,  you should learn how to backtest properly your strategy (meaning measure on historical data what would have been the profit), do some forward testing and then implement it. I know a few people involved in this kind of work in funds and it is not uncommon for them to forward test a strategy for 1 year before to even think about going live. Do not forget to include the cost of capital and learn how to size your positions using sound money management.

Do not forget to compute your edge statistically using a large number of trades. Many people think they have an edge and just got lucky ...



## Answer 23842

- posted by: [umps](https://stackexchange.com/users/-1/9907-umps) on 2011-04-22
- score: 2

First of all, your question is not "How to write a program for forex market". That can be done easily. The question is "How do I predict the movement of gold prices accurately enough so that I can profit from it".  

Second of all, If anyone knew a low risk small profit strategy, they wouldn't tell you for free. 




## Answer 40930

- posted by: [kenorb](https://stackexchange.com/users/-1/19007-kenorb) on 2012-07-31
- score: 2

You have to learn The Metaweb Query Language (MQL4 OR MQL5). But it takes years and lots of time to write your own bot and actually to get some real profits. It's easier to trade manually, human can see more patterns and read the news than the bots (which can't predict economical changes) or use some existing strategies which were already tested for couple of years on the REAL accounts.

The are existing bots on the market, thousands of them, so start from there.

First of all download MetaTrader4, then download all Expert Advisor you can find on the internet and play with them. Learn how to do strategy backtesting, change some variables and learn how it works based on the code. Basically you need experts with MQ4 extension which contains the source, if you get EX4, then it is encoded (with possibility to decode).

Some advises:

 - before you start writing the bots, there are some websites which are doing auto-trading, like ZuluTrade (recommended), Currensee, you can start from there (see how and when they trade),
 - NEVER use strategies with the big DD (they say 100% win, you'll get 100% lose),
 - don't invest your whole money at the first time,
 - DO NOT trust anybody (even me), on the internet there are SCAMS EVERYWHERE, they promises you million - THEY LIE, don't pay for the strategies where most of them are free (spend some time to read some reviews online about it, it doesn't cost),
 - DON'T LISTEN to anybody, people who are giving some advises, mostly they are losers (they just raise the value of them-self), people who're winning - they DON'T CARE about anybody and they don't share their strategies and success (they don't want to risk their money),
 - if someone wants to share their knowledge or sell their bots, there is ALWAYS a catch (why they don't keep it for them-self?),
 - if you play at the first time, be ready to lose your money and learn on your own mistakes,
 - if you play on the 2nd, 3rd, 4th time, be more careful each time and prepare to lose your money again,
 - if you survived for 2 months (even the balance stayed the same), then you're already good,
 - use micro accounts,
 - observe the market and learn (never trust the bots) e.g. <a href="http://www.fxstreet.com/rates-charts/live-charts/">FX Street Chart</a>,
 - never increase your lots, if you're doing well (use auto-balancing instead),
 - use the brokers with small provisions,
 - read how the brokers can cheat you,
 - if you did everything above, then you're ready to write your own bot,



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
