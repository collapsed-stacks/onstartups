## how does Billguard or Mint.com get the data from banks? Do banks have some open API?

- posted by: [Ryan](https://stackexchange.com/users/-1/12068-ryan) on 2012-03-12
- tagged: `bank-account`, `api`
- score: 1

How is it possible to get the data from the banks? Did they go and talk to each bank and convinced the bank to open a API for them? Or do banks have this API already that they are using and you can just plug into it?


## Answer 37103

- posted by: [abyx](https://stackexchange.com/users/-1/1915-abyx) on 2012-03-13
- score: 4

At BillGuard we use Yodlee's API. Yodlee in turn have several ways of getting the data out of banks - with some they have APIs while with others they just scrape it.

Mint used to use Yodlee, but since they have been acquired it seems they've switched to using Intuit's internal solution.


## Answer 37083

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2012-03-12
- score: 2

For mint the founder teamed up with yodlee because they already offered a service to banks that allowed him to get access to users transactions.


## Answer 40728

- posted by: [Jason](https://stackexchange.com/users/-1/18769-jason) on 2012-07-22
- score: 0

In the very beginning, the founder scraped several sites without using an API.


## Answer 40741

- posted by: [SteveD-](https://stackexchange.com/users/-1/6609-steved) on 2012-07-22
- score: 0

Wesabe screen scraped as described in this post by the founder about how Wesabe lost to Mint.  http://blog.precipice.org/why-wesabe-lost-to-mint

Here is an interview with Aaron Patzer, founder of Mint, talks a bit about how they acquired data.  Key point - some banks support a data exchange API called OFX.  Yodlee aggregated that access and scraped those banks that didn't support OFX. http://www.sramanamitra.com/2009/07/05/the-web-startup-success-guide-part-2-case-study-of-mintcom/





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
