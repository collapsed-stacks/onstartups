## How many users do you lose when you don't have a password authentication system?

- posted by: [J. Pablo Fernández](https://stackexchange.com/users/-1/751-j-pablo-fern-ndez) on 2011-03-01
- tagged: `facebook`, `twitter`
- score: 5


If you don't use a username/email and password authentication system and limit yourself to tweeter, facebook, other oauth and openid providers, how many users will you lose? How many will never registered?

Has anybody try to measure it? Or any informed guesses?


## Answer 20964

- posted by: [Arjan Einbu](https://stackexchange.com/users/-1/8166-arjan-einbu) on 2011-03-01
- score: 5

My guess is you lose close to none.

Some things to consider though:

 - Keep the logon process as simple as possible. The user should just click on an authentication method and be redirected to facebook/openid/twitter's page to authenticate.
 - Provide users with a way to register on one of these alternaives if they haven't got an account. MyOpenId is a good choice for this, as it is ONLY a logon-service and nothing else.
 - Provide users with some information on this logon process.

I think StackExchange do good job with all the above...

(I have no data to support this advice, but we're betting on it ourselves.)


## Answer 23241

- posted by: [Shawn](https://stackexchange.com/users/-1/9342-shawn) on 2011-04-12
- score: 5

I can't provide you with any metrics, but one thing to consider when choosing a provider is accessibility. Facebook is blocked at a lot of work places.  If they are blocked and that's the only method of authentication you provide then they can't use your site at work.

So, if you go down this route it's good to provide as many options as possible.


## Answer 23229

- posted by: [simpatico](https://stackexchange.com/users/-1/8280-simpatico) on 2011-04-12
- score: 2

I find it annoying that many sites only offer the Facebook login option and they lose me. But I think OpenID is totally OK.

I'd probably considering adding a help flyover encouraging the users that don't have any to sign up for one, saying that it's their opportunity to get 2 in 1, and provide the sign up link to your favorite.


## Answer 23244

- posted by: [Brian Karas](https://stackexchange.com/users/-1/8465-brian-karas) on 2011-04-12
- score: 1

Depends on what you're selling.  If your gig is selling new cross-stitch patterns to shut-ins, then you probably lose almost 100% of your target.  If you're selling some hipster check-in service, then you might have a net gain because people would appreciate not needing to deal with yet another login (YAL).

Tell us more about your target demographic...



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
