## How do you ensure product quality is met when outsourcing development?

- posted by: [Chris](https://stackexchange.com/users/-1/412-chris) on 2012-12-04
- tagged: `development`, `products`, `product-development-cycle`
- score: 1

What terms can be written into an agreement to make sure that a product developed with an outside company meets quality standards such as uptime, speed, etc?




## Answer 44758

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2012-12-04
- score: 2

The terms don't really matter unless you have a big legal budget to fight it out in court. More useful is to have staged payments and withhold those payments if you aren't satisfied.

As an example, you might specify that 50% is paid at "feature complete", 25% at completion and the remaining 25% some time after delivery, when the quality can be properly judged.

Of course, some people may not like these terms, but at least you will have a bargaining stick if things go wrong. In the end, it is all about trust on both sides, so if you can find someone via a recommendation, then that is always a good thing.


## Answer 44761

- posted by: [Pradeep](https://stackexchange.com/users/-1/4404-pradeep) on 2012-12-04
- score: 1

See, outsourcing is not bad, however it is not a silver bullet either. You can not just hand over the specs to your developer and hope that everything will turn out good.

You need to be participating in many activities which are involved in software development. Now you have mentioned two points:

 1. Uptime - First you can arrive to a feasible uptime. Don't expect somebody to promise you 100% uptime. If somebody does that, he is fake. Achieving even 99% uptime is uphill task. So arrive at a feasible figure based on the business needs.
 2. Speed - You can not expect in your spec that "Application should be fast". You need to categorize the sections of your application, and bucket them in page load time. For example - home page should load within 2 seconds. My Account page should load within 3 seconds. This you can catch during acceptance test and hold the payment and demand from developer/company to adhere to what is agreed. But again, don't beat the line. Certain tasks might be agreed for X time, but due to complexity or other obvious reasons, you should be ready to come to a agreeable term.

Apart from these two points for code quality there are several tools which can do static/dynamic analysis and can give you the report of quality of code.

There are so many other tools and best practices guidelines which can help you to identify a fake guy and a good guy.

HTH.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
