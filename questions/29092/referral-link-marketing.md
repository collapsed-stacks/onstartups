## Referral Link Marketing

- posted by: [Beau](https://stackexchange.com/users/-1/12868-beau) on 2011-08-20
- tagged: `marketing`, `referrals`
- score: 1

I'm interested in utilizing the viral marketing tactic of unique short-code URL referral. I can't figure out how this is done - my Google search terms are insufficient. Is there a unique-link referral tracking app that provides this service out-of-the-box?


## Answer 31764

- posted by: [menuflavors](https://stackexchange.com/users/-1/13964-menuflavors) on 2011-10-22
- score: 1

I don't know if there is an out-of-the-box solution, but being a developer I can tell you one way to implement it.  The destination url should be saved in a database table with a given identifier.  If your domain was short.ly then the short url would be short.ly?id=someId or short.ly/someId.  This would look up the destination url and then redirect by returning some 300/3xx status code.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
