## Protecting user data in multi-tenant SaaS

- posted by: [LC Yoong](https://stackexchange.com/users/-1/10686-lc-yoong) on 2011-10-20
- tagged: `saas`
- score: 0

What is your take on the ownership of members data in a multi-tenant SaaS (Software as a Service). I am designing a reservation type SaaS for the use of mainly two groups of people - the consumers and operators. 

The operators manage their reservation (for the consumers) via the SaaS. The operators can sign-up customers (walk in customers) into the system. 
The consumers can a) sign up on their own and link themselves to the operators of choice (hence one-time sign up) OR b) being signed up by an operator. Either way, the consumer now has a universal account in the ecosystem and can engage the service of any operators they like.

The question is what level of ownership the operators can lay claim on the consumer data?


## Answer 31652

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-10-20
- score: 1

I am making some guesses here based on the limited information provided...

The operators should only be able to view/report on data related to their business.  Even if an operator has signed up a consumer, they should only see data of that consumer related to their operation. 

If the consumer links in with other operators, this shouldn't be available to the original operator.

Without this, you won't have the trust of your consumers.

I try to make these decisions based on what is intuitive, and what would you expect... in this case, from the consumers point of view. If you can't put yourself in their shoes... then ask them.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
