## Should I use a seperate but related domain to send reports from my new webapp?

- posted by: [Doug Martin](https://stackexchange.com/users/-1/2126-doug-martin) on 2010-01-03
- tagged: `email`, `deliverability`
- score: 4

In other webapps I've done I've always sent email from the same domain as the app.  However for my next project I'm thinking of using a related domain.  For example if my webapp domain was widgets.com the report emails would originate from widgets-reports.com

The app sends daily reports and I'm wary of getting blacklisted as a spammer.  The emails are opt-in but in the past I've encountered users flagging automatic email they request as spam instead of disabling emails.

If I send from a related domain I should be able move to a new IP if necessary without disrupting the service's primary email.  I really can't think of a downside other than user's expectations that mails would originate from the app domain.

Thoughts?


## Answer 5892

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-01-04
- score: 2

It's nice to use a separate domain, but not because of black-listing, but rather to give you flexibility in how and where the email service is done.

There are SMTP services you can use that will prevent you from being blacklisted; you may want to investigate e.g. smtp.com or MailChimps.


## Answer 5899

- posted by: [dharmesh](https://stackexchange.com/users/-1/4-dharmesh) on 2010-01-04
- score: 2

I like to use separate domains for outbound emails -- it's much more flexible.

The one downside to this is that there is some minimal "brand dilution" (because the domain doesn't exactly match), but I think the tradeoff is worth it.


## Answer 5929

- posted by: [Joe](https://stackexchange.com/users/-1/1572-joe) on 2010-01-04
- score: 0

No.  Generally, ISPs blacklist IPs -- not domains.  So there is a benefit to using a different IP address from the one you use for outgoing corp email.  But the deliverability benefit for using a different domain is smaller than the downside (brand confusion as dharmesh said, maintaining 2 domains, etc).



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
