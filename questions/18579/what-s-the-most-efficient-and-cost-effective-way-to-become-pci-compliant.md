## What's the most efficient and cost-effective way to become PCI compliant?

- posted by: [Alex Cook](https://stackexchange.com/users/-1/6128-alex-cook) on 2011-01-05
- tagged: `software`, `credit-cards`, `security`
- score: 3

I'm working on a business-to-business web app.

About a year ago we gave our users the ability to charge credit cards (from customers calling them over the phone) directly within our software system.

Then we found out we needed to become PCI compliant, and we were quoted anywhere from $8,000 to $20,000 to make it happen.

Can anyone comment on this experience?  Have you ever become PCI compliant, and what has it cost you?

We're not storing any credit card information, our server is secure, and we use best practices.  $8,000-$20,000 to look at some code and verify that we're using best security practices seems astronomically high - especially for a startup.  Maybe the process of having a 3rd party audit is more complicated than I think.




## Answer 18583

- posted by: [alphadogg](https://stackexchange.com/users/-1/3197-alphadogg) on 2011-01-05
- score: 5

<p>"We're not storing any credit card information"</p>

<p>But, are you pulling into your servers any cc information, even if only to then transmit it? </p>

<p>Many web apps basically inline service provider screens/code, and do not actually traffic the sensitive data through their own servers. The data may be on your page, but it gets directly sent to a processing server outside your control. (Which means you are an SAQ-A on the <a href="https://www.pcisecuritystandards.org/documents/pci_dss_saq_instr_guide_v2.0.pdf" rel="nofollow">Self-Assessment Questionnaire</a>) </p>

<p>At that point, the primary item is that you should be using compliant software (if you have any shopping cart software you purchased and host) and service providers (the payment processors you may be relying on). You only need to comply with PCI DSS reqs 9 and 12. </p>

<p>Additionally, VISA has its own <a href="http://usa.visa.com/merchants/risk_management/cisp_merchants.html" rel="nofollow">overlapping requirements</a> based on transaction volumes. Assuming you don't process much volume, chances are high you only need to submit the SAQ, and maybe an independent scan. A full audit is probably not required.</p>

<p>However, if you actually receive credit card data, even to then only transmit, or if you have internal processing systems connected to the Internet, you must comply with more requirements, which may include regular penetration testing or actual full audits.</p>



## Answer 18660

- posted by: [Nicknow](https://stackexchange.com/users/-1/5730-nicknow) on 2011-01-07
- score: 3

Honestly, if it is at all possible get out of the credit card processing business.  Push that over to a processing company the way @alphadogg recommends with Authorize.net (and there are several merchants who will do this for you.)  PCI is a pain but it is easily doable even if you have to pay 20k.

My much larger concern for you is what happens WHEN there is a security breach.  It might be a hacker but is much more likely to be someone on the inside (employee, contractor, etc.)  Based on your posting you are actually processing credit cards from your customer's customers.  When you have a security breach you'll have egg all over your face and have to deal with the possibility of legal action, lost customers, and bad PR.

If they are entering the credit card information in the web-app it is very likely you can move to using a processor to handle this part of the transaction.  It will eliminate the PCI compliance issue, improve your site's security (if you don't have CC data you are less attractive to the for-profit hacking world), and avoid any expenses related a system breach.


## Answer 18630

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-06
- score: 0

If you're not storing credit card numbers, have secure servers, etc. generally becoming PCI compliant is fairly easy and inexpensive.  Shop around, sounds like that quote could be way higher than it needs to be.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
