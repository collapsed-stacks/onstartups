## How to simply estimate lifetime of a customer in early days of a startup

- posted by: [Ryan](https://stackexchange.com/users/-1/465-ryan) on 2012-02-06
- tagged: `saas`, `business-model`, `metrics`
- score: 0

How do you estimate (simply) the lifetime of a customer in the early days of a SaaS startup?

E.g. in the first, say 3 months, you will have a number of customers who have already left and a number that are still customers - but you have no idea of how many of these will quit at month 4 or year 4 so how do you estimate the average lifetime to help determine [Customer Lifetime Value (CLV)][1]


  [1]: http://en.wikipedia.org/wiki/Customer_lifetime_value


## Answer 35766

- posted by: [theonetruepat](https://stackexchange.com/users/-1/15795-theonetruepat) on 2012-02-06
- score: 1

The simplest way to measure life time value is when the customer stops paying you. Typically saas companies charge for their software on a recurring monthly basis. If the average customer pays up until the sixth month you have a lifetime value of 6*$monthly charge. 

In the early days it's hard to get a statistically accurate LTV but you should have some baseline numbers you can work with. Keep in mind, I wouldn't bet the farm on those numbers and neither should you. 

Alternatively, you can look at the industry you are in and try to find out what your competitor's average lifetime is and use that as a means to extrapolate your potential CLTV. 

This is just something that gets better with time. 


## Answer 35812

- posted by: [Ryan](https://stackexchange.com/users/-1/465-ryan) on 2012-02-07
- score: 1

<p>I wanted something that would come up with a reasonable answer in the early days so couldn't use Patrick's suggestion.</p>

<p>From the <a href="http://en.wikipedia.org/wiki/Customer_lifetime_value" rel="nofollow">wikipedia article on CLV</a> you have this simple model</p>

<p><img src="http://i.stack.imgur.com/IFTnc.png" alt="enter image description here"></p>

<p>GC = Gross Contribution (gross revenue)
R = retention rate (1-churn)
D = discount rate</p>

<p>Simplifying further by removing discount rate (cost of capital) and substituting churn for retention (r=1-c) this gives :-</p>

<p><img src="http://i.stack.imgur.com/XJk2k.gif" alt="enter image description here"></p>

<p>LT = Lifetime in whatever period you choose for c (churn)</p>

<p>Churn is the number of customers who cancel in any period or</p>

<p><img src="http://i.stack.imgur.com/GRdvV.gif" alt="enter image description here"></p>

<p>An example - suppose we have been</p>

<ul>
<li>Running for 2 months</li>
<li>Have had 100 people sign up</li>
<li>Have had 20 people cancel</li>
<li>Churn per month = (20/100)/2 = 0.1 or 10% (i.e. in any one month 10% of customers cancel)</li>
<li>Average Life Time (LT) = (1-0.1)/0.1 = <strong>9 months</strong></li>
</ul>

<p>Seems to me that this formula will</p>

<ul>
<li>Underestimate LT if your have a large enough subset of your customers who once hooked are unlikely to leave.</li>
<li>Overestimate LT if you have large enough subset of your customers who are loyal until later on (e.g. imagine you were doing some app about tracking pregnancy. Even hooked customers are likely to cancel after 9 months!)</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
