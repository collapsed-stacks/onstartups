## Sending emails on behalf of customers in a whitelabelable app

- posted by: [J. Pablo Fernández](https://stackexchange.com/users/-1/751-j-pablo-fern-ndez) on 2012-02-16
- tagged: `email`
- score: 1

We built a multi-tenant or whilabelable app so that each of our customers use it to communicate with their users and those users never know we exist. This is quite similar to Zendesk, Basecamp, etc.

We need to send a lot of transactional email, like "thank you for registering", "here's your password reset link", etc. At the moment we are sending it from our own account, our own email address with our domain. Obviously that's not acceptable.

I could just let each customer configure SMTP credentials, but in my experience they are likely to mess it up and our own app will have a poor user experience due to a third party we don't have any control over. I rather solve the problem in-house.

To solve this problem I'm considering Sendgrid and Amazon Simple Email Service but I'm not sure if either will get unhappy that we are sending emails from hundreds of different domains and how do we manage to get those emails reach destination. At the very list I think I'll need to instruct our customers to add the SPF records, right? Anything else? Apparently with Sendgrid I can't use domain keys.

I'm not looking just for the technological question, but also for the business side of things (that's why I'm asking here), any recommended providers?


## Answer 36377

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-02-20
- score: 3

Sendgrid, Postmarkapp, socketlabs, all of those services are designed for exactly what you are  talking about.  No, they shouldn't care as long as it's not SPAM.


## Answer 36279

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2012-02-16
- score: 2

<p>Have a look at <a href="http://mailchimp.com/features/" rel="nofollow">mail chimp</a> I think it has enough of the features you need with an API you can interact with.</p>

<p>Additional: </p>

<ul>
<li><a href="http://automatemysmallbusiness.com/automate-your-life-take-back-your-time/" rel="nofollow">http://automatemysmallbusiness.com/automate-your-life-take-back-your-time/</a> </li>
</ul>

<p>This is probably the best list of resources and the podcast is a good discussion about how to use them effectively..</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
