## Do you use a service for ensuring email deliverability (like Sendgrid, Postmark, etc.)? Why or why not? If so, what service?

- posted by: [Mark Bao](https://stackexchange.com/users/-1/58-mark-bao) on 2010-05-15
- tagged: `email`, `deliverability`, `webapp`, `development`, `recommendations`
- score: 4

Using an external service for delivering your emails can take a lot of load off your shoulders if deliverability is a must. Services like Sendgrid and Postmark have pre-configured, whitelisted servers so that your email ensures passage by spam sifters. However, such services are generally pretty expensive, too, especially if you are a high-volume sender.

Do you use an email deliverability service? If so, what service? Why or why not?


## Answer 11198

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-05-15
- score: 3

Having whitelisted servers is a **minor** plus, but why aren't your **own** servers whitelisted? In addition, isn't there a large chance that a servce sending emails for thousands of different compaies is going to attract a spammers?

Finally, whitelisting servers says nothing about your actual email content. Most spam filers look at the actual **content** of the message. If your content is considered **bad**, your email is spam no matter who sent it. Many spam filters these days consider any delivery URL to be spam, shich makes it a challenge to send software delivery emails.


We send our delivery emails from two independent email servers to ensure delivery.



## Answer 11254

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-05-17
- score: 1

*Disclaimer: I am working on a cloud-based email relay (similar to SendGrid) that is in beta right now (and free for the time being, if you're interested in evaluating).* 

Whitelisting and content are both variables in identifying if email is spam, neither is a fix-all, but you need to make sure you have done both (and other work, like getting your email DKIM signed). 

Email Service Providers, like SendGrid, Postmark, and ourselves all have different ways of ensuring the quality of the email leaving our servers. By leveraging our own internal methods for protecting our reputation at the server level and by working with the biggest ISPs (like Hotmail, Yahoo!, AOL, etc) to get whitelisted, we can save you the trouble of having to maintain that deliverability staff or email servers.


## Answer 11330

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-05-19
- score: 0

I use (and know the founders of) SendGrid.  Transactional email deliverability is fantastic, using it for truncation is fun and sending email blasts from mail.app is an added bonus. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
