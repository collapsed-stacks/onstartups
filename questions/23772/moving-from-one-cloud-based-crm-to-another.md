## Moving from one cloud-based CRM to another?

- posted by: [tcolling](https://stackexchange.com/users/-1/2813-tcolling) on 2011-04-21
- tagged: `saas`, `crm`, `online`, `hosted`
- score: 1

We're a small healthcare-related services company with one sales rep, whom I manage.  We are trying out the Salesforce.com contact manager and it seems to do the job for what we need.  We use Google Apps for email, etc and our sales model is based upon garnering referral sources who will send us individual clients who need our private-pay services.

My question for this group:
If we decided to move from Salesforce to a competing cloud-based product, will we be able to do so without losing data regarding account and contact interactions?

Here's a bonus question, too:
Is there a better choice, from a functionality and price standpoint, that we should use instead?  We want to stay away from non-cloud solutions like Act!, which we have already tried and rejected.

Thanks,
Tim 


## Answer 23780

- posted by: [Alex Miller](https://stackexchange.com/users/-1/8839-alex-miller) on 2011-04-21
- score: 3

<p>It depends on the platform you are trying to move to.  Most of the providers (like salesforce) do not structure their systems to make it easy to get information out - after all, it's in their interest for you not to leave.  They will therefore provide you with the data in a not super user friendly format - usually a giant .CSV file that has to be parsed and manually imported into a new system.</p>

<p>The flipside of that is that a number of providers realize that this is a big pain point and that you would never consider switching without being able to bring your data and have therefore created tools to help you move from Salesforce to their platform.  For instance, Zoho <a href="http://www.zoho.com/crm/crm-data-migration.html" rel="nofollow">has this guide</a>  on migrating away from your old data provider, which basically amounts to "Request your data in a CSV format and we'll do the rest for you".</p>

<p>tl;dr - yes, you'll be able to get your data out, but how easy it is to get it into a new system depends on who the provider is.  If its a SaaS provider and you're moving <strong>from</strong> SalesForce, odds are they will have some sort of system to make it easy.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
