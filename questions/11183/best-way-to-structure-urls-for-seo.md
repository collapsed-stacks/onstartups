## Best way to structure URLs for SEO?

- posted by: [Michael](https://stackexchange.com/users/-1/2774-michael) on 2010-05-14
- tagged: `seo`, `google`
- score: 2

I am creating a service that help users connect with local vendors in a certain niche.

Each vendor currently has a URL in the form:

    http://example.com/vendor/<id>/<vendor-name-slug>

For example:
http://example.com/vendor/5839/the-widget-store

It was suggested to me that it would be better to structure the URLs in this form:

    http://example.com/<vendor-name-slug>/<geographic-location>/<id>

For example,
http://example.com/the-widget-store/nyc/5839

The argument being that a likely Google search would be "the widget store nyc", and the restructured URL would more closely match the search term.  Also dropping the "vendor" part of the URL to make it shorter - although for this I would argue it would also give Google the information that the link is about a vendor.

Is there anything to this, or is it merely nitpicking (i.e. bikeshed problem)?

(By the way I'm new to this site but I love the content and community and hope to be able to contribute at some point.)


## Answer 11186

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-05-14
- score: 5

You will have to look at your inbound traffic from search engines. Do your end users often include location in their searches, or not? If yes, then having the location as part of the URL will help.

Depending on your web framework, it might be best to have the most significant information at the root of the URL structure, i.e.

    http://example.com/<id>/<geographic-location>/<vendor-name-slug>/

Remember to be consistent with uppercase / lowercase letters in the URLs, and trailing slash or not.


## Answer 11215

- posted by: [Griftastic](https://stackexchange.com/users/-1/3446-griftastic) on 2010-05-16
- score: 1

Since the geographic location is key, put it in the url and toss the vendor name.  I'd place the id number either at the beginning or the end, with rules in place to re-direct to something else if the url gets garbled.


What I do for a lot of wordpress sites is this:

    http://www.example.com/<post number>/<title of page>/
So it comes out something like this:

    http://griftastic.com/42/problems-with-this-ad-acai
So if the actual page title gets garbled, cut off, or changes, the post number (42) makes sure the right post gets seen.  This has prevented a lot of 404 errors for me.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
