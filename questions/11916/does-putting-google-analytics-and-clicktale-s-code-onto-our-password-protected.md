## Does putting Google Analytics' and Clicktale's code onto our password protected Alpha site expose the content?

- posted by: [Warren E. Hart](https://stackexchange.com/users/-1/2058-warren-e-hart) on 2010-06-09
- tagged: `analytics`, `google`, `website`, `launch`
- score: 0

We are launching a new site this summer and will have the Alpha version available shortly. We'll be testing this privately with a small group of trusted people before we do our public launch. To maintain the confidentiality of the site before launch, each tester will have a unique password that we'll change frequently.

We'd like to use Google Analytics and Clicktale to assist us in our testing and want to understand the risks of putting their code onto our site. On one hand, it appears that they don't actually crawl our content. On the other hand, there are concerns that their employees could have access to our site content and could use this in inappropriate ways.

It appears from both sites that they don't actually crawl the content but I'm wondering if anyone has insights into the real story here. 

Is this a risk? Should we wait till after we launch publicly to insert their code?

Thanks.


## Answer 11918

- posted by: [Stefanos Tses](https://stackexchange.com/users/-1/3178-stefanos-tses) on 2010-06-09
- score: 1

I can't imagine Google employees will care looking at your site's content. Why get into the trouble look at a site that they know nothing about? Is not like the next apple.com beta site...

Let me ask: why all this secrecy?  
If you afraid so much that someone will steal your idea don't enter the google code, until you move it to production.

I can't remember where I read that but I think is relevant:  
"If you want to confuse your competitors, give them ... your source code". 8-)


## Answer 11923

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-06-09
- score: 1

<p>IF you desire analytics on a pre-launch basis, why not just run something like <a href="http://piwik.org/" rel="nofollow">piwik</a>?
No one will have access to the data but you and your hosting environment..</p>



## Answer 11964

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-06-10
- score: 1

Don't know about Google analytics, but ClickTale employees don't have access to your account or webpages. I've used them in the past, and they've always had to ask me for my password for accessing my data, as they couldn't access it without it.

Just looked at their wiki, they also have the option for off-line recordings if you're going to be testing a website: http://wiki.clicktale.com/Article/Offline_recordings.




## Answer 11969

- posted by: [Mike Lee](https://stackexchange.com/users/-1/3589-mike-lee) on 2010-06-10
- score: 1

I don't know about ClickTale (though JaC0b looks like he's got that answer), but for Google Analytics, they do have to crawl your site to make sure the JavaScript beacon is installed. However, this won't trigger a site-wide crawl. They'll look at just your homepage to check for the beacon, and that's about it.

There's a possibility they'll crawl more, but it's very low. Most people have a problem trying to get Google to crawl them, so I don't think you need to worry.

Also, they can't provide data on password-protected pages. I doubt ClickTale can either.

There may be other solutions. If you want to get general analytics data during the Alpha, piwik (like jimg said) can work. It's a self-hosted solution. You can also track each user, since you're assigning each individual with a unique password.

If you're placing this code so you're ready for production, I'd say just wait until the production launch. Otherwise, you'll muddy the analytics data with test users and not real users.

I hope this helps. Good luck.


## Answer 11917

- posted by: [Michael](https://stackexchange.com/users/-1/329-michael) on 2010-06-09
- score: 0

I suggest you ask this over at google analytics support (http://www.google.com/support/analytics/) or a related forum. The question pretty off-topic for this community.

Good luck!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
