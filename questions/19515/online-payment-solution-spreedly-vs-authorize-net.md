## Online payment solution Spreedly vs Authorize.Net

- posted by: [Jewelthief](https://stackexchange.com/users/-1/4547-jewelthief) on 2011-01-27
- tagged: `ecommerce`, `billing`
- score: 1

> **Possible Duplicate:**  
> [What is the best merchant processing solution?](http://answers.onstartups.com/questions/615/what-is-the-best-merchant-processing-solution)  

<!-- End of automatically inserted text -->

I plan to sell online space for multimedia solution and charge user per month (everymonth) or yearly. This would primarily be focussed for USA market, but I forsee people in other parts of globe using it too.

From some other threads, it appears that [Authorize.Net][1] is a popular payment gateway. But I was wondering if there are benefits of using services like [spreedly][2] over it.

What are the points I should consider before deciding my payment engine.


  [1]: http://www.authorize.net/
  [2]: http://spreedly.com


## Answer 19538

- posted by: [Dan Grossman](https://stackexchange.com/users/-1/6897-dan-grossman) on 2011-01-28
- score: 1

They are two different layers in the payment processing stack:

 1. Your merchant account, which you get from a merchant services provider or bank. Either way, it's underwritten by a bank. This is where the money you charge people goes, then they deposit it to your bank account in batches.

 2. Your payment gateway, which provides an API to connect your website to a processing network for credit card transactions. Authorize.net is an example of a payment gateway. You can't use it without a merchant account, it's just a bridge between your website and the processing network the bank underwriting your account uses. 

 3. Subscription-as-a-service companies, like Spreedly. They are almost all new companies whose purpose is to relieve you of having to write all the code to manage recurring billing in your application. They talk to your payment gateway using your credentials the same way your website would if you wrote the code for your payment forms yourself. They don't do replace your gateway and don't work if you don't have a payment provider already.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
