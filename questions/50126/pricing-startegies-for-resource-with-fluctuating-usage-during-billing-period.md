## Pricing startegies for resource with fluctuating usage during billing period

- posted by: [F21](https://stackexchange.com/users/-1/13598-f21) on 2013-08-02
- tagged: `pricing`
- score: 0

We are building an online service and one of the dimensions we want to charge for is storage.

Our model is that the user gets X amount of storage every month and pays for any excess beyond that amount at the end of each month.

Currently, how much storage is being used is gathered every hour. We are considering a few different strategies.

 - A byte hour pricing model modelled after amazon s3's pricing:

> Assume you store 100GB (107,374,182,400 bytes) of standard Amazon S3
> storage data in your bucket for 15 days in March, and 100TB
> (109,951,162,777,600 bytes) of standard Amazon S3 storage data for the
> final 16 days in March.
> 
> At the end of March, you would have the following usage in Byte-Hours:
> Total Byte-Hour usage   = [107,374,182,400 bytes x 15 days x (24 hours
> / day)] + [109,951,162,777,600 bytes x 16 days x (24 hours / day)] =
> 42,259,901,212,262,400 Byte-Hours.
> 
> Let’s convert this to GB-Months:  42,259,901,212,262,400 Byte-Hours x
> (1 GB / 1,073,741,824 bytes) x (1 month / 744 hours) = 52,900
> GB-Months
> 
> This usage volume crosses three different volume tiers. The monthly
> storage price is calculated below assuming the data is stored in the
> US Standard Region:  1 TB Tier: 1024GB x $0.095 = $97.28  1 TB to 50
> TB Tier: 50,176 GB (49×1024) x $0.080 = $4,014.08  50 TB to 450 TB
> Tier: 1,700 GB (remainder) x $0.070 = $119.00
> 
>  Total Storage Fee = $97.28 + $4,014.08 + $119.00 = $4,230.36

- Calculate the excess every hour and add the charge to their owing balance.

- Charge the maximum (peak) amount of storage they used that month.

One of the things we are considering is to tell the user how much excess storage charges they have accrued at this point in time. This is obviously impossible with the average byte hours model.

The maximum (peak) pricing model seems to be the most unfair to the customer from their point of view.

What models for pricing storage or any other resource where usage fluctuates have you implemented in the real world? Which has been most successful?


## Answer 50128

- posted by: [steve](https://stackexchange.com/users/-1/27226-steve) on 2013-08-02
- score: 1

IMHO you should keep your pricing model as simple as possible. 

One of the things that really annoyed me about Amazon pricing for example, is that I just couldn't figure out how much something was going to cost every month (hey - lets measure diskspace in IOPS, and CPUs in ECUs!), as well as the fact they seemed to nickel and dime you for everything. That frustration ultimately led me to forming my own startup to compete with them (http://www.slicify.com).

At least if there is a simple, flat fee you know where you stand, and it's easy to compare your prices with your competitors. In fact, I'd be willing to pay more (in $c per GB) for a simpler price structure because it's much easier to understand what I'll be spending.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
