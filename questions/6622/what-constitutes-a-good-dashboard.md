## What constitutes a good dashboard?

- posted by: [Eric](https://stackexchange.com/users/-1/1832-eric) on 2010-01-16
- tagged: `design`, `user-interface`, `metrics`
- score: 7

Dashboards are the 1st screen to welcome users for the 1st time or everytime they use your web app. What are examples of web apps with good dashboard? What do you want in a dashboard? Do you guys have general tips in designing one?


## Answer 6626

- posted by: [Benjamin Wootton](https://stackexchange.com/users/-1/2094-benjamin-wootton) on 2010-01-16
- score: 5

Good question.  

I've logged into a few new web apps recently, and have experienced that 'what do I do now?' feeling on the first use.  

For that reason, I'm putting a lot of effort into merging my sign up workflow and user experience into the first few uses of my app, keeping them on board and walking them through the app, hopefully motivating my users to put the effort into learning the application. 

A few concrete I'm ideas I'm using on my home screen.

1) The ability to easily seed the database with sample data and then drop that data when they are ready to start entering their own.
2) Integrated tutorials that walk them through the use of the software within the context of their own user account.
3) Integrated help files accessible right in the app, not hidden away on the public site. 
4) Optional detailed tooltips which they can turn off once they become proficient with the app.
5) Subtle marketing messages to keep the user excited and interested.

Dashboards for the proficient user are probably a different question.  (Maybe users wouldn't want to be bothered with the above, and would appreciate a traditional management information overview style of dashboard.)  I haven't decided how yet, but I want to move from one style of dashboard to the other as the user moves from beginner to advanced, helping move from new user to expert.


## Answer 6627

- posted by: [Benjamin Wootton](https://stackexchange.com/users/-1/2094-benjamin-wootton) on 2010-01-16
- score: 4

There is also a relevant post by 37 Signals on this topic:

http://gettingreal.37signals.com/ch09_The_Blank_Slate.php

For the design of traditional management information BI dashboards, I can't recommend this book highly enough:

http://www.amazon.co.uk/Information-Dashboard-Design-Effective-Communication/dp/0596100167


## Answer 7247

- posted by: [zendar](https://stackexchange.com/users/-1/916-zendar) on 2010-01-28
- score: 2

<p>Check <a href="http://dashboardspy.wordpress.com/" rel="nofollow">dashboardspy</a> blog. Author collected impressive number of dashboards from very different software systems. </p>

<p>Browse through dashboards and you'll probably find some that you like.</p>



## Answer 6628

- posted by: [Krasimir Evtimov](https://stackexchange.com/users/-1/2262-krasimir-evtimov) on 2010-01-16
- score: 1

The most important thing for any dashboard is the ability to select exactly which gadgets and what type of information to be on the dashboard, instead of several preselected graphs and tables, which in most cases are only slightly relevant to the information that I'm really interested in. It would be really nice if there is an option to change the way in which the data is presented, i.e whether some chart is pie chart or bar chart, etc.

Unfortunately, most of the dashboard that I saw do not have such flexibility.


## Answer 7159

- posted by: [Corey Maass](https://stackexchange.com/users/-1/325-corey-maass) on 2010-01-26
- score: 0

I've been thinking a lot (and trying to implement) incremental UI. When someone creates an account, give them one big option "Start here" or "Upload your first file here" (and a few others like account, sign out). Then once they've done that, show them the second action, "Great, now share it with friends...". Don't show them again once they've done it. 



## Answer 7181

- posted by: [fido](https://stackexchange.com/users/-1/2101-fido) on 2010-01-27
- score: 0

**Tips for brand new clients in a very non-technical market**

One thing that I've been doing very successfully is creating STEP 1, STEP 2, STEP 3, etc. They are the ONLY things that a brand new client can do. If he tries to go to a menu item like "Reports", he gets redirected to "Before you can view reports, you have to set up X".

For example, I have a product for churches that allows church members to set up automatic tithes. Before a church can do anything in the system, they have to create at least one offering, enter in Authorize.net details, enter billing details, etc. Once a step has been completed, it changes colors and instead of "set up now" it says "done". When all steps are complete, the client never sees these again...ever.

After system has been set up completely, they see basic reports, recent tithes, etc.


## Answer 7238

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-01-27
- score: 0

I think an example of a great dashboard is Google Analytics.  From the GA homepage, you get a snapshot of recent activity up top, plus smaller snapshots of visitor trends, map overlay, traffic sources, and content looked at plus links to more detail on all of it, and then a simple navigation on the left.  In addition, a user can further customize what is seen initially.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
