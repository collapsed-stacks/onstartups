## Dates on invoices

- posted by: [F21](https://stackexchange.com/users/-1/13598-f21) on 2011-11-15
- tagged: `billing`, `order`
- score: 3

This question is in the context of selling products internationally. How should I date invoices and invoice payment dates?

Assuming we have an online shop based in Sydney, Australia. Should we always date the invoices and payment dates using our local time?

If a customer in Los Angeles purchases a product from us on `15 November 2011 10:00 AM Sydney time`, their local time is `14 November 2011 3:00 PM`. If we send them an automated invoice dated at our local time once the order is placed, then they would have received an invoice from the "future".

Is this acceptable practice? How would you date your invoices?


## Answer 32616

- posted by: [Paul Filmer](https://stackexchange.com/users/-1/14049-paul-filmer) on 2011-11-15
- score: 7

Yes this is acceptable practice to timestamp in local time, even if that means the invoice is 20 hours ahead of the recipient. In 20 hours time it won't matter anyway!

Down the track if you ever need to audit your records, for whatever purpose (tax audit, accountant, debugging a software glitch, etc), you'll be able to trace through transactions chronologically very easily.

Over hundreds of transactions across dozens of online suppliers across the globe I have never seen one adjust to my timezone here in Melbourne Australia.



## Answer 32621

- posted by: [rozon](https://stackexchange.com/users/-1/14441-rozon) on 2011-11-15
- score: 2

You do your filing and the customer does his filing. Your filing is obviously in your timezone, and you really don't care what timezone the customer is filing. :)

If anything you could note the timezone used on the timestamp... I wouldn't bother.


## Answer 32629

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2011-11-15
- score: 2

Most places I worked at where time was important did everything in UTC.  (navy communications, stock market datafeeds, etc)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
