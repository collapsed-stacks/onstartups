## Open source user accounts(openid) OR website specific user accounts?

- posted by: [Syed](https://stackexchange.com/users/-1/594-syed) on 2009-11-24
- tagged: `marketing`
- score: 2

these days i see the trend where websites are offering the user to chose one of his openid to login to the website instead of creating a new one.
it saves the harddisk space for the websites and users have one less account to handle.
Even answers.onstartups.com follows this model.

what are its pros and cons?

is it not used to show advertisers(or investors)how many registered users you have or your customer base? there must be some use of it thats why most of the websites insist on users registering a new account with them.


## Answer 4109

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2009-11-24
- score: 3

First, I would dismiss hard disk space is a non-issue.  

While cool from a technology/security perspective, the major con is the user experience -- having to go to a different site to log in can be a hurdle and a concern for non-technical users and those without an existing OpenID account.  

I guess it depends on your audience but imagine explaining to your mother how OpenId works.


## Answer 4112

- posted by: [John MacIntyre](https://stackexchange.com/users/-1/760-john-macintyre) on 2009-11-24
- score: 2

Hard drive space is a non-issue because your site still needs to set up user account records.  You really only save 2 data columns; password & salt.

And as Jon has pointed out, currently the only users who really understand OpenID is technical users.  For anybody technical ... OpenID is awesome, but if your target audience is non-technical, you may be best with the standard user name password scenario they are familiar with.  Jeff Atwood has alluded to this in the StackOverflow podcast. I believe they had problems with users on moms4mom.com and are currently in the process of adding standard user id / password functionality to StackExchange sites.


## Answer 4115

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-24
- score: 2

You can certainly do both, and from a UI perspective there's sort of three choices:

 1. Allow user to "log in with your Facebook/Gmail/Yahoo/Twitter account."  We know this is OpenID or OAuth but you don't have to say that.  People understand this.
 1. Allow OpenID as a secondary option, so geeks (like us) will also be happy.
 1. Have an option for "Or create a login with us" which *really is an OpenID server under the covers*, but you don't have to tell the user that.

This way you're just supposed one basic authentication technology (simpler for testing, security) but all types of user are happy.


## Answer 4107

- posted by: [Brian Swanson](https://stackexchange.com/users/-1/1150-brian-swanson) on 2009-11-24
- score: 1

I personally can't think of a direct advantage of having website specific user accounts, because with OpenID the website can get profile information about the user signing in, so you end up with most of the information you are looking for anyway.

The major advantage for your users with OpenID is only having to remember a single ID/password, and being able to use that on many different sites.


## Answer 4637

- posted by: [user1797](https://stackexchange.com/users/-1/1797-user1797) on 2009-12-05
- score: 1

A good summary of some of the benefits at https://rpxnow.com/benefits


## Answer 4108

- posted by: [Jon Hadley](https://stackexchange.com/users/-1/1176-jon-hadley) on 2009-11-24
- score: 0

OpenID is currently fine for technical users, but far too confusing for normal users (and some technical users too!), that's why you'll only usually see it on sites like Stack Overflow or OnStartups.

Hard disk / database space is cheap as chips, sites will be offering both options for a long time yet. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
