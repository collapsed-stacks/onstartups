## Do you have a recommendation on a micropayment credit card processor?

- posted by: [Jason](https://stackexchange.com/users/-1/4233-jason) on 2010-09-20
- tagged: `credit-cards`, `payments`
- score: 2

The transactions on my website are between $0.99 and $5.00. Paypal and other similar processors, charge 2.9% with a $0.30 transaction fee. This fee structure (particularly, the transaction fee) absolutely kills my margins. I'm in the process of researching micropayment processors.

The only one I've been able to find so far is Amazon FPS -- http://aws.amazon.com/fps/pricing/. For transactions under $10, they charge 5% with a $0.05 transaction fee which is great. The only negative aspect is the fact that users have to go from my website, over to Amazon, login (register if they don't have an account) and then pay. I'd much prefer to keep users on my own website, in my own cart. 

Two questions --

1.) Do you have experience with Amazon FPS? If so, what are your thoughts on the service?

2.) Can you recommend or know of any other micropayment credit card processors?

Edit:

Alex, below, pointed out that Paypal also has a micropayments solution: https://www.paypalobjects.com/IntegrationCenter/ic_micropayments.html

Does anyone have experience with Paypal's solution? If so, what are your thoughts on the service?

Thanks,
Jason


## Answer 14141

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2010-09-20
- score: 1

Paypal offers an option for accepting micropayments up to $12 for 5% + $0.05. There's some more information at https://www.paypalobjects.com/IntegrationCenter/ic_micropayments.html, but in typical Paypal fashion it is very sparse, so I'm not even sure that it processes credit cards and not just Paypal account transfers. Perhaps it's something you could try out though.


## Answer 14158

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2010-09-21
- score: 0

Amazon offers an API to their payments service so you should be able to keep the users on your web  site.
http://aws.amazon.com/fps/faqs/#b1

I would find a third party vendor that supports this, rather than try and implement from scratch



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
