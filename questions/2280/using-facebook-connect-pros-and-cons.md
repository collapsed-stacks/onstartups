## Using Facebook Connect - Pros and Cons

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2009-10-23
- tagged: `facebook`, `marketing`, `website`, `sales`
- score: 7

is Facebook Connect worth the efforts? any benefits in long term? are there any negative consequences like slow page loads and increased page download times etc?

**Update:**

Okay so I just tried Facebook Connect on http://www.huffingtonpost.com/ and it impressed me with the functionality. However, being a new user, I also found interface a bit clumsy and complicated.

Viral loop, branding and competitive advantage points are well taken. Looks like it adds value to both FB and independent websites.

But apart from sharing updates and fetching user info. What else is possible?

Can any one share their success stats like increase in page-views/visits etc...

**Update 2:**

Facebook has introduced a new home page news feed that only shows popular items. Probably this change affects the viral loop. Comments plz?


## Answer 2299

- posted by: [Adam Webber](https://stackexchange.com/users/-1/1027-adam-webber) on 2009-10-23
- score: 9

Using Facebook Connect and now we're seeing more Twitter Connects accompanying the Facebook option is a very good option. The point is take all the barriers to entry away from your potential users. 

1. Easy to remember: Users don't want to have to remember 12 different passwords, one for every site, so giving them the option of quickly logging in with their FB or Twitter profiles seems like a very convent step. 

2. More viral: You benefit because users on their network are now seeing that their friends are using your website and they will want to come too. 

3. Competition: If you don't offer it, you leave your competition the ability to try and convert your users by offering them the option to login quicker and more efficiently.   



## Answer 2308

- posted by: [Micah](https://stackexchange.com/users/-1/284-micah) on 2009-10-24
- score: 8

<p>Since everyone has highlighted a lot of the good stuff, I'll play devil's advocate here.  I've spent a year developing Facebook apps, so I know a little about this stuff.</p>

<p><strong>Fast Pace</strong></p>

<p>Facebook moves very fast when it comes to making changes and obsoleting things.  What works today might not work tomorrow, and most certainly won't work in a year.  So, unless you keep tabs on what they're doing and what has changed recently, your FB Connect login may break silently and new users won't be able to sign up. It's not impossible to keep up, but it's yet another thing you have to check every now and then to make sure it's still working. They might be more careful with FB Connect than they are with the app platform, but who knows?</p>

<p><strong>No True Emails</strong></p>

<p>Someone please correct me if I'm wrong, but I don't believe you get a true email address for FB Connect users.  Instead, you get an FB proxy email.  This means that Facebook will always sit between you and that user when you try to communicate.  Having such a giant, uncaring monolith between me and my users makes me uncomfortable.</p>

<p><strong>TOS Quicksand</strong></p>

<p>Facebook has no fear of modifying their terms of service, sometimes drastically.  So, even if you read all the FB Connect fine print, there's no guarantee that it will still apply in a week or a month.  You could sign up ten thousand FB users, then have FB change their TOS in some way that makes your entire site a violation, then they shut off your access to FB Connect, stranding you.  Granted, it probably won't be this drastic, but just look at the <a href="http://en.wikipedia.org/wiki/Facebook%5FBeacon" rel="nofollow">Beacon debacle</a>. A lot of 3rd party code immediately stopped working when they (thankfully) shut Beacon off.</p>

<p>Now I'm not trying to say that you shouldn't use FB Connect.  I'm just trying to emphasize that FB Connect is not all kittens and unicorns.  Remember: Facebook has their own agenda and will continue to pursue it, regardless of the positive or negative impact it has on your particular site.</p>



## Answer 2496

- posted by: [James T](https://stackexchange.com/users/-1/1139-james-t) on 2009-10-26
- score: 2

It is likely that facebook will support openid as a provider in the near future. 

With that in mind, concentrate on OpenID. When facebook gets around to it, you'll suddenly have all their users, but unless you're launching this minute, you'll waste a lot of time and effort to integrate something that will be obsolete in 6 months.

This site does it well... Giving users popular buttons to sign in with is easy, while still retaining the openid backend that allows people from all over the web to sign in.


## Answer 2297

- posted by: [user161](https://stackexchange.com/users/-1/161-user161) on 2009-10-23
- score: 1

I think the benefits of having 300 million users able to login with a single click is pretty compelling.

Load times are not affected much if you load the javascript at the bottom of your <body> tag.  This will break html validation of course, but thats a small price to pay in my opinion.


## Answer 2303

- posted by: [Manuel M](https://stackexchange.com/users/-1/1085-manuel-m) on 2009-10-24
- score: 1

Further comments, following Adam, above: 
Using FB Connect is valuable in a number of ways:

- it gives your site something of a "brand halo" from FB - your integration with it looks positive to many end users.
- it doesn't affect your site performance at all, unless you are pulling back lots of data. We implemented a project that read a lot of FB data, and initially made the mistake of pulling down records one-by-one - took forever, but once we switched to loading in bulk, it was fine.
- Some sites use the integration really well (look at Huffington Post at http://www.huffingtonpost.com/ for a well-done integration) - if you have the need and dev cycles to put it together, it adds a ton of value.

Downsides? If there's no compelling use case, your site can look a bit like a "me-too" player. As the FB API evolves, you may have to keep pace with what they are doing, but that's not a big issue in my mind.


## Answer 2359

- posted by: [Justyn](https://stackexchange.com/users/-1/605-justyn) on 2009-10-24
- score: 1

The biggest downside in my opinion is not capturing your users email address. However, if your business doesn't rely heavily on email marketing or converting customers (such as a blog), it's not a big deal. If eyeballs are your goal, FB Connect is a no-brainer. If you sell something, think twice. In most cases though I think the potential of the network and ease of use for your customer will win out.


## Answer 3350

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-09
- score: 1

One huge con is that you dont own the user's data and can only use it when they are logged in or you ask them for specific offline access to their data.


## Answer 3338

- posted by: [Joe A](https://stackexchange.com/users/-1/60-joe-a) on 2009-11-09
- score: 0

<p>FYI Facebook will start sharing user email addresses through their API.</p>

<p><a href="http://developers.facebook.com/news.php?blog=1&amp;story=326" rel="nofollow">http://developers.facebook.com/news.php?blog=1&amp;story=326</a></p>



## Answer 13952

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-08
- score: 0

this con is to be very carful to who your friends with there was a facbook killer a 17 year old girl accepted his reguest they met up at her house he raped her and stargled her to death, when her mother got home she was just barly alive! so their security SUCKS.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
