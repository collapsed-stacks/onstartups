## ecommerce and pci pa-dss, is it legal to sell/distribute with out it? many o/s carts are not certified

- posted by: [UnStartup](https://stackexchange.com/users/-1/2189-unstartup) on 2010-10-14
- tagged: `software`, `ecommerce`
- score: 1

There are many open source shopping carts that don't have any PCI compliance certification.

Is it legal to sell/distribute ecommerce related software that isn't compliant?

It makes no sense, since if the source code is modified in any way, you probably have to re-certify the software again correct?


## Answer 15116

- posted by: [Adam](https://stackexchange.com/users/-1/4272-adam) on 2010-10-14
- score: 1

My understanding of PCI compliance is that the person handling the credit card personal info or storing it needs to be compliant (so paypal, google checkout, etc).

Do these open source shopping carts take a credit card number, and expect you to run the transaction through the credit card company yourself?

This link sort of gets to the point: http://selfservice.talisma.com/display/2n/index.aspx?c=58&cpc=MSdA03B2IfY15uvLEKtr40R5a5pV2lnCUb4i1Qj2q2g&cid=81&cat=&catURL=&r=0.644091963768005

It depends on if you "process, store or transmit payment cardholder data".


## Answer 15605

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-10-26
- score: 0

My understanind is that PCI is from the credit card companies and so is a policy of use and not a legal / illegal thing.


## Answer 16496

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-11-14
- score: 0

It's not just the Payment Gateways that it covers.

While not a legal thing, there are heavy fines attached to breaches and your ability to take card payments can be revoked which would kill most e-commerce sites.

Think about:

  - Do any staff members process payments over the phone?  They can't write down numbers, you have to have processes in place to mitigate this risk.

  - How is data processed?  Do you store details in your database or files?  Do you hold them in log files (IIS Logs/Application logs).  How do you send it to the payment gateways?  How is error handling done, does it send emails to support staff with card details?

It is not something to take lightly and you should walk into it eyes wide open!

Steve.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
