## Do Google consider CNAME domains as duplicate

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-07-02
- tagged: `dns`, `domain`, `google`
- score: 1

I have domain1 and domain2. I want my visitors to use both to reach my product web site at domain1. Do Google will consider domain2 as duplicate content if I point it to domain1 via CNAME directive in DNS zone?


## Answer 12480

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-07-04
- score: 1

What you should do is host domain2 and use an HTTP 301 Redirect to send the browser to domain1.  Google recognizes this not only as "not duplicate" but sends all your domain2 "juice" to domain1.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
