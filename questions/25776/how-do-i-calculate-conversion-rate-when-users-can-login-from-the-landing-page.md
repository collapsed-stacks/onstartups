## How do I calculate conversion rate when users can login from the landing page?

- posted by: [ben](https://stackexchange.com/users/-1/10974-ben) on 2011-06-02
- tagged: `conversion`, `metrics`
- score: 0

I know conversion rate is calculated as

> (signups/visitors)*100

but my landing page is also used as the page that users login to the site. Therefore, some of the visitors will be existing users who are just loggin in. Do I therefore calculate conversion with

> ((signups-logins)/visitors)*100

?


## Answer 25795

- posted by: [AleFocardi](https://stackexchange.com/users/-1/10987-alefocardi) on 2011-06-02
- score: 1

<p>Your view of conversion rate is incomplete. You need to segment only new visitors if you want to use such an simple conversion rate parameter.</p>

<p>The existing user should definitely not be counted for this purpose, depending on how you're bringing traffic to your landing page, you'll be able to calculate it.</p>

<p>Here is a post by Avinash Kaushik on it: <a href="http://www.kaushik.net/avinash/2008/03/standard-metrics-revisited-5-conversion-roi-attribution.html" rel="nofollow">Conversion ROI Atribution</a> </p>



## Answer 25796

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2011-06-02
- score: 0

Create a funnel in your mind:

**Unique** visitors to your landing page

|

**Unique** visitors who completed the sign up


You can use services like statcounter, google analytics etc to put 'traps' on your landing page and the page that informs users on a successful sign up. Over time, you'll have your conversion rate as you measure unique visitors to your landing page vs. unique users who completed the sign up.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
