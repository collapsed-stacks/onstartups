## Is it a bad idea to have a direct credit card buying option on my website?

- posted by: [SpyrosP](https://stackexchange.com/users/-1/9856-spyrosp) on 2011-06-19
- tagged: `website`, `payments`, `ecommerce`
- score: 2

I'm preparing a digital product that I'm going to sell in the days to come. I am a programmer, so I don't have any problems in preparing my website and even setting Paypal to handle my payment system.

It seems that Paypal is the easiest and is probably the one I will be using. But I'm wondering, is it a bad idea to have a direct credit card buying option? I don't know how the procedure would work on charging a credit card directly, but I can safely say (from a programmer's view), that SSL would be invaluable for this one. Do you think that messing with that would be redundant for the needs of a startup?


## Answer 26483

- posted by: [Silver Dragon](https://stackexchange.com/users/-1/10922-silver-dragon) on 2011-06-19
- score: 3

This depends entirely on the product / market fitness of your offering.

Generally, technical folks have no problem with checkout via Paypal; however, for consumer-facing goods, this can hurt your conversion rate -as a lot of folks haven't got (or don't intend to get) a PP account.

Charging CCs directly is more straightforward from all user's perspective; however it puts a lot of complications on the software / business side. Fundamentally, you'll need:

 * A merchant account
 * A credit card processor
 * And either a dedicated CC vault, or a PCI-compliant codebase on your site, to store CC numbers if desired

Generally, either your bank, or Paypal's website payments pro can do most (or all) of this; however both requires passing a credit check, will do some amount of background search on your business, and will require a monthly fee.

Furthermore, since you're a Startup, your number one priority at this stage should be learning about your customers. For this reason, I'd advice to stick up a standard PP "buy now" button, launch, and start learning, instead of messing with this, which could prove to be both costly, and, as you say, redundant.

Hope this helps, and good luck!



## Answer 26488

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2011-06-19
- score: 2

I'd like to provide a counterpoint to Silver Dragon. I think a credit card option is a must, and it's easy to do. 

I think it's safe to say that there are far more people (myself included) who have credit cards and use them online, than those who use Paypal. Do you really want to force your customers to get a Paypal account? A lot of them won't bother and will go somewhere else.

I sell digital goods, and I use Paypal Website Payments Standard to process credit card payments. There is no credit check and there is no monthly fee. They just take around 3% commission on sales. 

From a technical perspective, you just need to put a Buy Now button on your website, so it's not complicated at all. Paypal has its share of issues but it's the easiest way to start taking credit card payments. The alternative is to get a merchant account etc., as Silver Dragon suggested, and here I agree that it's not the best option when you're just starting out.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
