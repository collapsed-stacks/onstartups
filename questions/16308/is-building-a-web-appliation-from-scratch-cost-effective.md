## Is building a web appliation from scratch cost-effective?

- posted by: [Alex](https://stackexchange.com/users/-1/4951-alex) on 2010-11-10
- tagged: `software`, `development`, `costs`
- score: 3

I am trying to find the most cost effective approach to building a web application based in PHP. I want to know if using a PHP Framework such as, [Social Engine][1] would be best to avoid having to avoid coding the monotonous Account Settings, Privacy Settings, Account Creation, Log in, Log out, etc.


The reason I am asking is that I have a coder that is currently building a web application for me, but, I think that he wanted to start from scratch and build out the shell of the site (Account Settings, Account Creation, Email Authorization, Privacy Settings) just to bill more. In hindsight, this could have been accomplished by just buying something like [Social Engine][2] and then customizing the specs of the project onto it.

**It's a social application, dealing with friends and status' and facebook "like" buttons. Is it difficult to grab the raw code, that's already written, and transform it and customize if how I want instead of starting completely from scratch?** Is this really the most cost-effective approach?

It seems like he's trying to build a car by hand, and started welding the frame, because I wanted to order a custom car with a different radio, and nicer seats. Just yank out the seats and radio and stick in new ones? Don't build the entire car from scratch. Am I wrong?


  [1]: http://www.socialengine.net/
  [2]: http://www.socialengine.net/


## Answer 16313

- posted by: [xiaohouzi79](https://stackexchange.com/users/-1/4868-xiaohouzi79) on 2010-11-11
- score: 2

<p>If you've hired anyone worth their salt they would be willing to discuss this in detail with you and the best time to discuss this is before any code has been written.</p>

<p>It may be that your idea doesn't require too much in the way of coding and it may better built from scratch. This all depends on the scope of the project and not something that can be determined just by listening to the description.</p>

<p>If your application does require a lot of different components: auth handling, database work, form handling etc. it may be good to use a framework. The benefits of a framework are added security, reduce repetitive programming for common tasks and many built in security features. (Note: I just had a look at SocialEngine, I've never used it from experience, what I am referring to as framework is something like <a href="http://cakephp.org/" rel="nofollow">CakePHP</a> or <a href="http://codeigniter.com" rel="nofollow">CodeIgniter</a>).</p>

<p>The good news is, it's not too late. You won't necessarily need to chuck everything out if you move to a framework. If you are only part way through the work you can move things across.</p>

<p>Be aware that the guy you have hired may not have experience with frameworks. This will become an issue if you try to discuss this with him/her as they will likely discourage you from using one. In which case you may have to ditch your current developer.</p>



## Answer 16315

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-11-11
- score: 2

There's an old adage among programmers: **"A lazy coder is an efficient coder."**

In other words, don't write anything you don't have to.  There is a lot of code out there under open source licenses that will do at least some of what you need.  The benefits of building on an open source foundation are many:

 - You don't have to re-invent the wheel. (Thus the cost of initial development is lower.)
 - Your maintenance overhead is lower, because the open source parts are constantly maintained by the community.
 - Open source components are usually more secure than closed-source components, because they are seen and tested by more people.

Note that I have not yet addressed closed-source frameworks such as the one you mentioned.  I would *never* build on one.  When you build on a closed-source foundation:

The pricing and license terms can change at any time, so you are at the mercy of the seller should you ever want to:

 - Sell your web site.
 - Add domains/subdomains in a site re-organization.
 - Upgrade to the next version.

*and* you are usually completely prohibited from:

 - Modifying the source code (if you can see it at all, and if you can't you should be concerned about security).
 - Licensing your platform to others.

*and*, if the supplier of the closed-source component goes out of business or simply decides not to produce the product any more, you are left completely re-developing your product on another platform, because you cannot legally maintain the closed-source component yourself.

There are plenty of open source products you could use, and avoid all this risk.


## Answer 16316

- posted by: [cfrech](https://stackexchange.com/users/-1/5331-cfrech) on 2010-11-11
- score: 2

To reiterate some of what's been said and add another perspective:

If the site is truly being built "from scratch" then no, in almost any case that's not a cost-effective approach.

But there's a chance your developer is using a framework or libraries or at least code he's already written to assemble the "frame" (a good analogy).

If not, I'd definitely be concerned. (Incidentally, not to split hairs, but the example you mentioned looks more like a full-fledged content management system [CMS] than a framework.)

My advice would be to have a conversation with the developer to better understand why he took the path he did.

If he's not using a CMS because he doesn't know how or isn't aware of one that would fit your needs, that's definitely pause for concern.

There are, however, cases where a custom platform is appropriate, depending on how much flexibility you need and how unique your product/service will be. Custom solutions, done right, give you everything you need, and nothing you don't.

Do be aware of the "hidden" costs in developing a custom platform. The beauty of going with a CMS like Drupal is there are lots of other Drupal coders out there who'd be happy to work on your project. If your current developer goes away, will he be the only one that knows the system he's created? (Be sure, if nothing else, he's providing decent documentation.)

And, unless he really knows what he's doing, he could be introducing security holes into your site. Authentication and login systems MUST be built with security top of mind. Again, an issue to clarify with the developer.

Bottom line: It's not too late to switch, and the costs you've incurred so far may not be the worst of it (in light of the above). Make sure you've evaluated all your options, including open source CMS solutions like Drupal and Joomla. And be open to the idea that, done right, the custom route may indeed make the most sense.

Good luck.


## Answer 16314

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-11-11
- score: 1

Depending on your requirments and temperment, Social Engine may be cheaper for the 'shell' of the application, but very costly or impossible to implement the other features. You may want to consult someone who has built apps on this platform covering a higher percentage of your needs. 

If this person is not familiar with Social Engine, you may have to pay him/her to get up to speed. Installation on your server may not be free from problems. Also, there seems to be some extra expenses for all the Add-ons. Otherwise, find another PHP developer with Social Engine experience.

Some people have very specific expectations and are accustomed to getting them met. When you buy off-the-rack, you may like the 90% fit, but for a perfect fit. You can hire a tailor to let out the waist, but if you want to replace the lining in the jacket and make the pants longer...$


## Answer 16475

- posted by: [Adrian Schneider](https://stackexchange.com/users/-1/4434-adrian-schneider) on 2010-11-14
- score: 0

As one of the guys who almost always builds things from scratch, here are some reasons in favor of it:

1. Your company owns the source code, and has full legal control to do what you want with it.  We try to develop all our projects as software we can re-use and re-sell to the masses.  Even if you only sell the entire business one day, make sure you can legally do so.

2. Building from scratch gives you a lot more architectural control.  Many free web apps are horribly written, or even if they aren't, if they don't meet all of your architectural needs, you will be fighting it non-stop trying to make changes.

3. It's a great learning experience.  People learn by doing.  Sure, reading others' code is always very beneficial, but if you never take on lead to any projects, you are limiting yourself.

Now, to clarify... I wouldn't recommend building it entirely from *scratch*.  Use some sort of framework to take care of all the low-level stuff.  I recommend Zend Framework for complex PHP apps.

Building things this way will likely be much more expensive and timely early on.  However, the long term cost could go either way.  If this is a major concern, and he hasn't earned your confidence, then perhaps using pre-existing software is the way to go.

Hope this provides a little insight. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
