## CRM with email integration and useful views for support?

- posted by: [Karen](https://stackexchange.com/users/-1/15449-karen) on 2012-01-06
- tagged: `software`, `customer-support`, `crm`
- score: 3

We're not really a startup, but we're still a small (9 employees + 1 part time sales), growing company and we finally need some CRM software.

Our Owner has been using and loving MS's Business Contact Manager.  It integrates VERY well with Outlook but doesn't seem to be available for multiple users without a little server hacking.

We just brought in someone to do sales part time, and I started a few months back as a Product Manager who also happens to do a lot of customer support.  The Sales Guy has used SalesForce.
I've used/administered Sugar, Oracle/Siebel, and, to a lesser degree, SalesForce in the past.  I'm opposed to these three as I think they are far far too complicated for our needs and I don't much care to administer those systems again.

Obviously, the 3 of us all have quite differing needs (below) and I'm having a hard time finding a solution that will make all of us happy.

- Owner:
 - Integration with an email system
 - Robustness and speed of desktop apps (drag and drop and such)
 - Track/Manage support contracts
- Sales Guy:
 - Simplicity
 - Ability to track leads and opportunities
- Product Manager:
 - Integration with an email system
 - Simplicity
 - Consolidated view of past interactions with customers
 - Easy way to add new customers (take action directly from a selected email)


I've trialed:

 - MS Dynamics - Their Outlook integration is **very** slow and leads much to be desired.  I would expect to be able to right click an email and add that sender as a contact and easily add to the system. Instead, I can "track" a single email thread which also adds an ID number to the email subject.
 - Zoho - Also lacking in the email integration department.  
 - Highrise - I like the simplicity of this so far, but we do have to forward emails to a new account to add to the system.  Some better integration would be nice.
 - Act - Well, I was in progress of testing this, but I'm not installing SQL Server right now...

It seems like there are quite a few systems that integrate with Gmail but we'd have to switch to Google Apps. I've got Capsule, Solve360, Insightly on my list to test if that route seems worthwhile.  

It seems unlikely given how many different things we need it to do, but is there a desktop app that does what we need?  If not, what's the best cloud-based implementation that will work for us?


## Answer 34490

- posted by: [Craig Robertson](https://stackexchange.com/users/-1/9190-craig-robertson) on 2012-01-06
- score: 1

Karen - Have you checked out Sugar lately? In their release 6.3 they have really made strides to simplify the process and really increase the capacity to integrate. You can archive any email using the bcc and a special email tag Sugar provides. Gmail is now integrated as well as face book, linkedin, twitter and a ton of other social media. Not trying to blow too hard for Sugar, but we have been going through similair trials, trying to figure out the best small to mid-size CRM and we keep coming back to and staying with Sugar (yes, we currently use it). There are a bunch of support companies that can help with the admin (search SugarCRM support on Google and see for yourself). We really wanted to stay with open architecture and for the cost vs. features analysis we had to stay with Sugar. 

In fact, the real problem usually lies, not so much in the application but in the integration software and service solution. We spend a great portion of time establishing the appropriate integration platform to work with ease and transparency (read simplicity). It even goes further as we support and maintain the entire platform as well, which ensures adoption and ROI. I am sure it's just as true in other CRMs like Sales Force and Zoho.

Feel free to look me up on our web-site if you have further questions.

Good Luck


## Answer 47365

- posted by: [Curt](https://stackexchange.com/users/-1/23992-curt) on 2013-02-13
- score: 0

The ones you might look at are Worketc.com, relenta.com and infoflo from carmelvision.com
The last one is something you can try on your desktop, but the server edition is what you would want.  If we go with that one, we would put all emails through it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
