## Managing automatic emails

- posted by: [sk24iam](https://stackexchange.com/users/-1/4660-sk24iam) on 2012-04-25
- tagged: `email`
- score: 0

I have a marketplace website.  There are several types of emails that I am having the coders develop to be sent to users.  For example, when a seller's item is sold they are alerted, when they have feedback to leave, when they receive a message on our website, etc...

What is the best way, as an administrator, to manage all of these alerts?  Is it an industry standard to have the coding team build all of these into the backend of the website to automatically be sent?


## Answer 40175

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-06-25
- score: 1

"Managing all these alerts" is a bit of a wide net.  

If you mean "content creation" I agree with Scott - there are no "standards" around transactional emails - many of the companies tailor them to match the style they represent (A financial company tx email would undoubtedly be more formal than a gamer forum, for example).

There are a few "best practices" sites around (google "transactional email examples" for a few good ones) and there's always Nielsens Usability reports ( http://www.useit.com/alertbox/confirmation-email.html )

If you mean "delivery confirmation" then outsourced mail providers like mailgun, postmark, mandrill are a consideration. Many offer visibility into the delivery process (esp. helpful when support fields new users questions about "I didn't get the email" - you can search by email recipient).  Here's an unverified list of recent ones ( http://socialcompare.com/en/comparison/transactional-emailing-providers-mailjet-sendgrid-critsend ) that should get you started. 



## Answer 38545

- posted by: [Scott Wilson](https://stackexchange.com/users/-1/17652-scott-wilson) on 2012-04-26
- score: 0

It looks like you're doing a good job identifying the specific points at which notification would be appropriate.  There are no specific standards AFAIK that deal with notification, but there are probably regulatory issues regarding email that you'll want to familiarize yourself with (in the region in which you operate).  And it's always a good practice to have an easy opt-out process so that people can pick and choose which if any emails they receive from you.  This will greatly reduce the number of spam complaints you receive (and will thus increase the deliverability of your email). 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
