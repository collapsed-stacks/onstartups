## How exactly is DAU / MAU calculated?

- posted by: [jorisw](https://stackexchange.com/users/-1/25229-jorisw) on 2013-02-27
- tagged: `metrics`
- score: 1

I'm reading a lot about DAU/MAU being a good metric for user engagement. But what is a DAU and what is a MAU?

For Daily Active Users: Is a user not a Daily Active User if they missed one day in the past 30 days?

For Monthly Active Users: Is a user a Monthly Active User if they were present once in the past 30 days?

Should I even be measuring by the past 30 days or should I go by calendar months?


## Answer 47727

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2013-02-27
- score: 1

**'There are three kinds of lies: lies, damned lies, and statistics.'**

There are no hard and fast rules here - It means whatever the implementator decides is a valid action.  

**Example:**  Facebook defines Monthly Active Users as the number of unique users per the past 30 days. 

Which then brings one to another question - what defines a unique user?  In facebook land, these are the actions that are tracked / define it:

  - mock ajax request
  - fbml link click
  - canvas page view
  - click-to-play swf
  - message attachment
  - fbjs ajax
  - accepting a request
  - viewing a profile tab
  - publishing something via a publisher

  As you can see, these actions are meaningless outside of facebook.  To define your own MAU, you need to instrument actions that best describe activities that represent "active" use.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
