## Best way to tell users to upgrade from lite version to full version in a desktop app

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2010-02-17
- tagged: `marketing`, `software`, `trial`
- score: 6

We have a lite version of our desktop software and many features have been removed in this version.

What's the best way to tell people we have those features but they can't access because it's the lite version.
 
**Some ideas:**

 - Keep the GUI just like the Full version but disable buttons those require Full version
 - Keep the GUI just like the Full version and show a messagebox to the user when they click the button. (*put an icon to button indicates that this is Full version feature, they'll pick up the pattern after 2-3 clicks*)
 - Remove all features, don't show them in the GUI and tell them what's been missing in the initial download/installer/welcome message
 - *Any other idea?*

We want users to use the lite version so I don't want to nag them all the time but also I want to lead them to upgrade to Full version. 

One final note: Lite version is **free**


## Answer 8165

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2010-02-17
- score: 2

Here's what we do for our Virtual Time Clock software:

1. Ship separate versions (ours are Basic and Pro)

2. In our evaluation (unlicensed) Basic version, we add a dialog at quit that tells outlines a few benefits of the Pro version and a link to a full feature comparison page (and download) on our web site. The dialog has a 'Do not show again' checkbox so users can stop seeing our Pro reminder whenever they please.

3. Any time we release a Pro update, we notify all our Basic and Pro users of the new features with an upgrade opportunity.


## Answer 8178

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-02-18
- score: 2

Your first two options are, tried and true theories.  The third option, is flawed, and will require you to create a new sales pitch each and every message to keep the idea of them upgrading fresh.

I have seen that dynamic messages in the Splash screen or the Welcome screen, as an effective method of putting the information in front of your Lite Users, without the negativity of spam mail.

Is there a way to randomly enable one small feature of the full version, per start up?  Their is nothing more convincing than to hooking the user into needing the feature


## Answer 8160

- posted by: [Tall Jeff](https://stackexchange.com/users/-1/957-tall-jeff) on 2010-02-17
- score: 1

I would argue the correct answer to this is variable and depends on the type of value proposition and branding image you are creating around your company and products and even the types of users.

Additionally, with that context, I think this is something that you could/should also run A/B experiments on. For example, for each person who installs, at time of first invocation you could randomize a persistent setting to vary the exact way that you nudge them to upgrade for the life of that free install. From there, when they potentially later decide to click the upgrade me button you hit a scenario specific tracking URL to hit on your website. Presto! - Real data! Anyway, the various scenarios possible are used to figure out what textual language and presentation techniques improve conversion rate of installs to upgrade selections and even ultimate purchase. The higher the download rate of the free version, the more scenarios you can test at one time within the random set and still come up with statistically significant results.

*Non data driven opinion*: I would argue that hiding the features completely would be least desirable choice. You definitely want some level of hook to show them what they are missing as long as the approach doesn't make the UI too confusing.

***Note***: For this to work right, make sure your selection criteria at install really is random! - this can be a bit tricky to do well since not all platforms/language tools have a good source of entropy for their random number generator seeds. ie: If the scenario selection criteria is not appropriately random, this will obviously bias the result.




## Answer 8182

- posted by: [Dmitry Leskov](https://stackexchange.com/users/-1/2093-dmitry-leskov) on 2010-02-18
- score: 0

Let your users download a trial that has all features of **Full**, but turns into <s>a pumpkin</s> **Lite** if they do not install a license key in 90 days. Remind them at 60, 30, 15, 7, 3 and 1 day before the expiration, and then every time you release a new version (assuming you have the automatic updates feature and the user have not switched it off).

Optionally, have a *happy day* once a month, and have the trial display a 20% coupon on the happy day that occurs between installation and the first reminder and a 15% coupon on the next one.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
