## Can I work on my SEO and have my web site "invisible"?

- posted by: [Spiro](https://stackexchange.com/users/-1/2232-spiro) on 2010-06-09
- tagged: `seo`, `website`
- score: 4

Here is a kind of confusing :) web site/SEO newbie question. I was looking for answer everywhere, but it is hard to find the one I was looking for.

The question:

Since my product is still not ready for promotion, but would like not to waste time and work on SEO for my web site, is it somehow possible to have my site promoted, but in the same time "not visible" to outside world? Should I put some "coming soon" home page, or redirect the trafic to some other place (Google, Bing.. where), or...? Can I effectively apply to directories, make backlinks, and completely work on tuning SEO, without accepting visitors to ANY of my pages? Will crawlers recognize and succesfully promote contents of site like this, and will all my SEO efforts work the same as if I have site visible?

What are your suggestions, experience, recommendations? What's the best way to do this?

Thanks in advance for your time and your answers! 


## Answer 11921

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-06-09
- score: 8

Well, I'm not so certain I understand exactly what you'd like to accomplish, but here it goes:

1) if you don't want any search engines to crawl and index your site, then put a file called "robots.txt" in the root directory with this in it:

    User-agent: *
    Disallow: / 

people can view the site, but search engines will not index your site.  

2) If you want only a select few people to access the site while it is being "built", then password protect the directories.  On a typical linux host, here's how you do that:

a) create a .htaccess file in the root of the website containing:

    AuthName "Members only in here"
    AuthType Basic
    AuthUserFile /path/to/your/.htpasswd
    AuthGroupFile /dev/null
    require valid-user

b) use the utility htpasswd (in the directory you want to create the .htpasswd in) like this:

    htpasswd -c .htpasswd username 

(for the first time only. remove the -c if you want to add more users) 

----------
Now, remember that if you are building backlinks, the backlinks *need* to go somewhere, so you may not be getting any benefit from your linkbuilding (or approval from partners) unless the site is live. If crawlers cannot reach the destination, or see a robots.txt exclusion in the destination, then they likely will not include the link - and have no positive impact on your effort.

Better to create a coming soon page that is visible, create the production site behind a password protected other site with no indexing, then move the completed production site over when ready.


## Answer 11953

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2010-06-10
- score: 4

I don't get it. You want to attract traffic to your site without having a site? Why?

More importantly... why would a search engine ever want to point to you if there's nothing there yet? They would be sending their searching audience on a wild goose chase. Search engines don't like to do this, because it makes the search engine look bad.

Start a blog. Talk about things that are important to your eventual customers. Maybe people will find the blog, and follow it. Then when you have something to announce you'll have some readers who care.


## Answer 11941

- posted by: [Lizeth Gomez](https://stackexchange.com/users/-1/3623-lizeth-gomez) on 2010-06-09
- score: 3

It sounds as though you want to promote your website while it is being built. Your best bet would be to create a "Coming Soon" page to direct users to while keeping your dev site offline. Also, as far as I know, if your page is not published and public, search engines cannot index it. 

However, I will say, this has the potential to annoy your potential clients if they search for something only to wind up at a "Coming Soon" page. If your site is not a 6-month project, I would simply complete the site and allow it to be indexed, and searched for after completion. 


## Answer 12908

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-20
- score: 0

Yes you can do this. A great example I was looking at just today is Blekko.com. They have done a lot in terms of PR and have been covered on seobook and techcrunch as well as other sites. You'll also see they are leveraging this traffic to get more word of mouth (if you want an invite to the private beta you have to follow them on twitter and tweet to them or fan them on Facebook). This is a great way to start building links as well as get a list of excited customers waiting for the launch, so your new product can start with a bang. 

I wouldn't think reputable directories would accept a coming soon page but if you have a good enough service you can still get links in ways I mentioned above.

Hope this gives you some ideas.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
