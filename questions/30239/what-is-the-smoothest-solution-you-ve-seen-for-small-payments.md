## What is the smoothest solution you've seen for small payments?

- posted by: [blueyellow](https://stackexchange.com/users/-1/13386-blueyellow) on 2011-09-17
- tagged: `payments`, `ecommerce`, `development`, `micro-payment`
- score: 1

We have a site where visitors can pay 99 cents for a service. It would be cool if the user experience were similar to iTunes: the user clicks one button, doesn't have to type in credit card info, confirms with another button, and then the transaction is over.

Seems like the way to get closest to this is to support a few different payment services (e.g. google in-app payments, amazon fps) then offer the most suitable one to the user -- the one that makes the number of clicks as low as possible. For example, if the user is logged into Google and has a Google Checkout account, offer Google In-App. If the user is logged into Amazon, offer Amazon FPS.

Any examples of existing web apps that do this in an awesome way to make small payments as frictionless as possible for the user? We need some examples of state-of-the-art solutions, given current payment services.


## Answer 30248

- posted by: [xpda](https://stackexchange.com/users/-1/13101-xpda) on 2011-09-17
- score: 1

Amazon's is the smoothest I've used. Any system that saves the payment and customer info online can be made seamless, using a number of payment methods. And any system that saves payment and customer information online needs to be bulletproof from a security standpoint.


## Answer 30256

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2011-09-18
- score: 1

Look at points systems (e.g. istockphoto.com) where you purchase a number of points then spend them. 

Whether these are appropriate depends a lot upon what you are selling and whether your customers expect to be making multiple purchases. They have the advantage that (a) you get money up front, and (b) the micropayment transactions can occur entirely within your website. 


## Answer 30254

- posted by: [simplyme](https://stackexchange.com/users/-1/11458-simplyme) on 2011-09-18
- score: 0

for such a small micro-payment, entering credit card is not a good way. try to use mobile payment if it suits you.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
