## What is a good first ticket response time/SLA for B2B Saas?

- posted by: [bhttoan](https://stackexchange.com/users/-1/23673-bhttoan) on 2013-05-31
- tagged: `customer-support`, `metrics`
- score: 2

Up until recently, we used our own messaging system with our application for customers to log tickets and then just email for anyone not a client.

We are now trialling Hesk to give us a "proper" help desk and over the last few days we have been looking at average first response times to tickets - I do not mean an autoresponder or moving a ticket etc, I mean when a REAL person reads the ticket and actually replies to the customers enquiry.

At the moment our average response is just under 4 hours (222 minutes) which, for a bootstrapped and free B2B application with 3000 customers globally and no official 24x7 support, I think is pretty good but what is the industry accepted definition of "good"?

I found an article from WooThemes where they are talking about a 12 - 24 hour SLA's and they are achieving ~14 hours http://www.woothemes.com/2013/01/customer-happiness-report-january-2013/ and this link https://support.zendesk.com/entries/21999767-Using-the-Reporting-dashboard on Zendesk shows a graphic which eludes to a global average of just over 24 hours.

Is there any more detailed research on this by industry, country and so on which anyone can share?


## Answer 49348

- posted by: [MDMoore313](https://stackexchange.com/users/-1/23558-mdmoore313) on 2013-05-31
- score: 1

I have to say it depends on your staff and how big of an environment you support. Once place I worked had a ratio of 1 tech for every 500 workstations. We were able to resolve a lot with remote tools right away (first time the user called in), but our standard resolution time was 72 hours. We have to account for multiple locations, other priorities, etc.

In the end, it's really a balance of what can be tolerated by your users, and what you can sustain as a service provider. For example, if your providing service to a hospital that can't afford to wait on you for 12-24 hours, then you must adjust accordingly: Be it charging them a support premium that's used for 24x7 support, biting the bullet and taking the extra load without more compensation, etc.

If you're talking about ***pure response time***, and not ***resolution time***, 12-24 hours is great if you communicate that to your users beforehand (on the 'contact' page, for example). I love when I email a website and get a speedy response from a real person (within a business day or two), some places I've emailed seems like my email got thrown into smtp server of doom never to be seen again, and others just take longer. 

One last thing, by ***resolution time*** I'm wasn't referring to implementing feature requests, but actually fixing an existing feature or bug (unless the resolution is literally just answering their question via email and closing the ticket). Communicating to a user that you received their request is great, but if you never *move* on it, then what's the point I'd ask. You can have an automated response informing them that a ticket has been created right away, and have a person follow up with them with details or when more information is needed.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
