## Data aggregation from hundreds of different websites into one

- posted by: [Tony Brattle](https://stackexchange.com/users/-1/14617-tony-brattle) on 2011-11-23
- tagged: `data`
- score: 0

what would the process be for aggregating data from hundreds of websites into a master database? I would then do calculations on the master data base,  then resell.

Thank you. 


## Answer 32941

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-11-23
- score: 2

 1. Get legal permission to use each web site's data
 2. Hire a team of web script writers to scrape the data from each web site
 3. Collect the data
 4. Verify data collection is correct (each time you scrape a site)
 5. Store in master data base
 6. Update scripts as needed for data collection



## Answer 32944

- posted by: [chentudou](https://stackexchange.com/users/-1/5346-chentudou) on 2011-11-24
- score: 0

It depends on the data you are getting. If it is data that the websites you are targetting readily share then it will likely be accessible through some kind of data feed that they provide. If its not readily available you may need to 'scrape' it as Gary mentions.

Once you have the data, depending on how you got it, you may need to 'map' it into your database. Basically, if you scraped it you or whoever did the scraping may have been able to get each data set from each site in the same way and so it will already be arranged in a table in the same way. If you have got it from a feed, a .csv or .xml file for example you may need to write a script to 'map' each data column to fit the arrangement of your database.

Specific methods would depend on what type of data you're getting. What kind of database you want to use and what processes you would like to do with the data. In my experience I have used PHP to get xml, csv, txt feeds, and aggregate them into MySQL databases but have not done much 'scraping'.




## Answer 36291

- posted by: [Patrick](https://stackexchange.com/users/-1/15596-patrick) on 2012-02-17
- score: 0

Have a look at scraperwiki.com - It is the Mekanikal Turk for Scraping websites.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
