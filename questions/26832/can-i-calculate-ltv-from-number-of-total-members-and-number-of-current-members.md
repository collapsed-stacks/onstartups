## Can I calculate LTV from number of total members and number of current members

- posted by: [eoinoc](https://stackexchange.com/users/-1/11530-eoinoc) on 2011-06-27
- tagged: `subscriptions`, `memberships`, `customer-value`
- score: 0

I'm trying to calculate average customer lifetime value of a membership site.

The data available to me is unfortunately either incomplete or very simplistic (or else I don't know how to extract the information needed).

Let's say I can find the total number of signups the site has ever had, plus the number of current members, how can deduct from that the average lifetime of a member?


## Answer 26850

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-06-28
- score: 0

Not really - you're missing a lot of key information. Most importantly, you don't know how long people stay around because you don't know when each person came and left.

Take a simple example and you'll see why: 

* imagine that the site was created January 1st
* the site has been in existence for 1 year
* now it is December 31st
* it has only ever had 3 members
* it now has 1 member

Both of these are equally possible:

* one person joined in March for a day, one person joined in June for a day, and the current member joined yesterday and is already planning to quit. -> Average customer lifetime is 1 day
* Three people joined on January 1st. Two of them just quit, but two more will join tomorrow. -> Average customer lifetime is 1 year.

This is a simplistic example of course but multiply all the numbers by 1000 and it may be more realistic.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
