## Web Analytics: Identifying referral traffic from sites on HTTPS

- posted by: [webbie](https://stackexchange.com/users/-1/16413-webbie) on 2012-03-28
- tagged: `analytics`
- score: 2

As Google, Facebook, Twitter, and other sites implement https the referral data in analytics tools is becoming less accurate, e.g. HTTPS traffic comes with a blank referer and appears as   direct traffic. 

How big of an issue is this for you as a business owner or marketer and how do you work around this issue? Does anyone have any insight into how companies in analytics space are dealing with this issue and if there is any hope?

p.s. I got a spike in "direct" traffic the other day against seasonal pattern and it's really annoying to not be able to tell where the extra clicks came from.

EDIT: Yes, I understand that HTTP_REFERER is what's missing and understand the technical limitations. Since we (site owners) can't make big sites pass extra info to us via URL parameters I was wondering how others are dealing with this. 


## Answer 37680

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-03-29
- score: 2

The analytics and statistics package look at something called the HTTP_REFERRER, and that is passed from page to page as you click around a site or to other websites. Every page loaded there is a field passed HTTP_REFERRER of the page prior.  

However, this field is not passed when the user is on a secure https site and goes to another website or goes to a page on the same site that is not https.

It's a big pain in the but in the analytics industry right now and has some of my custom 'conversion' metrics all messed up.

The only solution to this is if Google passes some new field in the URL in the future when they pass the visitor to your site like they do with Adwords.  I'm not sure if Google will do that though.


## Answer 37679

- posted by: [Salmon](https://stackexchange.com/users/-1/5445-salmon) on 2012-03-29
- score: 0

<p>The issue is not HTTPS, the issue is referral URL. 
There's no way around it, because you only have <a href="http://en.wikipedia.org/wiki/HTTP_referer" rel="nofollow">HTTP_REFERER</a> when the user gets to your page and that's what Analytics packages use. 
Cookies will also not work here since it's a different domain. </p>



## Answer 48625

- posted by: [nutcracker](https://stackexchange.com/users/-1/25896-nutcracker) on 2013-04-17
- score: 0

This is somewhat outside the control of the receiving website. Your best bet is to go https on your website and then the referrer header will be passed along as normal from both http and https websites.

If you're running on https and want your outbound links to include a referrer on http sites then it gets tricky. 

Facebook is using https and is getting around the issue by using some sort of redirect via a server running http. From a [zdnet.com article](http://www.zdnet.com/blog/facebook/stumbleupon-passes-facebook-in-us-referral-traffic/2902):

> "Although Facebook are allowing https, they are also now running
> referrals through a non-https redirect which allows us to track all
> the referrals," a StatCounter spokesperson said in a statement.
> "Essentially instead of a user clicking a link and going from
> [https://facebook.com](https://facebook.com) to a third party site, the user goes from
> [https://facebook.com](https://facebook.com) to [http://facebook.com](http://facebook.com) to the third party site. As the
> user is NOT going directly from a https site to a third party, the
> referral can be tracked."

I'm not exactly sure how they are implementing this but I'm keen to find out for my own https site.

It might also be possible to add utm_source, utm_medium and utm_campaign parameters to all outbound links from your https website so that receiving website can use google analytics to extract the referrer from these values.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
