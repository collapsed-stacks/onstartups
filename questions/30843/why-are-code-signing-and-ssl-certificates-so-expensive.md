## Why are code-signing (and SSL) certificates so expensive?

- posted by: [Nestor Sanchez A](https://stackexchange.com/users/-1/1476-nestor-sanchez-a) on 2011-09-30
- tagged: `software`, `web`, `security`
- score: 4

I was looking for cheap code-signing certificates, but all I saw were over $100/year. I think the same applies to SSL certificates.

I read some references to insurance coverage amounts, maybe to be paid if a "certified customer" falls in improper or criminal behaviour.

In comparison to domains, certificates are very expensive. Could someone tell me why?

Plus, why not rely on credit card ownership to demonstrate some level of credibility?



## Answer 30846

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-09-30
- score: 11

The low end on code signing certificates seems to come from Comodo resellers, who offer certificates from $90 - $100. Code signing certificates are fairly specialized. There is not a large market for them. In addition, they require actual **manual** work to verify the information you provide when you get one. While code signing certificates can be revoked, much of the software that checks for signing does **not** go on line to verify the signature has not been revoked, hence the need for greater security when issuing such a certificate.

SSL certificates are available for **much** lower prices. I have seen them go down to about $15. SSL certificates can be issued automatically, if all your company details match up. SSL certificates can (and often are) revoked at the browser level, with new browser releases. (Check out the Diginotar revokation in the last month.)

Domains have **nothing** to do with certificates. Anyone can buy a domain. Owning a domain name says nothing about the reliability of that company.



## Answer 30845

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2011-09-30
- score: 3

Issuing authority have to perform some background check and papers validation (company registration, photocopy of some documents etc. ) that is done manually. They have to provide time server as well.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
