## How to reduce the number of users who don't complete the registration process?

- posted by: [Sherif Buzz](https://stackexchange.com/users/-1/4592-sherif-buzz) on 2012-11-21
- tagged: `registration`, `user-acquisition`, `user-experience`
- score: 4

I run a dating site, and I'm trying to reduce the number of users who start the registration process but do not complete it. Our registration process is as follows:

1. User enters their email address and chosen password.
2. They're sent an email to validate their email address, and shown a form telling them to validate their email address.
3. User clicks on link in validation email and continues registration process.

We're losing quite a few people at step 2 - they do not validate their email address and never come back. I keep email validation as a first step mainly to be can-spam compliant and also to reduce bogus registrations.

Any advice as to how to reduce the loss during this step?




## Answer 44399

- posted by: [Komra Moriko](https://stackexchange.com/users/-1/21719-komra-moriko) on 2012-11-21
- score: 9

The main thing about registration completion is that _the user needs to care_.  ;)

Without having more information about your specific registration process, here are some things you can do:

**Reduce the likelihood that your confirmation email goes to the users spam folder**

 - Use Litmus to make sure your email content will pass spam
   filters
 - Set up SPF records to verify your sending IP address
 - Consider using a service like SendGrid to increase deliverability
   (you can also monitor open and click rates on transactional emails with SendGrid)

**Test subject lines and email content**

 - Test subject lines, find out which ones most compel the user to open the email
 - Make sure the link the user needs to click is easy to
   click

 - Make sure the user knows what clicking the link will do

 - Emotion is the driver of action, make the content of the email compelling to the user

 - Does the email content look trustworthy and professional?

**Review your current registration process**

From the way you write about it, I suspect that the process is more arduous for the user than necessary. Here are some questions to ask:

 - At what point in the user's visit do you present them with the option
   of registering?
 - Are they engaged enough at that point to make an investment in your site?
 - How friendly is the registration process?

Put your current registration process through UserTesting.com -- you'll be amazed. 

Maximizing conversions is an art. Think like your users. _Really care about your users._ Test, measure, optimize, test, measure, optimize...



## Answer 44541

- posted by: [sarahfriedlander](https://stackexchange.com/users/-1/21526-sarahfriedlander) on 2012-11-27
- score: 1

In addition to what other users have posted here are two other options to make sure your users complete the signup process:

 - Send them a reminder email in spurts of 1 week, 1 month, 3 months if they forgot to validate their email reminding them to do so.
 - Have them create their account with another registration service.  For example on many sites users can immediately login with their Facebook, Google or Twitter accounts which doesn't require them to validate through an email.



## Answer 44647

- posted by: [Sherif Buzz](https://stackexchange.com/users/-1/4592-sherif-buzz) on 2012-12-01
- score: 0

Just to update everybody on what we actually did and plan on doing further down the road.

1. The one main change that made nearly all the difference is moving the email validation to the last step. Our conversion rate doubled just because of this.

2. We already have SPF, domainkeys, etc, so our email does not go to spam (no change)

3. We made the registration process a bit more flexible (more fields are voluntary or can be filled in later)..this caused a moderate improvement.

4. Am now adding Facebook login, will update with stats when we have them.

regards and thanks.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
