## Web service with subscription/payment and with automated email

- posted by: [tucson](https://stackexchange.com/users/-1/2407-tucson) on 2011-01-30
- tagged: `email`, `database`, `service`
- score: 2

I am considering starting a business based on daily/regular emails that will be fed an automated process getting data from a MySQL database.

I am looking for a service that:

 1. offers a ready-made website that interfaces with customers for subscription/payment
 2. send emails to my subscribers, triggered by my daily script

I had a quick look at aWebber, but I could not see any feature to automate payment and email delivery. MailChimp seem to have an API, but I cannot find a ready-made solution.




## Answer 19634

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2011-01-31
- score: 2

The poor mans version is the Paypal Subscribe button, you can set the iteration, amounts, and it will send emails based on the transaction result.

You can step it up a bit with services such as CheddarGetter.com, which give you a bit more control, and an api. 

If you have a merchant account, you can also use Authorize.net for subscriptions, that also works through an api, and just like the services above provides safe storage for credit card numbers.

... Usually what I recommend is that you build your own system.  Building your own system affords you to store more information in your db, program refunds, upsells, downsells, retention, and my favorite a pro-rated subscription rate that allows you to bill your customers first on a pro-rated amount then monthly ( this can be done with paypal subscriptions by doing an intial cost, but its much cleaner in your system).

If you are going with the Paypal option, please look into EWP (encrypted web payments) which allow you to encrypt your subscribe buttons and prevent from others from manually changing the dollar amounts.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
