## Protecting the customer after using our service and avoiding system abuse?

- posted by: [chuck](https://stackexchange.com/users/-1/22377-chuck) on 2013-10-10
- tagged: `service`, `problem`
- score: 0

<p>would really appreciate some help on some difficulties I am facing:</p>

<p>We are developing a service which connects customers with service providers on an agreed price. </p>

<p>The customer puts up a price they were offered from another service provider. Then, other service providers can offer a lower price or better offer to the customer. They can then choose the service provider that is suitable for them.</p>

<p>I am facing a couple of problems though:</p>

<ol>
<li><p>How do we ensure the customer is protected if the service provider changes there price once the service is carried out, increases it for example?</p></li>
<li><p>How do we implement measures so that the customer does not abuse the system when initially putting in the details regarding their original price? I.e setting their own price to beat the process altogether</p></li>
</ol>

<p>Thankyou for your time and responses</p>



## Answer 51346

- posted by: [user60812](https://stackexchange.com/users/-1/19115-user60812) on 2013-10-12
- score: 0

<p>Well, lets start with the first problem<br>
Customer Protection - this involves 2 separate requirements.<br>
First the vendor doing the bidding needs to be protected in case their costs go over the estimate, think construction. Most of the time customers are not great in describing requirements or scope, and having to renegotiate mid job is not a situation anyone wants to be in. You need to also protect your vendors because demand is useless without existence of supply.<br>
Second protecting the customer from malicious vendors. Best way go about that I think is implement an escrow system. So the customer must release the funds to vendor or dispute, either way funds are controlled by your company until issue is settled  </p>

<p>Second problem<br>
Well that's not a problem you need to worry about at all. It's the free market anatomy, if the customer sets the price too low, there will be no vendors who will bid. Thus forcing  the customer to increase. Eventually the community will realize this and wont attempt to lowball too much. One way to remedy is come up with Price Suggestion engine for similar services previously sold. This has 2 benefits of compiling valuable data and providing customers with a decision pricepoint.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
