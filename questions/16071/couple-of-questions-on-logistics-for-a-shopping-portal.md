## Couple of questions on logistics for a shopping portal

- posted by: [Sandeep](https://stackexchange.com/users/-1/5233-sandeep) on 2010-11-04
- tagged: `shopping`
- score: 1

Hi…I am exploring the feasibility of a niche shopping portal. Am yet to finalize the product but one of the strong potential short-lists is luggage and bags. A couple of areas that I’m hoping for directional inputs are -

1. How do we update the images (pictures with different angles with or without models) /information/specifications of the product, especially if they are drop shipped directly to the consumer from different locations of the brand manufacturers across the country?

2. How to update inventory available with the vendor? (assuming we are not storing inventory initially). As in how does one keep track of the number of pieces of a product available with the supplier/brand in real time so that a consumer does not order anything which has just gone out of stock

cheers,

Sandeep


## Answer 16074

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-11-04
- score: 1

> How do we update the images (pictures
> with different angles with or without
> models) /information/specifications of
> the product, specially if they are
> drop shipped directly to the consumer
> from different locations of the brand
> manufacturers across the country?

Usually the manufacturer or, if you have one, your upstream distributor, will provide you with those images.
 
> How to update inventory available with
> the vendor? (assuming we are not
> storing inventory initially). As in
> how does one keep track of the number
> of pieces of a product available with
> the supplier/brand in real time so
> that a consumer does not order
> anything which has just gone out of
> stock

Look for suppliers that offer an API to get this information from them in real time, and if there isn't already a tool for your platform that uses it, hire a qualified dev to do the integration.

--Susan



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
