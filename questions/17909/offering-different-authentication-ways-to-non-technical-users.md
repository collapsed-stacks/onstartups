## Offering Different Authentication Ways to Non-Technical Users

- posted by: [ncakmak](https://stackexchange.com/users/-1/4028-ncakmak) on 2010-12-16
- tagged: `best-practices`
- score: 1

Good Days,

I have recently been tasked with developing an online portal for the real estate agents. I am planning to make the code as generic as I can so that I can use it as a product for the other industry shareholders such as mortgage lenders, small local bankers, closing attorneys, etc..

There will be a login page for some user specific pages that the agents will be able to put their business data.

Knowing that majority of the users will not be technical-savvy, is it a good idea to use different authentication methods such as OpenID and the others like Google and Facebook? Will utilizing them as an additional login facility add any value to the portal and the product eventually? Or, will offering different authentication methods just confuse them?

I am looking forward to hearing your experiences and thoughts.

Thank you!


## Answer 17913

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-12-16
- score: 4

Absolutely!

A number of troubling realities about password-based login are finally making it to the mainstream consciousness thanks to things like the Gawker leak.  Almost every user, technical or not, already as an OpenID, even if they don't realize it.

As long as the interface is clean and easy to understand (I like [Janrain Engage](http://www.janrain.com/products/engage)), offering your users additional login options reduces the resistance to registering.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
