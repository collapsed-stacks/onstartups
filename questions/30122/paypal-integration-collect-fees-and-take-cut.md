## Paypal Integration - collect fees and take cut?

- posted by: [Venturesocially.com](https://stackexchange.com/users/-1/4597-venturesocially-com) on 2011-09-15
- tagged: `pricing`, `fees`
- score: 0

We are currently building a web application that will help people organise their clubs. As part of this we would like the users of the site to be able to collect payments for their events online. For example, let's say there is a user called John who created an event and the overall cost of the event is $100 and he invites 10 people. 

I would like to be able to then charge each person $11 ($1 is an arbitrary fee) for website fee. Somehow, either directly or indirectly John would get $100.

What is the best model to implement this type of arrangement? 

Do I charge a flat 10% fee, so John pays $10 to me as a fee? But I don't know that 10 is the upper bound of invites?

Do I somehow (and I don't know this part) create a third party account where the 10 people attending deposit the money into this account and then once ready I will deposit the $100 into John's account?



## Answer 30162

- posted by: [Lloyd S](https://stackexchange.com/users/-1/12549-lloyd-s) on 2011-09-16
- score: 1

Take a look at Paypal Adaptive payments as this sounds like it provides the type of revenue distribution you need. 

I suspect you need to be charging 5-10% as a minimum range on top of the base price to cover yourself for transaction fees. The amount you charge above that depends on the the exact service you are providing.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
