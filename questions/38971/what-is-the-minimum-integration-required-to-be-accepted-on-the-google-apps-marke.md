## What is the minimum integration required to be accepted on the Google Apps Marketplace?

- posted by: [mick g](https://stackexchange.com/users/-1/17157-mick-g) on 2012-05-10
- tagged: `google`, `google-apps`, `marketplace`
- score: 1

I have a SaaS startup and was wondering what the bare minimum would be to publish it on the google apps marketplace. My app currently authenticates users on its own, but im willing to implement Google single sign on. On the pricing front my customers purchase "credits" via Paypal - there's no signup or subscription fee. Will google marketplace allow this given that they wont get any commission? Or will I be required to change my system so users buy credits through Google?


## Answer 51476

- posted by: [gdoming](https://stackexchange.com/users/-1/27436-gdoming) on 2013-10-22
- score: 2

<p>There are a number of optional integrations. But (today) the only one that is required is Single Sign On.</p>

<p>All the details can be found in <a href="https://developers.google.com/google-apps/marketplace/" rel="nofollow">Google's documentation</a>. It specifically mentions SSO as a requirement:</p>

<blockquote>
  <p>"SSO integration is required for installable listings to be accepted into the Marketplace."</p>
</blockquote>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
