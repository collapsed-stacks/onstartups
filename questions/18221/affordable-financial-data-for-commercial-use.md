## Affordable financial data for commercial use

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-26
- tagged: `business`, `finance`, `data`
- score: 1

Does anyone know where we can get affordable financial data? eg: ticker symbols, realtime quotes...

I know we could probably mine Yahoo Finance, but the data needs to be licensed for commercial use.


## Answer 18227

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-12-27
- score: 1

I am not sure what you mean by "licensing" the data.  Typically a vendor is "fee liable" if they pass it on to other users.  If you know you only need it from one exchange you may just want to write to the exchange's API/feed.  

Not sure what is suitable for you, but have a look at these:

 - http://googleblog.blogspot.com/2007/01/real-time-quotes-for-free.html
 - http://stackoverflow.com/questions/1975085/getting-real-time-market-stock-quotes-in-c-java
 - http://www.iqfeed.net/

You are going to have to do a bit more work than just ask a question on a startup website.  



## Answer 18232

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-12-27
- score: 0

<p>"displayed on our website" IS distribution, and it cost "arm and a leg": </p>

<ul>
<li><a href="http://www.dukascopy.com/swiss/english/data_feed/webproducts/" rel="nofollow">http://www.dukascopy.com/swiss/english/data_feed/webproducts/</a></li>
</ul>



## Answer 18229

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-12-27
- score: -1

Depends what you need. Yahoo is neither licensed nor real time.

What symbols are we talking about? WHAT COMMERCIAL USE? Inhzouse or distribution? For distribution you will pay. Getting hte data is not th expensive part - getting the distribution real time rights is (BATS is IIRC 5000 USD monthly - and that is one US stock exchange network alone, CME,CBOT etc. dont seem to have any realtime redistributin rights, you need to register every recipient and pay).

Fhr number of symbols is another factor. Most networks / systems dontscale. I moved my data feeds for my interesting exchanged (pretty much GLOBEX, so I now get CME, CBOT, NYMEX and COMEX) over to Nanex 2st of December and got a good deal there (a little short to 1000 USD monthly, including my exchange feeds). Sounds expensive but these are complete feeds - not symbols, but every symbol trading on the exchanges. And they have a decent system for handling outages (I.e. automatically download missed data, maintain a library of historical tapes etc.).

It wont get a lot cheaper if you want "complete feeds" and again, redistribution / commercial use has higher costs 8like I pay around 280 USD alone in exchange fees, and these are non-professional. Get professional it jumps, get redistribution it jumps a LOT.


## Answer 18230

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2010-12-27
- score: -1

All the free data & tickers you could probably ask for are here: http://eoddata.com/

"Download FREE end of day stock market quotes and historical data for many of the world's top stock exchanges."



Also, although it may not be exactly what you are looking for, SEC Edgar data may be very useful since it is updated daily and free for anyone to use. At least it's a start. And a big one to boot.

http://www.sec.gov/edgar.shtml



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
