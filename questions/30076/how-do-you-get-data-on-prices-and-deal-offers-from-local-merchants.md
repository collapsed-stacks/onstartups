## How do you get data on prices and deal offers from local merchants?

- posted by: [web2jeet](https://stackexchange.com/users/-1/13186-web2jeet) on 2011-09-14
- tagged: `entrepreneurs`, `recommendations`, `market-research`, `research`
- score: 0

What the best way and economical to get updates about the prices and offers from local dealers?

I want to cover 58 areas local dealers/retailers from my city. 


## Answer 30136

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-09-15
- score: 1

Ok, I think I understand what you are looking to do.  The situation is that you have a bunch of businesses in your area and you want to bring all their pricing data together in one place to be analyzed or displayed.

So the first big hurdle is collecting that data. 

Options for collecting the pricing data on their products:

 - Visit each retailer convince them to let you export the data from their point of sale system which has all their pricing on some regular basis.  (Not really practical, and I doubt anyone would agree to this)
 - Build a web page or Google doc that every business goes to once a month and keys in all their products and information for you to have it.  (Doubt they could be convinced to spend the time)
 - You or an employee visit each location with a mobile phone, laptop look at all the data and key it into a spreadsheet (Probably the most realistic, but most work for you)

A web app to collect this data could be written quickly with Ruby on Rails, and hosted freely on heroku.com.  Or you could try to use Google docs / forms / spreadsheets to do it.

But overall this is a difficult problem to solve, and no one has found a good way to solve it.  Startups / websites that want to have the price of groceries at all the locations so you can buy products at the cheapest places still do this by manually sending someone into the store to log it.  

Website that do gas pricing at all the gas stations around the city have crowd sourced it and allow people to submit prices in via a mobile device.  If you could some how get your audience for this data excited about entering it, or turn it into a game then you might have better luck collecting it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
