## Verifying Business Identity

- posted by: [user744319](https://stackexchange.com/users/-1/13425-user744319) on 2012-01-10
- tagged: `business`, `webapp`, `identity`
- score: 0

My webapp keeps information regarding certain businesses when they use it (Under their full consent off course). One problem i have is that I have no clue how to validate whether the business using the app is the business they claim to be.

How do other startups who use similar data verify a business' identity?


## Answer 34657

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-01-10
- score: 0

If you want to validate the business for some reason then I would suggest you at a minimum send a confirmation email to a business email address they provide. In other words not gmail.com or aol.com but a real business domain like ibm.com.

Now at a minimum you have a reasonable assurance that the person works for or is associated with the business that owns the domain.

Next if that domain has a website, does the website have a SSL certificate and if so what kind. If it is not one of the cheap certs (like GoDaddy), then the signing authority will have done the work to insure the validity of the business.

If on the other hand you have a client that doesn't have a domain name for their email and does not have a SSL cert, then you are undoubtedly dealing with a small company. In such a case perhaps you could ask them to send you ten cents via PayPal as a way to verify the identity of the sender. Not perfect but perhaps better than nothing.


## Answer 34659

- posted by: [user15528](https://stackexchange.com/users/-1/15528-user15528) on 2012-01-10
- score: 0

I think this is a fruitless endeavour. It is very easy to hire people to pose as working for a company and then attempting to demo your product. I just don't see how you can be 100% sure, unless you've met them in their office.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
