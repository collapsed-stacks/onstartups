## Strategy for sending email reminders for a SaaS

- posted by: [Owen Fraser-Green](https://stackexchange.com/users/-1/4818-owen-fraser-green) on 2011-05-27
- tagged: `saas`, `email`
- score: 3

I'm building a free-to-use SaaS to help people understand the energy efficiency of their homes and I'm planning to send email reminders to help promote activity in the site e.g. users who registered but didn't activate their account, users who activated but then didn't do anything in the site, active users who appear to have overlooked a feature of the site, etc. 

I don't want to send anything which might be construed as spam and irritate our users so I've come up with some criteria to avoid that such as:

 - Provide an obvious and easy way to opt out of any particular class of reminder or all mails altogether like a link in the bottom of ever mail and a page in the user settings.
 - Allow the longest reasonable delay before sending a reminder e.g. a few days for the activation reminder.
 - When a user qualifies for two different classes of reminder mail at the same time, make sure there's at least a couple of days' gap between when they're sent. They won't appreciate receiving two mails from us the same day.
 - Send repeat reminders but scale it according to the users' activity. Those who've barely used the site should receive one or two reminders and that's it. Those who have shown a lot of activity in the past might qualify for a few repeats spread out over time.
 - Avoid sending reminders the same day that other campaign mails are going out e.g. those advertising new releases.

Does anyone have any advice or other tips?


## Answer 25581

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-05-27
- score: 1

<p>I can't believe I am praising the government but the FTC has a very good description of <a href="http://business.ftc.gov/documents/bus61-can-spam-act-compliance-guide-business" rel="nofollow">how to remain CAN-SPAM compliant</a>. Aside from staying on the right side of the law, it's just plain good advice. The bullet points are:</p>

<ul>
<li>Don’t use false or misleading header information.</li>
<li>Don’t use deceptive subject lines.</li>
<li>Identify the message as an ad.</li>
<li>Tell recipients where you’re located.</li>
<li>Tell recipients how to opt out of receiving future email from you.</li>
<li>Honor opt-out requests promptly.</li>
<li>Monitor what others are doing on your behalf. </li>
</ul>



## Answer 25661

- posted by: [Roy Dictus](https://stackexchange.com/users/-1/8917-roy-dictus) on 2011-05-30
- score: 1

<p>Use a service for this, such as MailChimp (<a href="http://www.mailchimp.com" rel="nofollow">http://www.mailchimp.com</a>). They do this better than anyone would on his own.</p>



## Answer 25674

- posted by: [Joseph Barisonzi](https://stackexchange.com/users/-1/8791-joseph-barisonzi) on 2011-05-31
- score: 1

I really appreciate the focus of this question on how to avoid spam. There might be another frame for this same question which would deliver a positive business development strategy without resulting in delivering spam.

How can you regularly communicate with your prospective users in a way that encourages them to engage with your service?

Obviously if they experience emails from you as spam or as crass commercialization they will not want to engage with your services. 

So to your list of "what not to do" to be identified as spam -- I think you should develop a solid conversion plan that maps out the process of initial contact to long-term evangelists of home energy efficiency. 

Within that plan you might want to consider having every email associated with an action that if taken -- and self reported -- on the site connects the user with some type of access or benefits. This level of engagement will also translate into a much more valuable user base to which to sell to advertisers/sponsors if that is in fact the revenue model. Connection those actions at some point with a social media widget would make the evangelical nature of the mission even more compelling! 
 


## Answer 26144

- posted by: [Rafferty Pendery](https://stackexchange.com/users/-1/11003-rafferty-pendery) on 2011-06-10
- score: 0

<p>The criteria you have put together definitely seems good. In terms of delivery, it is a good idea to use an outside source. </p>

<p>I love MailChimp and they can be great for automating the sending of your emails if you use their API. Another option for that is <a href="https://www.jangomail.com/" rel="nofollow">Jangomail.com</a>.</p>



## Answer 26145

- posted by: [b0x0rz](https://stackexchange.com/users/-1/11068-b0x0rz) on 2011-06-10
- score: 0

activation reminder you should send IMMEDIATELY, because most people expect them right away and even go to the email to do it immediately - so it should be in their inbox in a few seconds.

when a use qualifies for more than ONE (reminder, whatever,...) MERGE the mails and send only ONE. technically slightly more complex, but very logical when you think about it.

--

provide a setting that says: NEVER SEND ME ANY REMINDERS and abide by those who choose / select it. this excludes ONLY the activation reminder (first one, and possibly others if users change their email and have to confirm it).

as a convenience you may provide two more OVERALL settings (not just for reminders):

 - don't send me more than X mails per day
 - don't send me more than X mails per month

where X is configurable by each user.

--

other than that i feel you are on the right track simply be considering this.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
