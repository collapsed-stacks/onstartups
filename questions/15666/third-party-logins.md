## Third party logins

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- tagged: `website`, `user-interface`
- score: 0

what is the best way to get up third party logins? Is it a case of going through each client (google, facebook, twitter, workdpress etc) individually? 


## Answer 15710

- posted by: [xiaohouzi79](https://stackexchange.com/users/-1/4868-xiaohouzi79) on 2010-10-27
- score: 1

<p>You should check out the <a href="http://code.google.com/p/openid-selector/" rel="nofollow">openid-selector</a> project. You will notice it is the same as the one built in to this site. Check out the demo page you will see it's almost identical.</p>

<p>It's also very easy to integrate into your site.</p>

<p>Note: This is just 3rd party login and not full user integration. So although the user is authenticated through Facebook etc. it doesn't mean you have access to their Facebook user object with their friends etc. Have a search round the web for authentication vs. authorization to get a better idea of what I'm saying.</p>



## Answer 15667

- posted by: [Siddhartha Oza](https://stackexchange.com/users/-1/4370-siddhartha-oza) on 2010-10-27
- score: 0

Yupp. Pretty much so. For each service that you wish to support for logging in, you would need to write separate code.

oAuth is still far away from its promise. :((


## Answer 15675

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- score: 0

It depends on how you develop the website. Are you using CMS such as WordPress or Drupal?
If you are, most of them have modules/plugins to support it.

But yeah, you do have to code each of them one-by-one, even though some of them uses the same standards such as OAuth used by Facebook, 4sq, and Twitter.


## Answer 15690

- posted by: [Yuri Gadow](https://stackexchange.com/users/-1/5083-yuri-gadow) on 2010-10-27
- score: 0

<p>There is at least one aggregator, <a href="http://www.janrain.com/products/engage" rel="nofollow">Janrain Engage</a>, and a creative Google search ought to turn up more. Additionally, there are free and commercial components you can use in your product that handle some or all of the standards. And, if you prefer to do it yourself the big three standards are OAuth &amp; OAuth 2 and OpenID (which combined net you almost every provider.)</p>

<p>I'd put together a table of all your target providers and their sign in method(s), e.g, OAuth1. If they're all the same, using that standard in your product with third party libraries won't take much more effort than using an aggregator.</p>

<p>I've integrated with Facebook (OAuth2 and still offering FB Connect if you're feeling really masochistic), Google, MySpace, and Yahoo (all combinations of OpenID and OAuth1), Salesforce (really weird OAuth1), LinkedIn and Plaxo (both vanilla OAuth1.) I found every one has quirks and needs from a few lines of provider-specific programming to a hundred to handle those quirks (beyond the mostly identical programming to handle the standard.) Additionally each provider has differing setups, e.g., Yahoo works better with XRDS on your end, MySpace has separate development endpoints, etc.</p>

<p>If you have cash for an aggregator and don't need to deeply integrate the providers' APIs past the sign in, e.g., contacts, status updates, etc., then that is a an attractive way to go, though integrating with an aggregator could take work that exceeds integrating a single standard, e.g, OAuth1 (but probably not two of them.)</p>

<p>If your product uses an even semi-mainstream programming language, you'll have a variety of SDK's and widgets to choose from that'll make using the big three standards surprisingly fast (once you relax accept that each provider has their own idea of standard.)</p>



## Answer 15725

- posted by: [Aymeric Gaurat-Apelli](https://stackexchange.com/users/-1/4785-aymeric-gaurat-apelli) on 2010-10-28
- score: 0

It depends the technology you are using. In Ruby on Rails there are some very easy ways to integrate several third party services without using JanRain Engage.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
