## Converting website visitors to registered members

- posted by: [Sam](https://stackexchange.com/users/-1/10234-sam) on 2012-02-02
- tagged: `conversion`, `traffic`
- score: 0

I've got a niche restaurant rating site, and there is only one direct competitor out there, that has been the go to site for this niche for about a decade. My site is different in every way other than the fact that it has restaurant listings and reviews. Sites like Yelp, etc are very indirect competition, and are not a concern for me at the moment. 

I'm still working out bugs and developing one last feature to complete the MVP. However I'm getting about 50 visitors a day right now due to organic search engine traffic. I have done zero advertising and am not yet ready to market the site. At the same time, I want to get these early adopters signed up and hopefully contributing to the content on the site. Right now, very few of these visitors are converting to registered members.

I have an option for FB login, and also a standard site login. The FB connect is very simple and requires just the users FB login credentials (they would likely already be logged into facebook and so already be authenticated). The standard signup and registration process has been simplified, however I am asking for mandatory things like: (1) first name, (2) last name, (3) email address, (4) username, (5) password, (6) zip/postal code. The optional fields on the signup form are: (1) gender, (2) birth date.

Is this too much to ask of someone to signup? Should I minimize to just username, email address, and password?

What can I do to start optimizing conversions for the early adopters?

Lastly, once a visitor has registered as a member, how can I encourage them to continue to post reviews and keep them coming back to my site?

PS- not sure if it makes a difference, but right now my current target and focus is only on one major city in North America. 


## Answer 35626

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-02-02
- score: 4

You need to put yourself in the customers shoes, if you are a visitor, what benefit do you get by signing up?

If there is no benefit, then asking for any information is asking for too much.

Perhaps you should focus on finding some incentive to offer people who sign up. Could you perhaps offer discount coupons to some restaurants? Of perhaps a chance to be in the "first 500" hall of fame? whatever, figure out ***some*** incentive.

Do you have an email newsletter that people can signup to receive? If not, could you write something simple once a week talking about new restaurants that have opened or that you visited for the first time?

When you delver value, people will signup.


## Answer 35653

- posted by: [dnbrv](https://stackexchange.com/users/-1/15284-dnbrv) on 2012-02-03
- score: 1

First off, I have a feeling that you're misusing the term *conversion* because it means a prospect's advancement down the sales funnel. Thus, if you don't need people to be members in order to make money off them, then you aren't having a problem with conversion.

Secondly, it's hard to say what the cause is and how to increase sign ups. Most likely either your service doesn't seem to be worth signing up (I'm talking about long-term value not BS one-time incentives like others have suggested) or the site has UX issues (unconvincing copy, unclear calls-to-action, layouts, information architecture, workflows, etc).

If you make money on any visitors regardless of their membership status, you should be tracking retention (repeat visitors) and referrals (traffic from 3rd-party sources and direct hits). Healthy growth of these numbers will indicate word-of-mouth support for your idea.

If you actually need people to sign up to make money, then you've got a long road ahead analyzing visitor paths around the site to identify conversion choke points. You'll need to do a lot of A/B and MV testing to optimize the sales funnel.

However, you still need to talk to your users about their needs regardless of how you make money off them. Low signups may be simply lack of trust for Facebook & your service.

P.S. Definitely get rid of the separate username field. Email address is good enough to be a unique user ID.


## Answer 35632

- posted by: [rbwhitaker](https://stackexchange.com/users/-1/15024-rbwhitaker) on 2012-02-02
- score: 0

JonnyBoats is right.  You need to provide something to people who are signed up that everyone else doesn't get.  Perhaps that's the ability to contribute content, as you suggest.  Or a weekly newsletter as JonnyBoats said.  If there's enough value, visitors will fill out very long forms to get registered.  If there's no value, they won't fill out anything.

As far as what information is the bare minimum to ask for, yes, you could probably reduce it.  I don't see a need to necessarily ask for more than an email address and a password.  The rest could be filled in on their profile page later if they want.  The email address allows you to verify that they're a real person, and also can function as their sign-in name.  In fact, logging in with an email address tends to be easier than remembering a different user name or display name for every site, in my personal experience.  While I don't think it's needed, I can understand why you might want first/last name, but what's the motivation for asking for their zip code?  Is this some sort of location based website?

Bottom line is, you need to provide value or you won't get any sign ups.  But yes, there's room to reduce the number of fields you ask the user to enter to register, if you think that might be contributing to the problem.


## Answer 35637

- posted by: [Sid](https://stackexchange.com/users/-1/13800-sid) on 2012-02-02
- score: 0

<p><strong>Login</strong></p>

<p>I'd suggest OpenID login the way this site and other Stackexchange sites use. Even if the actual authentication mechanism/protocols are different behind the scenes, make the UI consistent. There are several OpenID libraries there to facilitate integration.</p>

<p><strong>Incentives</strong></p>

<p>You should see if you can offer enough WITHOUT signup. This incentivizes the user to actually sign up for tailored service. eg: Anonymous listing of restaurants before login or even a video showing what's behind the login curtains. That alone should motivate users to complete an already light signup page.</p>

<p><strong>Lighter signup:</strong></p>

<ul>
<li>You can skip the zipcode requirement or move it to the "complete your profile" page but using their location roughly <a href="http://stackoverflow.com/questions/37015/what-services-can-i-used-to-find-a-users-location-based-on-their-ip-address">based on their IP address</a>.</li>
<li>Try using their email address <em>as</em> the username itself. One less thing to fill, one less item for them to remember. Just remember you should think about people DO change their email address, so your underlying 'username' code should allow for that.</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
