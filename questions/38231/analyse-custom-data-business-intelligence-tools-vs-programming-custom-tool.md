## Analyse custom data: Business Intelligence Tools vs Programming Custom Tool

- posted by: [Luksurious](https://stackexchange.com/users/-1/17522-luksurious) on 2012-04-16
- tagged: `data`, `business-intelligence`, `analysis`
- score: 0

I wanted to know what you would recommend for analyzing data in this scenario:

We have a web application that requires users to register etc in order to use it. For our further decisions on what to do next and also for potential investors analyzing our users is important. Metrics like 

 - How many users registered on a certain date, progression charted with selectable timerange
 - How many users have registered up to a certain date
 - or more complex: given certain user categorization, how high is the rate of returning users for each group
 - etc.

So far we have used a custom tool that is directly querying the database and presenting selected data in charts using the Google Charts Tools.

But this is rather bad at the moment, because our development team is currently the limiting factor and would like to have the business guys do the analysis themselves because it can get fairly complex which in turn would require quite some programming effort.

I have found certain Business Intelligence software like Pentaho and JasperReports but they seem extremely complicated to setup and use and feels like total overkill. We have also thought about using MS Access since they also have nice reporting features.

So my questions are:

 1. Is there any good standard software that enable our non-programmers to get the data analysis they want?
 2. If so, would you recommend for a startup that has limited time and resources to dig into a specific tool and learn how to use it? Or is a custom tool the best shot?

Thank you very much for your help,

Lukas


## Answer 38234

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2012-04-16
- score: 1

The newer version of Excel should be able to handle your data set and probably has more capability than you will ever use. Since the business people are not editing and storing relational data.

Your programmers could be involved in getting the data out of your system in a form that a business person can work with. They don't have to worry about providing every filer, search, group and sort scenario. Business people should be able to create complex formulas. 

I think they will prefer this over Access. Access can make it easier to generate reports in an attractive format as the data set changes (Excel needs additional coding to make sure those formulas get applied to the new rows.). You may migrate an Excel report to Access once you solidify the format and want to run it every month/quarter with a click of a button. Excel is better if the report always needs to be adjusted every time you run it.


## Answer 38233

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2012-04-16
- score: 0

<p>If you're in PC land, Excel is a great tool that lets you work fast and range over data and relationships, whether in the spreadsheet or with database connections. If the latter doesn't work for you, putting an intermediate database up to sit between the live system and your desktop is good. In Mac world, I like Numbers well enough, but it doesn't have anything like the depth in this area.</p>

<p>If you are looking for deep patterns buried away in the data, then really you're in the realm traditionally dominated by SAS and SPSS, but <a href="http://www.r-project.org/" rel="nofollow">the R language</a> is truly awesome with lots of open source libraries. </p>

<p>However, the kind of use cases you describe are pretty straightforward, so I'd start with a spreadsheet, and either stay there or use it to prototype reports and charts in your tool of choice.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
