## CRM for small software vendors

- posted by: [Paul](https://stackexchange.com/users/-1/5940-paul) on 2012-03-09
- tagged: `crm`
- score: 2

We are looking for a CRM solution for a small software vendor. We would like to be able to manage classic CRM data such as:

account, contact info, orders, etc.

But there are a couple of other things which are specific to software vendors:

- sales info requests we have received from this person
- support requests we have received from this person
- reminders for ending maintenance contract
- email unsubsription status
- type of contact: customer, somebody who has tried out our software, reseller, a trade show contact
- platforms they use: C++, python, Windows, Linux etc.

I know many CRM platforms can be extended to handle these info, however the amount of effort to integrate support, sales, our custom data field needs is too large for a company of our size. We are looking for a CRM which is specifically tailored for companies who develop and sell software products,

Thanks in advance, 

Paul


## Answer 37019

- posted by: [Anagio](https://stackexchange.com/users/-1/14857-anagio) on 2012-03-10
- score: 2

@Paul you aren't going to find a CRM that will meet your specific needs out of the box. I don't believe that SalesForce is a general purpose CRM. They have spent hundreds of millions in acquisitions and have integrated their applications and have a great API. SalesForce itself can be customized to meet every businesses needs. Have you called them to go over your needs and speak with a specialist who can tell you how to make SF work for your company?

Your sales information requests, can integrate with salesforce

Support requests can integrate with salesforce through zendesk or your own custom app using their API. http://www.zendesk.com/product/features/salesforce

Reminders to end maintenance contracts? Your own application can do this and use SF API to update contacts information

Email unsubscription status? I use Chargify.com on one project they email subscription status's. As does my application built on zend framework, and if needed could be integrated with SF API

Type of customer and their platform? You can create custom fields in SF to popular however you choose. http://www.salesforce.com/smallbusinesscenter/faq/customize.jsp

I wouldn't keep my fingers crossed that you'll find a CRM built 100% for software vendors, way to many variables. Instead you should look for a CRM that is as customizable as possible. SalesForce IMO is it.

All these software companies use SF 
http://www.salesforce.com/showcase/#cloud=all&view=grid&sort=industry&filter=industry-sftwr



## Answer 37108

- posted by: [Milan Stosic](https://stackexchange.com/users/-1/16904-milan-stosic) on 2012-03-13
- score: 0

<p>Hm, have you tried some project management tools - activecollab, basecamp and so ... generaly CRM and project management terms are very similar because when you search for them you search for something to track what you do with your clients, of your projects.</p>

<p>Therefore you cover project management and CRM so maybe to look for some of project management solution suitable for software companies (with some ticketing, invoicing, timetrackig systems) - check <a href="http://www.activecollab.com/" rel="nofollow">activecollab.com</a>. They are working on a new version which will be more powerfull than current one - <a href="http://www.activecollab.com/version-3/" rel="nofollow">http://www.activecollab.com/version-3/</a>)</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
