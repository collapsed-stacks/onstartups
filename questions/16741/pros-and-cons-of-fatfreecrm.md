## Pros and cons of FatFreeCRM?

- posted by: [Joseph Turian](https://stackexchange.com/users/-1/423-joseph-turian) on 2010-11-19
- tagged: `software`, `sales`, `recommendations`, `crm`, `productivity`
- score: 1

What are the pros and cons of using FatFreeCRM?

It appears to be a lightweight, open-source CRM package.

**What important features in other CRM packages is it lacking?**

How difficult is it to migrate from FatFreeCRM to something proprietary, like SalesForce.com or Highrise?


## Answer 16812

- posted by: [Kyle West](https://stackexchange.com/users/-1/4267-kyle-west) on 2010-11-21
- score: 1

<p>FatFree is a solid system, but there is a tradeoff of having to maintain it yourself. If you're a rails development shop it should be trivial to get yourself up and running, if not I would spend the couple bucks on Highrise and your more important resource (your time) on your business.</p>

<p><strong>Regarding features.</strong> I have used everything from highrise to zoho to salesforce and the only features we ever really used were contact tracking and deal tracking. Everything other than that is great at a Fortune 500 company but pretty worthless at a startup. You don't need a report to tell you how many potential customers there are and where in the "pipeline" they are when there are 3 of you in the company ... you know.</p>

<p><strong>Regarding migration.</strong> All the data in fat free will be in a database that you own and have control of. Salesforce offers tools to import just about anything so that would simply be a matter of exporting and importing. Highrise, I believe, only allows you to import contacts so you would have to use the <a href="http://developer.37signals.com/highrise/" rel="nofollow">API</a> if you wanted to get your deals in as well.</p>

<p>Hope that helps.</p>



## Answer 16796

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-11-20
- score: 0

I would consider using it if my application was built on Rails.  I still like Highrise the best. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
