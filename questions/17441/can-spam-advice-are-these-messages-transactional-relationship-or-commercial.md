## can-spam advice, are these messages transactional, relationship or commercial?

- posted by: [Sherif Buzz](https://stackexchange.com/users/-1/4592-sherif-buzz) on 2010-12-06
- tagged: `marketing`, `email`
- score: 2

I'm running a dating site and as the volume of emails is growing dramatically, I want to be 200% sure that I am can-spam compliant. Here is the types of emails that I send and how I classify them :

1. On signup, "please validate your email address" -> Transactional, no unsubscribe link  in email
2. Profile approved -> Transactional/Relationship, no unsubscribe link in email
3. Photo Approved -> Transactional/Relationship, no unsubscribe link in email
4. Photo Rejected -> Transactional/Relationship, no unsubscribe link in email
5. Request Password -> Transactional, no unsubscribe link in email

6. Message Received -> Relationship, link to settings page in email

7. Announce new features, send potential matches -> Commercial, link to settings page in email

8. Friend "X" invites you to try site -> Commercial, link to block all invites in email

My concern is about #3 and #4 - when a user uploads a photo to their profile, we send them an email whether it's approved or rejected. I consider this relationship but am not  sure...

Any advice appreciated.




## Answer 17453

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-06
- score: 2

Actually all of your messages are SPAM compliant.  Most mail services like MailChimp or Constant Contact will have additional requirements, but there are 3 main points to the spam act that you need to be aware of:

1. If you are sending a marketing message, it needs to be called that.  So you cannot send an email called "important information about your account" and in the body have links to buy something.

2. Your messages need to show what company is sending the emails, so basically if you have your contact information on the bottom of the email or even a link to your site's contact page you are good.

3. You need to let your users unsubscribe from further mailings.  If you give them a link to unsubscribe on your site you are fine.


On that last point, when a user goes to your site to unsubscribe give them a few options:
1. Remove me from all mailings
2. Remove me from account announcements
3. Remove me from new features 
4. Remove me from tips.



With the four points above you wont be breaking USA law, but might still get blacklisted on a few mail servers.  The reason for this is Yahoo, Gmail, Hotmail etc are pretty strict on what they consider spam.  They dont look at legality but more how users interact with your message and how many mark it as junk.  So with that in mind, send as little unnecessary email as possible, and ask your users to ad your no-reply@yourdomain.com (or whatever address sends the messages) to their safe lists.   Over time, Yahoo, hotmail and others will learn you are legitimate.

Dont use a shared IP address for emails.  Someone else could ruin your reputation. 




## Answer 17444

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-12-06
- score: 0

I believe in both cases (3,4) the communication is specific to the user profile, therefore acceptable exchanges.  Having a link to their profile in the message also would help.

If there is a specific push / process in place to get members to add their photo, perhaps adding in another step would help.

 - **1.5** photo received
 - **2.0** photo accepted
 - **3.0** photo rejected

That way, in 1.5 you are acknowledging that you have received their photo submission, notifying them that it is under review and that a decision is forthcoming (again, profile notification messages are acceptable).  That way, message 2/3 will be expected.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
