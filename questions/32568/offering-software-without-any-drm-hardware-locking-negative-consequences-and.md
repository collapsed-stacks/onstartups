## Offering software without any DRM / hardware locking - negative consequences and how to avoid them

- posted by: [user9982](https://stackexchange.com/users/-1/9982-user9982) on 2011-11-14
- tagged: `software`, `software-licensing`, `piracy`
- score: 3

Let me be the first to play the part of Mr Obvious and state that any DRM can be broken. (I expect the usual amount of upvotes for that)

Now, what are the pros of offering a software without DRM:

1. no need to design, implement, maintain, test, support the DRM component, or no need to buy and integrate the DRM component.
2. everyone can just download and run, so more people end up using the software

I'm concerned about some negative consequences of offering the software without any license protection:

1. If the software is niche (and will stay this way because of its nature), cracks may not even be available. So we are losing a certain amount of income from the sale to people, who would buy the software if DRM would be present (without cracks available).
2. We are losing a certain amount of income from people who would buy the software if their only chance to use it illegally was to use a crack. One reason for that may be that people are afraid of viruses in cracks. The other may be a psychological thing - that is, people are more aware they are acting illegally when they have to actively bypass the DRM.
3. How can a software author enforce some other license restriction without DRM? Again, it's a psychological thing, since users tend to mentally relax EULA points (which they don't read) to their benefit, unless they have to actively bypass the DRM, which enforces them. Example restriction may be use of the software on one PC at a time.
4. How to offer time limited free updates to software? For example, what if we wanted to grant users the right to every new version for 2 years from the time of their purchase? (which is often a necessity to sell anything). With the software freely available, you would have to hope that your customers undergo software audit and the auditors somehow check the date of the installed version versus the date of license purchase. Which would probably mean that the software author would have to embed the date of the build into the software, which would already be a kind of DRM, and would have to hope that software auditor takes notice of it, which is realistically very unlikely if the software is niche.

Do you have experience selling software without technical license protection mechanism? How do you deal with any of the issues raised and possibly other issues?


## Answer 32583

- posted by: [Barry](https://stackexchange.com/users/-1/14427-barry) on 2011-11-14
- score: 2

DRM like open-source, nonprofits and even criminal enterprises are part of the total economy regardless of our moral position on them.  Security is a constant, unending cat-and-mouse gambit.  It's like no one's going to leave their car unlocked because there are car thieves, quite the opposite.

The point of DRM isn't to make it *impossible* for an unlicensed user to take advantage of your precious sweat, but to make it *prohibitively expensive for the average user to hack* such that it's not worth bothering.  There are always some theoretical edge cases, but a practical matter is not leaving money on the proverbial kitchen table esp. if this is your primary means of support (if so, pathos emotional appeal beside a picture, it works wonders).  

Risk management formula (Rational maximization of gain)

    P(Success)*reward - (100%-P(Success))*penalty - opportunity_cost 

 $$ :: $ )

 -$ :: Skip it.

---
Here's some choices:

 - Price an app low enough (2-10 USD) that it just doesn't make sense to break (again, see above).
 - Build a quality app and lock it up.
 - Build a quality app and that has some serious freemium features but leaves large group/enterprisey/pro user things for the $$$ version.
 - Crowdfunding to get going/visibility (e.g., Kickstarter, etc.).


And feel free to try the tipware only route but if you feel extra generous and have an abundance of time. ;)



## Answer 32609

- posted by: [Matt](https://stackexchange.com/users/-1/8784-matt) on 2011-11-15
- score: 2

This very much depends on your software, what it does, and how.

DRM for an entirely offline $5k app is probably a must.  You will lose a percentage to piracy, and, well that's just a cost of doing business as there's no way to entirely stop it.

Of course if your app is in a highly niche area your app might not be popular with the pirates, but for the most part they'll crack everything.  You might be lucky, you might not.

On the other hand we live in an entirely web centred world.  If your app is built around some element of online service, or account, then DRM is probably unnecessary.  It's basically not going to matter if someone pirates the app if it's of limited use without the web services that go along with it.

Sure someone can trade logins and password with friends, but if you track IPs and concurrent logins and block more than say 3 logins at a time for a solo user account etc.

How does the cost of increasing the online subscription aspects compare to the overheads of buying/developing, integrating and working with potentially unpopular anti-piracy measures?

As to your thoughts on psychological effects of having to use a crack, I'm not convinced - surely it's going to be a simple google search for whizzyprogram download?  If there's a link there, pre-cracked, then will they even realise it's been cracked?  Or care?

One thing I am sure of though a lot of users of a cracked app would never consider buying it even if the DRM was bullet proof.  This may due to their financial status, or their personal views.  There's a ton of misinformation about $xxx in lost software sales by the various anti piracy organisations however.  The vast majority of that xxx will never translate into sales even if piracy were somehow made globally impossible.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
