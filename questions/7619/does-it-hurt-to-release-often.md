## Does it hurt to release often?

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2010-02-04
- tagged: `release`, `marketing`, `software`, `development`
- score: 3

I'm a big believer of "release early, release often" but what's the limit?

**Our software**

 - Traditional - Desktop software
 - We are new but already got many clients
 - Updates requires about 15-30 mb.
 - Update process is fairly straight-forward
 - Q/A is out of the question in here, I assume the updates are almost always delivered perfectly (*for the sake of argument let's say there is only 4% chance of delivering an update with a bad bug*)
 - Subscription model (*we charge every year and includes all minor, major updates*)


**Question**

 - Do you think releasing a new version every week is a good idea or twice a month?
 - Shall we change our release cycle? Could this make our customers frustrated or happy?
 - Any experience that you can share? Maybe some hard data on the subject.




## Answer 7621

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-02-04
- score: 9

Our flagship product has similar characteristics.  We've found with some tuning over the last year that releasing more often than about once every 6 weeks is counterproductive.  When we've had updates that were closer together we saw that people generally didn't track with our updates (they kept their older version).

 - Users don't appreciate each release as much because there isn't always something in it for them; with larger releases we make more headway across the entire product so people nearly always find something compelling in what we're doing.  **This can lead to release fatigue** where your customer impression is that your application isn't stable (in more ways than one - stable meaning you have to patch it, and stable meaning they know what it does)
 - **We spend a disproportionate amount of our time converging.**  This isn't just a matter of testing and QA; it gets into all the little things you do to make sure something is really production grade like documentation, updating our samples, updating our product web site.  There's overhead to these tasks even when there are just a few small changes (e.g. they only scale down so far)
 
We've been shifting to more of a once a quarter cycle and doing more in each release.  The initial feedback on this has been very good - customers like the predictability and it's made conversations easier with folks about future enhancements (they know we don't just ship whenever so the earliest opportunity is the next quarter).  We have the time to keep our marketing message together and have a more natural communication cycle.

This timing has also allowed us to introduce a public beta cycle - we do a "preview" builds as necessary for people that are just itching to get the latest thing, knowing that it isn't complete (documentation not reviewed, subject to change, etc.) which keeps their excitement up without creating a support burden for us.  On a three month cycle between releases we like to have a preview build out at about the two month mark.  


## Answer 7648

- posted by: [SmartCompanySoftware](https://stackexchange.com/users/-1/1629-smartcompanysoftware) on 2010-02-05
- score: 1

People who are 'technical' love freuquent updates, but most people are not 'technical'. Your users are simply that, people who use your software. They won't care if you've increased the speed of a method by a factor of 4. They do care about the software working and being stable. They will see the benefit of new features, but they still have their job to do and when they find time, they might upgrade.

Think of it this way: If you bought a car from Ford and then every two/four weeks they called you and told you to bring the car to the dealer for a 5 min upgrade, how long would you put up with this?


## Answer 7624

- posted by: [Abdu](https://stackexchange.com/users/-1/2029-abdu) on 2010-02-04
- score: 0

<p>Releasing early can hurt. When I build a new website, I make sure it has enough features to make most customers interested. Because you don't get another chance to make a good impression. If you released early and most people weren't interested, you lost them. Most probably they won't come back to check again. There are already too many other choices in the market and they have probably went with your competitor. <a href="http://answers.onstartups.com/questions/7560/sooo-many-startups-coming-out-everyday-is-the-web-market-getting-saturated" rel="nofollow">See my other post</a>.
Also those people might be talking negatively about your incomplete product. Really bad. Because the web keeps text forever and people might not make the connection that that's already old news (being in the future now when final is released). So be very careful.</p>

<p>Releasing often is not a bad idea as long as you don't change the UI suddenly, for example, that people get lost and frustrated. If these are bug fixes and gradual enhancements, the better.</p>

<p>Personally I love frequent updates. I download a new nightly beta build of Resharper5, a Visual Studio plugin, almost everyday and I use it all day long everyday. I do this so that I get the new features and bug fixes. And  so that I can help the development team with the bug reporting and feedback. Eventually I want a solid software when it comes out and I want to be part of it and it has the features I want.</p>



## Answer 7641

- posted by: [Doug G](https://stackexchange.com/users/-1/2107-doug-g) on 2010-02-05
- score: 0

I tend to think of that mantra as applying more to Web Applications than to stand-alone desktop applications.  I know with products like iTunes its annoying as @#$% everytime it makes me lose 5 mins of my life installing some new release with no new obvious features.

Quarterly release sounds like the right timeframe, however you can offer an option for users to pull down mid-cycle releases as long as it has a clear set of release notes so they can determine if its worth their while.

Best of Luck,
Doug


## Answer 7645

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-02-05
- score: 0

Yes, release early, but release as Beta software.

While it is beta software, update it often. Add the features and improvements and bug fixes, and release whenever there is something that makes the upgrade worth everyone's time. As beta software, that could be as often as every week or two. As a beta, encourage customer feedback and make the fixes and consider the suggestions your users offer.

Once you get to a point you feel your it is worthwhile to start full-fledged marketing, then release Version 1.0.  At that point, stop the fast releases. They are not expected nor wanted once a full release is out. People want stability. Now only update for or major features (a .1 release) or major bug fixes (a .0.1 release). Feature releases should not be more often than once a quarter. Don't annoy your customers at this point. 





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
