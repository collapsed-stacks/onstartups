## New Web App / Website - Authentication

- posted by: [Martin](https://stackexchange.com/users/-1/4248-martin) on 2010-10-26
- tagged: `website`, `security`
- score: 1

*(Not sure if this was a programming or startup question, but I will ask you guys)*

Authentication on a new website:

Should I go with OpenId, or use my own Forms-based authentication.  My website is not geared towards technology buffs, so I am thinking I might scare people away with OpenId.  Also, Forms-based is a lot easier (for me) to get up and running.

I would like to offer OpenId in future releases, but I am wondering if I am going to cause myself more headaches by not fully implementing OpenId in the beginning.


## Answer 15594

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-10-26
- score: 3

Why not offer both? I would definitely go with forms-based authentication, specially if your users are not tech savvy, OpenId is great but I have heard from many people offering SaaS solutions that not many people use it. I am currently working in a SaaS product myself and I am using forms-based authentication... if enough people ask about OpenId then I'll implement it later.



## Answer 15682

- posted by: [John Plummer](https://stackexchange.com/users/-1/4891-john-plummer) on 2010-10-27
- score: 2

It depends on your market but I would generally say no.

You're unlikely to lose users by only implementing forms based, but you may lose them if you only implement OpenID.

If this is true for your market, you need to implement forms based. You can add OpenID at a later date, but you should only do so when you have nothing more important to add (which may well be never).


## Answer 15592

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-10-26
- score: 1

I personally dont see any reason to adobt open id.  The benefits for small sites are not that great.  As for user experience, i think its about the same.  Its nice to be able to do a one click registration, but asking someone for an email, name and password is not that devestating where you are going to lose users.

My opinion do what is easiest. 


## Answer 18665

- posted by: [tomeduarte](https://stackexchange.com/users/-1/6408-tomeduarte) on 2011-01-07
- score: 1

You should implement form based authentication, but take care on what platform you'll use.

For instance, if you're using Ruby On Rails, you could use https://github.com/intridea/omniauth or https://github.com/binarylogic/authlogic - that will allow you grow your authentication mechanism as your needs evolve.

You'll find that with most modern web frameworks there are plenty solutions like that available.


## Answer 15622

- posted by: [xiaohouzi79](https://stackexchange.com/users/-1/4868-xiaohouzi79) on 2010-10-27
- score: 0

If you are going to offer OpenId in future releases I would suggest that you either implement or at least work out how you are going to implement it now.

If you build a username/password type sign on and later want to add OpenId support you may find yourself rewriting large parts of the code and database, not to mention having to rework the whole flow of the sign on process.

If you at least think it through (how will you display, store and authenticate different users) and have your database ready with any extra columns you can make the decision to adopt or not at a later phase.


## Answer 15626

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- score: 0

<p>I would also recommend that you implement your own form-based authentication. But you might want to checkout <a href="http://janrain.com/" rel="nofollow">Janrain</a>. They handle the integration with 3rd party services, such as openid.</p>



## Answer 15676

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- score: 0

I believe if depends on your purpose. If your purpose is to simplify users registration, I believe it's best to use form-based registration. But if you intend to integrate your website with social graph features, such as Open-graph on Facebook, accessing Twitter account, then you can use OAuth or other authentication standards.

But generally, I believe you would need them both, unless your website is tightly-coupled with 3rd party sites, such as TwitPic to Twitter.


## Answer 18661

- posted by: [Nicknow](https://stackexchange.com/users/-1/5730-nicknow) on 2011-01-07
- score: 0

Just go with the forms-based authentication.  If your app gets up and running AND you see a demand for OpenID you can look at implementing it.

I've never seen a web-app where OpenID made up any signficant number of users (say more than 2%).  In addition, with the popularity of Facebook, Twitter, and LinkedIn sign-in you would probably be better off (**after** your app is running) looking at implementing those.

Stop 10 random people tomorrow and ask them if they have an OpenID (outside of a developers conference or the Google campus).  I would be shocked if more than 1 of them said yes.  Then ask them if they have a Facebook or LinkedIn account.  You'll probably get 5-6 yes responses - more if you are asking younger people and/or office workers.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
