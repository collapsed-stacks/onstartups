## Bill the clients automatically or send them an invoice?

- posted by: [user3462](https://stackexchange.com/users/-1/3462-user3462) on 2011-02-20
- tagged: `subscriptions`
- score: 2

I am working on a monthly subscription site in which users can cancel/upgrade/downgrade anytime they want. I am integrating the payment module with Paypal and would like to know the pros and cons of billing the users monthly over sending them an invoice and having them manually make a payment.

Personally to me, sending them an invoice is an unnecessary step that requires user's action (and I will need to worry about scenarios such as what happens if they dont pay, do I cut them off from using the system)?

Thoughts?


## Answer 20524

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-02-21
- score: 1

Well considering online payments are the most flexible and easiest option for most, you would be crazy not to have automated online billing as opposed to sending them out an invoice they manually have to pay and read.


## Answer 20522

- posted by: [Andy Cook](https://stackexchange.com/users/-1/6493-andy-cook) on 2011-02-20
- score: 0

<p>You should build the automatic invoicing system. Here are my reasons:</p>

<ol>
<li>After you get more than 5 customers, sending invoices is going to become a pain</li>
<li>Chasing customers for money is a non-value adding activity for your business</li>
<li>Getting paid should be a fun experience for you, not a chore</li>
<li>If it's a task that can be easily automated, you should just automate it to begin with. You can even make your life easier by integrating with a third party service that specializes in bill collections. <a href="https://cheddargetter.com/" rel="nofollow">CheddarGetter</a> and <a href="https://www.wepay.com/howto/collect" rel="nofollow">WePay</a> are some you could use.</li>
</ol>



## Answer 20536

- posted by: [bhanu prasad](https://stackexchange.com/users/-1/7050-bhanu-prasad) on 2011-02-21
- score: 0

If you are really cares about customer service then  sending an invoice is the best way so that these transactions can be viewed by customer or show it to others.Anyways i feel sending invoice will be automatic not manual so it is not a big deal.

If you send an invoice to customers it also adds a mileage to the company because they feel that they are treating very well.



## Answer 20538

- posted by: [burritoboy](https://stackexchange.com/users/-1/7868-burritoboy) on 2011-02-21
- score: 0

Subscription sites that allow upgrades, downgrades and cancellations can become very complex when you begin accounting credits that are due to accounts. Chasing up invoices, then logging the different movements between products, plans and pricing and accounting for discounts can become very cumbersome. If you grow your subscriber base, a manual invoice system will be very difficult to scale.

There are many tools that can help you manage either process you choose. For example, freshbooks.com can be helpful with invoices and chargify.com, zuora, vindicia are examples of tools for subscription billing management.

Also, depending on your product offering you should consider also offering a yearly subscription. Typically, customers on a yearly plan have different retention rates than monthly subscribers and the upfront cash may help you manage growth better.




## Answer 20560

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2011-02-21
- score: 0

I think there is a reason most subscription services work the same way, by automatically billing the customers monthly. You'll probably have enough hassles dealing with expired credit cards and failed payments, so why would you also want to chase people who are late with the payment or aren't paying at all? 

Sending out invoices also seems like unnecessary effort if you can avoid it. Customers usually get access to billing history where they can download invoices/receipts for their records.

Also, there are services like Spreedly, Chargify, Recurly, CheddarGetter which can help you with handling subscription related tasks. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
