## How to track customer email support metrics with gmail?

- posted by: [maxua](https://stackexchange.com/users/-1/8650-maxua) on 2011-04-20
- tagged: `email`, `customer-support`, `metrics`, `google-apps`
- score: 4

We're using Gmail to field customer support requests. I am looking for a way to track key metrics of how we serve customers: average response time, %% of inquiries left unanswered, customer "happiness" meter.

Any ideas how to accomplish this? I've tried to search Google Marketplace and haven't found anything good.


## Answer 23725

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-04-20
- score: 2

<p>Are you using any form of CRM system at the moment does it have any of the metrics you are after if so it maybe fairly simple to extract that info and show in GMail?</p>

<p>We use a CRM system called <a href="http://capsulecrm.com/" rel="nofollow">Capsule</a> (though any good CRM should do what Capsule does for us) it has a Gmail/Apps integration for adding users into the system automatically allowing cases/opportunity etc.</p>

<p>We then use a separate platform called <a href="http://rapportive.com/" rel="nofollow">Rapportive</a>, to provide Capsule information back to ourselves with a custom raplet, so the sidebar shows the users open cases/opportunity plus history which we have added. By using the CRM as the centre of our universe but Gmail as the shell to access it we have a lot of statistics (mostly very custom to us) such as user purchases, who last dealt with the customer, last interaction, when the next follow up was meant to be (and if over due) we also have a small happiness widget to indicate quickly if the user was last deemed to be happy (again something we whipped up in an afternoon).</p>

<p>With this information being custom to us it made sense to make it ourselves (our CRM integrates in 3 separate sales ledgers, and numerous support mechanisms as well as email/IM/telephone sales conversations all of this is being put in via the API), though through Raplets we were able to quickly build a platform to see the data, the key part was realising for us Gmail wasn't the place to store the data in the first place but a dedicated CRM.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
