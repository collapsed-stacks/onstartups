## Zoho vs. Highrise vs. Salesforce

- posted by: [Alex](https://stackexchange.com/users/-1/2845-alex) on 2010-11-19
- tagged: `crm`, `productivity`
- score: 15

I am looking to finally implement somekind of CRM here, as it get's more painful to run business without it. At the moment Zoho or Highrise seem like solutions I can consider.
We're using Google Apps also, so all email is in there. Zoho seems to handle GMail integration better(at least judging by their video) though.

**Update:** looks like Salesforce could be another good, albeit more expensive option?

I am seeking some recommendations on which one would be better to use and integrate with Google Apps. I am basically looking for the following high level features:

 - Keeping track of customer communications, with reminders when to follow and such
 - Having clear understanding of what's in pipeline, at what stages, how much business closed every month
 - Keeping customer profiles and contact information and sharing it among ourselves here

One thing that I may be looking for in the future is high level project management features.

Can someone who used either of these systems shed somelight of whether they helpful or painful to use for what I need?

Thanks!






## Answer 16740

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2010-11-19
- score: 8

<p>I have deployed ZohoCRM for one of my previous companies, I also decommissioned recently Highrise.</p>

<p>Once you have 2-3 sales people, you will outgrow Highrise. ZohoCRM is built out bit better, but lacks a lot of features. It is a mess to get the data out of either of the systems and get it into new system.  Highrise... not sure what all the hype is about. It is one of the dumbest  CRMs I've used (and I have dealt with turds like SalesLogix and MicrosoftCRM). Only thing it had going for it is semi decent UI.</p>

<p>I would look into something that can scale with you: SugarCRM or... Salesforce (just make sure you squeeze them really hard for a discount in the beginning, since Salesforce sales people are worse than used car sales ones). </p>

<p>UPDATE: recently I wrote an article where I lay out steps you need to take when deploying CRMs and other sales operations components: <a href="http://theoperationsguy.com/building-sales-operations-infrastructure-what-your-team-needs-to-sell-better" rel="nofollow">Building Sales Operations Infrastructure. What Your Team Needs to Sell Better.</a></p>



## Answer 16755

- posted by: [Fabio Ferrari](https://stackexchange.com/users/-1/557-fabio-ferrari) on 2010-11-20
- score: 6

<p>We are using <a href="http://insight.ly/">Insigtly</a> and it seems to be good enough for our needs.</p>

<p>It's simple and not so complete, but it's integrated on Google Apps and it's free for now.</p>



## Answer 16739

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-11-19
- score: 3

<p><a href="http://www.knoxleider.com/2010/salesforce-com-vs-zoho-vs-highrise/" rel="nofollow">Here is a review from someone on the internets</a>.</p>

<p>I'd probably steer clear of 37 signals.  </p>



## Answer 39645

- posted by: [Miriam Schwab](https://stackexchange.com/users/-1/14810-miriam-schwab) on 2012-06-03
- score: 2

We've been using Zoho CRM for about four years now, and it's really met our needs. We track leads, opportunities, quotes and sales orders in there; contacts are kept updated there, and then synced to my Google Contacts account so I've got them on my mobile phone too. Three user accounts are free, any more than that start to be charged, but the fee is really minimal. You can do a lot of customization in there, in terms of adding fields and whole new areas to records.

Salesforce is a great system, but huge in terms of features and costs. I know a few companies and organizations who were using it and moved away, due to the fact that their needs were much simpler and Salesforce was overkill for them.

We tried Highrise, and in my opinion it's just a glorified contact management system. It's not great for managing serious business processes.


## Answer 39598

- posted by: [Matthew Galloway](https://stackexchange.com/users/-1/15145-matthew-galloway) on 2012-06-01
- score: 1

Just checking, have you considered open source?

Great thing is the "zero cost" (in the cold hard cash sense), which also means you are freely able to really give them a good spin around the block at no financial risk!

There are several good ones, I'd recommend:

SugarCRM

vTiger

CiviCRM (if your niche is appropriate for it, I'm going to be using it for a couple)


## Answer 39666

- posted by: [Tariehk](https://stackexchange.com/users/-1/18250-tariehk) on 2012-06-04
- score: 1

We choose Infusionsoft as our CRM.  However, we did a lot of research and Salesforce was the other choice for us.  However, we picked Infusionsoft because it was a less expensive option and it had a lot of functionality that we needed.  I think you should take your time and try the free trials because once you pick a CRM, you do not want to switch it.


## Answer 41866

- posted by: [SJH](https://stackexchange.com/users/-1/19577-sjh) on 2012-09-06
- score: 1

I evaluated Highrise, Zoho, FreeCRM, and Insightly and choose Insightly; it has a good interface and recently they provided documentation for their API. Support team is very responsive and requested features do get implemented. I asked for a feature and found it available in about 2 weeks. What I really like is the Google Gmail gadget you can get a lot done just from your inbox.


## Answer 42075

- posted by: [Hendrik](https://stackexchange.com/users/-1/19628-hendrik) on 2012-09-19
- score: 1

Good answers already, here my personal review after testing and using different CRMs in startups.

**Goal for me**: Time to market and thus productivity is everything. Work hard to receive customer feedback, if good continue, else close the company.

 - **Salesforce**: Very expensive. Has a lot of features and will be perfect when scaling. Lots of easy to generate reports. Problems: We use only 5% of the features, interface is bloat, for developing integrations you need to pay. No me gusta.
 - **SugarCRM**: Free. Has a lot of features. I could do everything I could do with Salesforce. Interface I liked more than Salesforce. Problem: You have to host it on your own. This is a pain, especially as it is developed in PHP. I spent 2 hours per week fixing server configuration problems in a previous startup.
 - **Highrise**: Very cheap. Very productive as it is easy. Clean interface. Easy integrations via their API. Problem: Lacks advanced reports. As a developer you can code them via the API, with no knowledge it is more difficult.

When starting, go for Highrise. Once you have a proof of concept and proof of scale consider switching.



## Answer 17033

- posted by: [dharmesh](https://stackexchange.com/users/-1/4-dharmesh) on 2010-11-26
- score: 0

A lot depends on what your growth plans are and what kind of features you anticipate needing in the future.  Changing CRMs is painful, so investing some time in figuring out the "right" one early is worth it.

When we started, we took the simplest path (Google spreadsheet). Not surprisingly, we outgrew that as the business started to get traction.  We then moved to Salesforce.com.  Overall, that's been a good decision for us.  Salesforce.com is stable, has a rich set of functionality and a relatively open platform (so you're less likely to outgrow it).  But, it does start to get expensive as you move into higher tiers and add a lot of users (we have 100+ now).


## Answer 34971

- posted by: [Remiii](https://stackexchange.com/users/-1/15705-remiii) on 2012-01-19
- score: 0

I use HighRise since 1 year and I look to migrate on SugareCRM, OpenERP or SalesForce.


## Answer 42019

- posted by: [z-boss](https://stackexchange.com/users/-1/9067-z-boss) on 2012-09-16
- score: 0

<p>In case you missed this: <a href="http://en.wikipedia.org/wiki/Comparison_of_CRM_systems" rel="nofollow">Comparison of CRM systems</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
