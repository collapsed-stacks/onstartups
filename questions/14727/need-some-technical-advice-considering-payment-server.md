## Need some technical advice considering payment & server

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-03
- tagged: `payments`
- score: 1

I want to launch an application using the Saas model. Every customer should have his own unique page (including domain name) and login. Next to that they should be able to pay online and be charged every month. 

Since i know absolutely nothing about programming i was hoping that someone could explain me in plain language what the possibilities are and how they should be done. 

tnx in advance! 





## Answer 14729

- posted by: [blparker](https://stackexchange.com/users/-1/4449-blparker) on 2010-10-03
- score: 1

Without much knowledge of the problem, this can be accomplished at almost any level. At the basic level, you can implement your application using an already existent payment gateway like Authorize.NET or PayPal (and many others). The application could be implemented in such a way:

 1. When a user signs up, a username and password is created for his/her account
 2. The username can be used to create a custom URL locating the user's profile
    - Ex: http://example.com/username
 3. You can monitor when the last time the person paid by storing this data in a database
 4. When the next payment cycle is approaching, send a reminder email
 5. If they pay (you can leverage the PayPal or Authorize.NET API to determine this), their account is in good standing
 6. If they fail to pay, you suspend their account

At this level, this isn't terribly difficult to implement, and I would guess that there are solutions out there already that you could purchase to handle just this scenario.

From there, the sky is the limit. You could implement your own payment authorization and billing solution.


## Answer 14734

- posted by: [studiohack](https://stackexchange.com/users/-1/4606-studiohack) on 2010-10-04
- score: 0

For Server questions, you could check out http://serverfault.com

For programming questions, you could check out http://stackoverflow.com

To possible hire someone, check out http://careers.stackoverflow.com/


## Answer 14741

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2010-10-04
- score: 0

Since you know nothing about programming you have to find a programmer (as a partner or an employee) - because you can't create your app without programming.

This programmer will have a technology he/she is better at or more experienced in than others - that is the technology you will build your app on.

When you have something worth paying for you find a payment service provider - the right choice will depend on a lot of specific details you don't know yet (like number of customers), there are tons of companies in this category each with it's own pros and cons.

Anyway, building the system to have different sub-domain (or even domains) for each customer and interfacing with a payment company is relatively easy for any experienced programmer, most of the work - and the part you should concentrate on - is building and marketing the actual application.




## Answer 14739

- posted by: [viv](https://stackexchange.com/users/-1/2665-viv) on 2010-10-04
- score: -1

<p>Benj,</p>

<p>Hosting front:</p>

<p>By individual domains, I hope you mean sub-domains. In that case, you can buy any hosting service ( I would recommend <a href="http://linode.com" rel="nofollow">Linode</a> ) wherein you can create how many ever sub-domains you want - ..com</p>

<p>I wouldn't recommend going for a cloud / Amazon EC2, etc. at this point of time - a simple VPS hosting should be enough</p>

<p>Programming Front</p>

<p>There are multiple ways to get this module working. You could build the framework on your own completely with <a href="http://en.wikipedia.org/wiki/LAMP_%28software_bundle%29" rel="nofollow">LAMP</a> / .NET , etc. (or) use a <a href="http://en.wikipedia.org/wiki/LAMP_%28software_bundle%29" rel="nofollow">CMS</a> to build it</p>

<p>Payment:
Paypal wins hands-down. It's simple and easy to integrate and works like a charm!</p>

<p>HTH</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
