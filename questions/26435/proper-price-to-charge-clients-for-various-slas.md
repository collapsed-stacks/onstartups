## Proper Price to Charge Clients for Various SLAs

- posted by: [AAC](https://stackexchange.com/users/-1/1696-aac) on 2011-06-18
- tagged: `pricing`, `consulting`, `sla`
- score: 3

I am the co-owner of a small web development firm.  We offer Ruby on Rails programming for our clients which mostly consist of small companies.  We typically charge $80-$110 per hour.  For 2/3 of our clients we build large projects, deploy them, handle bug fixing for about 1 month and then disengage.  The other 1/3 we provide ongoing maintenance (additional development).  We set up a service contract for monthly hours billed at a set rate.

How would you suggest I price the following SLAs for those clients which we have service contracts for?

 - Sometimes critical bugs pop up in applications after the 30 day post deployment window closes (at which point bug fixes are no longer free), yet clients want us on call for these things.  They want it done ASAP whether it be 11:00 pm Tuesday or a weekend.
 - In the event a client website gets hacked (we do basic security testing, but we are not security experts), they of course need immediate attention.
 - We set up almost all our client web servers on Amazon EC2.  Sometimes the web server needs a restart.  Sometimes a process is stuck and needs a restart.  Sometimes EC2 itself goes down.
 

  In addition to what I mentioned above, we are increasingly seeing clients that ask for small updates/enhancements that only take a few hours if not less, but they want the turn around time to be 1-2 days or sooner.  What additional charge would you put on our hourly rate for such things.  I was kind of equating it to next day delivery versus standard mail where you have a roughly 30% + cost.  


  Finally, for those of you that have service contracts.  Say 80 hours per month and the clients only used 50 hours.  Do you let that carry over to the next month? 


THANKS!


## Answer 26455

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2011-06-18
- score: 1

I think your best bet is to offer support packages for your clients that want on-going support as maybe a percentage of your original contract or at some fixed, dollar amount per month. 

It gets a little messy if you have support hours, etc simply because you have to keep track of all that and it feels like you are nickel and diming them.

So, my advice would be to have different levels of support (Silver, Gold, Platinum or whatever), charge it per month based on having a paid support staff (with some margin) and see how it goes.

As for specific dollar amounts, that's your call. I would look at how you priced the project as well as the efforts at each level. The old standby is 10-20% of ASP, per year for corporate type software but every business is different.


## Answer 26537

- posted by: [Bob Murphy](https://stackexchange.com/users/-1/5778-bob-murphy) on 2011-06-20
- score: 1

I once did a software support contract like what you discuss.

With that contract, the client prepaid for the equivalent of one half-time person per month. Then they got up to that much work, per month, for no additional charge - with no month-to-month rollover. However, they got 24x7 service, and had a pager number (yes, this was back then) for an on-call engineer who would start work on any problems within an hour. If they needed more work in a month, they paid our regular hourly rate.

Basically, the client was trading losing those rollover hours for getting instant, priority response where somebody on my staff dropped all their work for all our other customers. They were also compensating us for keeping enough slack in our schedule to accommodate that.

> clients that ask for small updates/enhancements... they want the turn around time to be 1-2 days or sooner

In this case, customers want you to drop what you've already committed to do for your other clients without having prepaid for that privilege. Of course, you can't usually do that, so really, somebody will be working overtime.

This reminds me of hard drive recovery services. If you're willing to wait a week or so and let the company work according to its schedule, you pay one price. The faster you want it done, the more you pay. If you want somebody to start immediately and work continuously until the hard drive is recovered, you often pay three times the "normal" rate.

So I think a 30% premium is really undercharging for 1-2 day service. You might consider using a rate schedule like:

 * Start in one week or more: our normal rate.
 * Start in two days: 1.5x our normal rate.
 * Start tomorrow: 2x our normal rate.
 * Start today: 3x our normal rate.

That way, your customers get to make their own decisions about speed versus cost, and the more you're having to juggle your commitments and guzzle stale coffee, the more you hear a nice "cha-ching!" sound in the background.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
