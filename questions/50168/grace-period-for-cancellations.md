## Grace period for cancellations

- posted by: [F21](https://stackexchange.com/users/-1/13598-f21) on 2013-08-04
- tagged: `billing`
- score: 1

We are building a SaaS app where most of the features will be add-ons. Customers can add and remove features at any time and the amount is charged or prorated to their account.

One of the things we are pondering is how to deal with cancellations.

We are considering a cancellation policy like this:

 - Customers can cancel at any time and are given a grace period of 14 days.
 - Once they have cancelled, they can no longer use the app. However, they can log-on during the grace period to reactivate. They can also use this period to download their data.

This leads to 2 problems:

 - If the user reactivates their account, should we change the monthly billing day from their previous day of the month to the day when they reactivate the account?
 - The changing the billing day means that we need to recalculate the amount they have not used during the grace period and pro-rate that, which can be confusing.

Another solution would be to keep their account active and stop billing them at the end of their current billing period. After that, we put their account in grace mode and give them a further 14 days to reactivate or download their data.

The problem with this approach is that it is a bit unfair to the customer. Since we are using a prorated system to bill for add-ons, customers may expect the same to happen for cancellations.

What cancellation policies have you used for your web apps? Did you have a billing policy where add-ons are prorated? Are customers happy to hold out until the end of the billing period or do customers often demand that you refund their money/balance immediately?


## Answer 50212

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2013-08-07
- score: 1

I have dealt with this in two ventures and it really comes down to 3 things.  First, how complicated you want to make your accounting system.  Second, locking in a customer (ethically).  Third, what are your competitors doing (for example you might offer a 14 days grace and advertise it as a benefit. 

In the end, we went with the simplest approach for accounting which is.  x days free trial, billing monthly (no pro-rated).  So bob can sign up today and get a 15 day trail.  Afterwards he can go to a billed account which will bill at $100 month.  We only pro-rate the first bill.  This is because we like to do all our credit card charges on the 1st of the month, and have a few days to deal with expired cards, and failed attempts.  By the 7th of the month we usually know whos account is overdue and they are locked out.  No grace period.  To re-active they simply pay up (this time we dont pro-rate, and the customer is out the days of service for inactivity).  This seems harsh, but they did not get locked out because they "canceled" but failed to keep their obligation and pay.   When they pay, they are back in live status. 

As for cancellations, when a customer cancels they are locked out of our system.  They can log back in at anytime and re-active their account.  If they need their data out of our system, then they can log back in, pay for a full month, and export their data. or they can open a ticket and pay us for an export fee. 

We do this for 2 reasons.  1. We lock in our customers.  2. We understand that once a customer cancels they are of very little value.  Now you might see a few comments talking about customer retention and good customer service, but for us those efforts are best spent on our paying customer base and new customers. 

To summarize, use the simplest approach for accounting and stick with it.   If you want to give up a good chunk of your income use a system like Chargify.com to simplify the whole thing.  But in my example with a pro-rated first payment and hten monthly payment on the 1st its easy enough to code without any 3rd party service. 

PS. Most customers dont read your policies, so dont be afraid to tilt them in your favor. 


## Answer 51271

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2013-10-06
- score: 1

<p>Early on don't get too obsessed with automating all of this stuff.  We set ours up so we can manually fiddle with pretty much everything for our customers.</p>

<p>Why? Because when someone forgets to update their credit card or even cancels I want to send them a personal email or call them to learn why. They may like the service but not use it a ton, but if they get a call from the company to get feedback from them and get their opinions they may be more likely to continue the use.  Early on you need to built relationships and learn a lot about how people use your applications.</p>

<p>But more specific to your question, we don't auto cancel accounts for expired credit cards, they just start to get nagged and then when they add it back in it back charges them. </p>

<p>One of the systems we have locks their account and when they access it the first and only thing they see is the credit card screen until they get their account in order. Depends on the Saas, one system if we just turned it off for late payment it could really hurt their business, so it nags for awhile first.</p>

<p>When someone wants to cancel their are notices that they won't be able to get back in, their information will be deleted etc.  It sounds a little scary for them to cancel, so if they are going to cancel they will think long and hard about it and export their data etc. prior to actually canceling.</p>

<p>We don't actually delete all their stuff when they do cancel, we lock up their account and then delete it in 30 - 60 days. Just in case. But they would have to get in touch with us via email/phone if they wanted to get their data back. You might charge a restore fee or something. This is primarily in place in case someone else at their company had logged in to the account and cancelled it accidentally or intentionally to harm them.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
