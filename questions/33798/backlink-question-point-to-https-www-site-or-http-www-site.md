## Backlink question - point to https://www.site or http://www.site ?

- posted by: [Dmurtagh](https://stackexchange.com/users/-1/12396-dmurtagh) on 2011-12-16
- tagged: `seo`
- score: 0

When getting backlinks, should I point them to https://www.site.com or http://www.site.com ? for reference, when someone goes on my site by typing in http://www.site.com or www.site.com they get redirected to https://www.site.com. Also, please note that all pages on our site have a secure 's' in them, example https://www.site.com/blog

thanks




## Answer 33859

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-12-18
- score: 1

If you are always going to have HTTPS running on your site I would build up all your links using HTTPS. I assume if someone hits your homepage your web server, htaccess or some script is forcing it to HTTPS, this typically results in a permanent 301 redirect. So in theory the search engines should recognize that and be OK with it.

BUT - at least in the past search engines looked at http and https as separate sites. 

I would link to the HTTPS page for consistency and so all incoming responses don't have to have a 301 redirect sent to the browser and sent over to the new page.

That is if your site is always going to be 100% https for all URLs. **Then just link to that.**



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
