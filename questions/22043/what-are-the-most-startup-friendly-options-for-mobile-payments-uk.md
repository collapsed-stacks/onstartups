## What are the most startup-friendly options for mobile payments? (UK)

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-03-22
- tagged: `monetization`, `uk`, `mobile-payments`
- score: 4

A young team in the UK has come up with a neat way of creating a social application to help people keep their promises - for instance, keeping up-to-date with their coursework.

Without getting into the details of what they're up to, they believe that small, pre-agreed cash fines are the right 'stick,' and research has suggested that this has to be instant. Their users are willing to volunteer to be fined, but experiments where they've simply been told what they 'owe' haven't worked.

The obvious solution is some kind of mobile payment.

Their website already captures email addresses and mobile numbers, and they are using text messages and email to track progress and report problems (e.g. if I see you out when you said you were working, I can report you and you'll get a text).

To be clear, they don't have, and aren't planning, a mobile app. The solutions they've come up with so far seem pretty good, but they have (for them) high monthly charges. They need the lowest possible recurring cost, even if this means a high per-transaction fee.

The solution needs to work in the UK, and allow pre-pay mobile users to pay a small fee (<£5) - either simply as a fine or as a payment for some virtual goods such as an image, an audio or video file. It has to be possible to trigger this with nothing but a mobile phone number, leading to a simple automated process that could include an exchange of text messages. For instance,

1. The payment could be triggered by replying to the message
2. Or by clicking a link in the message (without depending on smartphone quality browsing)
3. Or the initial service set-up could include some kind of opt-in, so that 'fines' would be fully automated

The team aren't concerned to make money - they consider themselves a 'social enterprise' helping people to help themselves. But they will need at least to cover external costs for a payment service, even at low initial usage volumes.

What providers would you recommend?


## Answer 30212

- posted by: [Ryan Chatterton](https://stackexchange.com/users/-1/3753-ryan-chatterton) on 2011-09-16
- score: 1

Honestly, I've been searching and thinking for you, but I can't think of anything that exists with that criteria. 

I think they are going to have to make it. Could be a game changer.

In fact, the ultimate execution if your question could be more important than the idea they have right now.


## Answer 33732

- posted by: [Mike Eng](https://stackexchange.com/users/-1/15037-mike-eng) on 2011-12-14
- score: 0

<p><a href="http://credit.frontlinesms.com/" rel="nofollow">Try Frontline SMS: Credit</a>.  </p>

<blockquote>
  <p>FrontlineSMS:Credit software enables your business or organization to manage a mobile money account via specially-formatted SMS messages that notify you of incoming payments and initiate new payments to an individual or a group.  </p>
</blockquote>



## Answer 36091

- posted by: [lukeshek](https://stackexchange.com/users/-1/16193-lukeshek) on 2012-02-12
- score: 0

I'm not sure whether I understand the whole concept, but...

1. A user volounteers to take part in this experiment an be fined if caught not following their schedule.
2. Someone else who catch the user sends a text message and the user is being charged.

My question is: how do you want to charge the user? Will he have to pre-pay a certain amount of money (for example on your bank account) and then, if he's caught, you'll take the fine off the money? Or you want to charge his mobile account everytime someone else informs on him?

If you automaticaly want to charge his mobile account, you want to look for SMS MT (Short Messaging Service Mobile Terminated). Unfortunately, I don't know of any English providers of SMS MT. In Poland this service is available for free (no monthly charges), but T-Mobile charges about 200 quid once you activate the service. I believe there is something similar in England. The only thing is that you get only 50% of the ammount a user was charged for.

However, I would suggest that you take the fine off the deposit a user has to pay at the beginning. The person who's reporting would send a normal text, yet to an email address. Then a PHP script would handle the email and charge the fine. This way you won't have to pay any monthly charges.

You should be able to easily send a text message to an email address instead of a mobile phone number, however I've never tried this on any UK mobile network (although I probably had a sim card from every single one).

You could as well get a user's card number and debit his card directly.

As I said, I've never tried sending an email via a text in any UK network and if this doesn't work (in Poland this works in Plus GSM which is a partner of Vodafone, in Play which is a partner of Three, and in Orange which is the same company in both countries), you might try to find out which network lets you receive texts through their website. You could use a PHP app to log in your mobile account and check the messages. 

If the above solutions fail to work, the last one I can suggest is... get a Polish sim card. Cost of sending a text message to a Polish network from an English one is pretty much the same (calling from England to Poland is cheaper than calling from England to someone else in England), about 5-15p a text, but each network enables receiving texts through their website. The only disadvantage is that you fave to find someone who speaks Polish and can help you creat an app checking the account.

In the meantime I made a quick research and for example found that your Vodafone number corresponds to phonenumber@vodafone.net, your T-mobile number to phonenumber@t-mobile.uk.net, etc. If you send an email via a text, this address would show as the sender's email.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
