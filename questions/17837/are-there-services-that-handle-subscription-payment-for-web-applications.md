## Are there services that handle subscription payment for web applications?

- posted by: [Bill](https://stackexchange.com/users/-1/5989-bill) on 2010-12-15
- tagged: `payments`, `subscriptions`, `webapp`
- score: 3

I currently run a startup that sells an iPhone app through the App Store.  I love that the App Store takes care of the work of charging users, collection of sales tax, basic reporting, etc. and just wires over the final revenue at the end of the month.  I think it's been a huge boon to independent developers, who can focus on just building a product.

I'm curious if there's something similar for web applications with a paid subscription model.  I know Google Checkout has subscription support but as far as I can tell, it's not as comprehensive as the App Store model.  I was excited by the Chrome Web Store, which seemed to offer this service, but I definitely can't use a service that's limited to only one browser.

Just curious if anyone's seen anything like this.  Anything I should take a look at?

Thanks!


## Answer 17840

- posted by: [Cameron McGrane](https://stackexchange.com/users/-1/1010-cameron-mcgrane) on 2010-12-15
- score: 3

SAAS wise you could investigate http://recurly.com/ and http://chargify.com/ 

Dev side you could research http://servicemerchant.org/ open source dev kit.


## Answer 17841

- posted by: [Emile](https://stackexchange.com/users/-1/5988-emile) on 2010-12-15
- score: 3

Actually depending on who your merchant service processor is, you may already have a set of tools.  For instance, authorize.net has CMS so you can do recurring billing.  All the data is collected and reported for you.

If you want a more web 2.0 feel for you and your customers, you can integrate authorize.net with http://www.freshbooks.com/ or http://www.chargify.com  .  I'd recommend the former for larger invoice projects and the latter if you have a few tiers of relatively low-pricing schemas.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
