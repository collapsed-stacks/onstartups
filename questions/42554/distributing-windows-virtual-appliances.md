## Distributing Windows virtual appliances

- posted by: [Cocowalla](https://stackexchange.com/users/-1/2832-cocowalla) on 2012-10-11
- tagged: `software`, `microsoft`
- score: 0

Complex Linux solutions are commonly packaged as virtual appliances.

I'm interested in the Windows side of this, but haven't been able to find much relevant information on the web.

We are building a complex, Windows-based software product that customers will deploy on-site (cloud is not an option), and want to make deployment as easy as possible for customers - a virtual appliance seems to fit the bill.

But I don't know if Microsoft permit this sort of thing, or how it works in terms of licensing.

Ideally we would want to do this for both the evaluation and production versions of our product - but even if we could just use a virtual appliance to allow customers to evaluate the product before purchasing, that would be something.


## Answer 42563

- posted by: [NeedAGeekIndy](https://stackexchange.com/users/-1/19608-needageekindy) on 2012-10-11
- score: 0

What you are talking about is going to be difficult without running afoul of Windows licensing rules.  If you sell a pre-licensed version of your virtual appliance, you would be going against the rules that cover reselling of licenses.  I know you are not reselling Windows licenses for profit, but if MS looks at it and thinks that you are, you are in trouble.  

MS licenses used in virtualization by one company, but owned by another, is another tricky area.  I ran into that with VDI licensing.  It is mostly a complication with Windows 7, but you need to be careful with the MS Server licenses also.

What you want to do is difficult, and overly complicated, but not impossible.  I would definitely consult with a lawyer that specializes in MS licensing.  Sadly, such a thing exists.  One option I see to possibly bypass all of your worries would be to prep your VM, install your software and then SysPrep it to remove all licensing.  The customer would provide their own license.  That is the easiest route, and I think would be a workaround to all of MS's license rules, but consult a lawyer.

If you want to distribute VM's, you really should have started with a Linux platform.  Their licenses were made for such a proposition.  With MS, you are in shark filled waters.  May I ask why you would not package it as an installer for clients to install on their own machines?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
