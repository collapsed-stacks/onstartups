## How to determine interest on overdue payment, based on terms of the contract

- posted by: [user4568](https://stackexchange.com/users/-1/4568-user4568) on 2010-10-01
- tagged: `contract`, `terms-and-conditions`, `payments`
- score: 1

So, like most of the people starting out with own business, I picked a boiler plate contract and made minor modifications and used for a client project.
You might already be familiar with this contract (used over and over on the internet):
http://www.scribd.com/doc/13341916/WEBDEVT-Team-SPARKs-Website-Proposal-ver-12
(This is not our contract, but is a modification of the same template).

But now, the client is overdue on payment and I would like to use the terms of the contract to speed up payment. Terms are (see section 12 of the above).

> Final payment of the remaining balance
> plus any additional charges incurred
> will be due within fourteen (14)
> business days after delivery of this
> email or letter and invoice. If
> payment is not made within fourteen
> (14) days of notification, simple
> interest will accrue on the balance
> owed at a rate of 18% from the date
> the payment was due.

Now, I'm not clear whether the interest is calculated daily or monthly or etc. Say for a payment of $7000 what's the interest for 30 days overdue?


## Answer 14653

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2010-10-01
- score: 1

Ok, hwere we go. This is simple math.

* A year has 360 days, a month 30. Yes, this is how banks calculate, sorry.

* 18% is 1.5% per month.

So, 30 day interest is 1.5% of the orignial sum.

Interest is calcualted daily if needed (period below one month). Max. 30 days a month.

So, 7000 USD; 30 days is 105 USD.

For a lot ofd defauils how that is properly calculated check Wikipedia:

http://en.wikipedia.org/wiki/Day_count_convention

Sadly bankers came up with their own way to do things.


## Answer 14651

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2010-10-01
- score: 0

Here's how I would do it:

Your contract says you charge Simple Interest which means that you don't earn "interest on interest" i.e. your interest payments stay constant, at a fixed percentage of the original principal. 

    I = P * r * t

Where 

    P = Principal = $7,000
    r = Interest rate (18% or 0.04931507% per day)
    t = Number of days past due (30 in your example)

Therefore,

    Interest for 30 days = $7,000 * 30 * 0.0004931507 = $103.56






---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
