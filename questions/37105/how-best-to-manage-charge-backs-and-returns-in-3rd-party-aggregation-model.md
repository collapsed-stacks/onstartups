## How best to manage charge backs and returns in 3rd party aggregation model?

- posted by: [dmoore](https://stackexchange.com/users/-1/16903-dmoore) on 2012-03-13
- tagged: `insurance`, `service`, `merchant-account`, `retail`
- score: 7

My partners and I are working on a startup and part of our model is acting as a 3rd party aggregator of certain services, similar to a travel agent, meaning customers pay us and we pay the service provider.

My question is, what is the best way to prevent or be prepared for the inevitable instances when: (1) a customer pays with a fraudulent card and we don't find out until after we have already paid the vendor or (2) the vendor provides poor service and the client comes to us requesting a refund?

Is the best thing to hold some receipts in reserve for a period to cover these instances, or is there insurance we can purchase?  Our merchant account provider is holding a 5 percent 6- month rolling reserve against our receipts due to the risk inherent in our model.  Is that sufficient?


## Answer 37237

- posted by: [Alex Cook](https://stackexchange.com/users/-1/6128-alex-cook) on 2012-03-16
- score: 1

Strategically find and sign up *good vendors*. 

In addition, I don't think this is your #1 priority right now.  How are you certain anyone cares? How do you know anyone actually wants this product you are building? Will anyone actually buy anything on your site?

I'd get out and talk to as many potential customers as you can.

Have you read the Lean Startup book? It's a great resource at your stage:
http://www.amazon.com/Lean-Startup-Entrepreneurs-Continuous-Innovation/dp/0307887898

I think you are thinking 50 steps too far in advance.  If you get to the point where you're having to deal with vendor charge backs, that's a good problem to have.  

Startups are about avoiding certain death - so get out and talk to as many potential users as you can!

** Edit 3/12/13
It sounds like you're concerned about handling payments on a marketplace.  I'd suggest checking these guys out:
https://www.balancedpayments.com/


## Answer 49841

- posted by: [Pablo Marambio](https://stackexchange.com/users/-1/26960-pablo-marambio) on 2013-07-10
- score: 0

Given I have worked before at a payment service provider (PSP), I think I know the answer to the first question: _"a customer pays with a fraudulent card and we don't find out until after we have already paid the vendor"_

The thing is, it depends on the PSP and the local payment regulations.

In general, the party that gets paid by the PSP is the one who will suffer the chargebacks. That is, if the PSP pays the aggregator (you) and not the end merchant, then you are liable for the chargebacks. However, in some countries the card holders (in this case, your customers) are liable for the frauds. In this case, the customer cannot trigger a chargeback because he is responsible for the safety of his payment medium. 

If your business is on the first case, that is, if the PSP pays the aggregator and not the vendor and the customer can trigger chargebacks, I would try to cover or limit the liabilities on the contract between you and the vendor. For instance, you could deduct the chargeback (or a fraction of it) from future payments to the vendor.

I guess the answer for (2) _(client asks for a refund when the vendor doesn't fulfill his expectations)_ also depends on the contract between you and the vendors. If I were you, I would try to cover myself against vendors' liabilities.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
