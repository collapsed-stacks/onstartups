## Free event and action dashboard for startups - Is this is a useful idea?

- posted by: [Nilesh](https://stackexchange.com/users/-1/6985-nilesh) on 2011-02-11
- tagged: `bootstrapped`, `user-interface`
- score: 1

This post/question is little long but could be useful for startups so I decided to write it here.

  I have been using an internal dashboard to track my application events and user actions in a php based dashboard system. When I launched my dashboard software (desktop app) I had no clue what was going on with my sales. All I had was just google analytics. For e.g I wanted to know when did the user decide to purchase? Did the user who downloaded the app click on any tutorials, watch any videos, how many users who downloaded actually installed and launced the application, How many users visited the buy now page after expiration of the software trial and so on?

So out of frustration I used my own software to build metrics for tracking the user actions.

The user actions are tracked only when the user clicks on any button or menu item and the menu item is suppose to take them to my website. 

Here is one snapshot of the dashboard pages
![Action Dashboard Infocaptor][1]


  [1]: http://i.stack.imgur.com/Y0YCs.jpg

This is just one of the pages. I have other pages that show me summarized event actions such as

(Just total counts - no details)
Sales for the Month, year, quarter, week

For other events I have a page that allows me to click on the button and specify an event name. The system then automatically registers the time.

For e.g if someone requests a web demo, I go to this page and enter the event "WEB DEMO REQUEST" and "CUSTOMER NAME". So next time when the web demo is complete I enter "WEB DEMO DONE". So when the customer actuallys sends a PO or buys I would enter "PO RECEIVED" or "PURCHASE". 

So what happens over the time, the mini data-warehouse has all the action events tied together on a timeline. This gives a great insight into what is working and not.

I thought if I put this on the web for free then lot of startups and established companies can benefit too, right?

Since this is a home grown system with lot of tweaks, I would have to spend atleast couple of weeks to put it in usable format for general use. The system would have pre-built reports and dashboards enough to get started.

My questions 

 - Is this a useful idea and is it worth putting my time to make it public?
 - Since it is going to be free, should I put any limits on the number of events as someone could just abuse the system and flood the database.




## Answer 20115

- posted by: [Ryan Elkins - IActionable](https://stackexchange.com/users/-1/2566-ryan-elkins-iactionable) on 2011-02-11
- score: 2

First off, my startup does something somewhat similar. In addition to providing dashboards and analytics around what people do we primarily use that data to give site users points, badges, etc. to motivate engagement. The basic framework revolves around recording activity, though. A company called Mixpanel does almost exactly what you are talking about. I don't say that to discourage you, but to let you know where I am coming from on this. It's definitely something people like, would use, and are willing to pay for.

So, coming to the free part - you should definitely put a limit on it if you want to make it free. You could easily find someone putting millions of actions per day through the system - not as abuse, just as their normal level of activity. You could find yourself quickly struggling to support the scale this thing could grow to. Depending on how you wrote your application you could also quickly find that the basic architecture doesn't work. When you start getting a million events an hour, SQL queries start to really slow down if your DB strategy didn't account for 100s of millions or billions of rows.

So, to sum up, it's a good idea but think of the costs to you to run this and really think about why you would want to make it free. My advice would be to either turn it into a business (with perhaps a free plan for small startups) or plan to release it as an open source project that people can run on their own hardware, so it's free but you're not paying the server costs to handle that flood of data coming in.


## Answer 20119

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-11
- score: 1

Have you seen http://mixpanel.com?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
