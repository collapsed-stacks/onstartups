## Singleboard/SOC based products and IP laws for a small company

- posted by: [SuperTron](https://stackexchange.com/users/-1/14843-supertron) on 2012-05-07
- tagged: `intellectual-property`, `products`, `licensing`, `small-business`
- score: 0

I run a small business in custom software development in Canada, and I think it has gotten to the point where I can release my own product.  My question has to do with using existing singleboards/SOC's in a new product design, and the licensing problems that come along with this.  To be more precise, I would like to use a [CuBox](http://www.solid-run.com/products/cubox) in a product that I can sell to the general public.  Is this possible, or should I design my own SOC for this purpose to avoid IP issues?  Any tips would be appreciated.  Thanks beforehand.


## Answer 38879

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-05-07
- score: 1

<p>Upfront <a href="http://en.wikipedia.org/wiki/IANAL" rel="nofollow">IANAL</a> - so it would be worth asking one.</p>

<p>It seems that solid-run is in the business of delivering a armada 500 soc packaged solution (but they have not delivered it in volume as of yet) so it is likely they "want" you to use their product to deliver a solution to your customers.  Since we don't know exactly what your product is, and whether it requires all the functionality that the CuBox intends to deliver - its difficult to determine fit.  </p>

<p>Since the OS stack is open source, and there is no mention of licensing restrictions on the CuBox site, I would send a question regarding commercial use / restrictions / licensing on their site (or sales@) and see how they respond.  </p>

<p>Designing your own SOC allows you to get exactly what functionality you require for your app ... at the expense of a higher engineering cost upfront until the volume increases that the BOM (bill of materials) + internal support is cheaper
than an COTs solution. That probably would be the bigger concern here vs. licensing costs - but without product understanding, its just a guess.</p>

<p>Good luck with your effort.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
