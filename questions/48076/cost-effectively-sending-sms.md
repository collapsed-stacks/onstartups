## Cost effectively sending SMS?

- posted by: [Anonymous](https://stackexchange.com/users/-1/11482-anonymous) on 2013-03-18
- tagged: `cost`, `low-cost`
- score: 4

I'm working on a startup idea (have been for a few months, in fact). Part of this idea revolves around sending SMS reminders/alerts to my customers (fairly heavy usage).

The startup is to be based in the UK and target primarily the UK market which has *very* patchy support for the email-to-SMS gateways you guys in the US seem to have - not that that would be an ideal solution since you need to know their provider.

I was planning on integrating with [Twilio][1]'s SMS API, which looks great (and I still might, depending on the answers here!) but at £0.03 per SMS, it could end up eating into my profit margin too much, given the price point for my product/service I've deemed necessary to shoot for.

What are my other options? Can I buy a mobile phone on a contract with unlimited texts and go-about integrating that with my app somehow. Or can I buy some kind of GSM modem or something? I don't know much(/anything!) about this.

<sub><sup>I thought here would be the most appropriate place since it's something many start ups have probably had to tackle and is more a question of "how do I do this cheaply for my startup?" than asking for advice on the specific technical implementation.</sup></sub>


  [1]: http://www.twilio.com/sms


## Answer 48079

- posted by: [Rudi Visser](https://stackexchange.com/users/-1/25522-rudi-visser) on 2013-03-18
- score: 2

3p is about average for sending SMS messages in the UK, you'd be hard pressed to find something cheaper. I would consider, rather than Twilio, using [BulkSMS](http://www.bulksms.co.uk). I have used these in the past and can vouch for their reliability on the basic package (this is only a personal recommendation though, I haven't used Twilio!).

To cover your final statement with regards to a contract phone, you can of course do this, but it's normally against the terms of service for this kind of usage. What you could do, though, is call up a business manager at one of the phone networks and discuss your options, they may be able to at least match a deal or even beat it if you were on one of their not "unlimited" packages - just explain your situation clearly.

For business tariffs, T-Mobile seem to be the best in the UK, so I would speak to them first.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
