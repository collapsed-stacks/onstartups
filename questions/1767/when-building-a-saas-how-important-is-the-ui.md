## When building a SaaS, how important is the UI?

- posted by: [Arman Arami](https://stackexchange.com/users/-1/425-arman-arami) on 2009-10-17
- tagged: `b2b`
- score: 7

When asking this question I am more concerned about the UI at the time of launch. When you first release the product to be used/tested by the general public.
By importance of the UI I am interested in two things.
 
- How important is the information architecture of the UI? Modeling and Flows
- How important is the look and feel of the templates/screens?
- And lastly I am wondering if you would or would not launch the product if any of the above (modeling and flows or look and feel of the screens) is lacking?

Now please keep in mind that I have heard both sides of the argument:

 - Image is everything and the first
   time you launch a SaaS product if the
   audience can not interact with it and
   find things easily or if they don't
   like it, they are gone and won't some
   back.
 - You should release the product
   and let the audience/users tell you
   what they need and fix things as you
   go along based on the users needs.


## Answer 1770

- posted by: [Micah](https://stackexchange.com/users/-1/284-micah) on 2009-10-17
- score: 10

I'm in the launch early and iterate camp.

That being said, looks are waaaay more important than features in my experience. If it looks terrible, most people won't bother to learn the features. However, if it looks good but lacks features, they will beg for you to add the features they want.

So, I would say: launch with less features, but make everything look good. Perfect navigation isn't necessary, nor is perfect workflow. However, a little bit of CSS and imagery will make your app pop and make a huge difference in first impression.


## Answer 1774

- posted by: [dharmesh](https://stackexchange.com/users/-1/4-dharmesh) on 2009-10-17
- score: 2

It depends a lot on the market and target audience.

If it's a consumer-focused site, the UI/UX likely counts for a lot (think Mint).  If it is a B2B market, then it may not be as important.

I'm also in the camp of release early, release often.  Keep the early design simple, focus on the actual problem at hand, and iterate based on what you learn from your users.  In the early days of our product (B2B), the design wasn't very good, but users did not seem to care that much.  When we asked them what they wanted from us, it was always focused on features/functionality -- not design.


## Answer 1778

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-10-17
- score: 2

The only thing to do early is make sure the "view" and "everything else" is split up.  That way it can start as ugly as necessary and get pretty later.

Although that's also not completely true, because things like "updating in-place" or "live updates" and other AJAX-y concerns often need to be architected rather than spliced in later.

Still, I'd rather have a non-AJAX application that people are starting to pay for than a fancy application that no one wants to use.


## Answer 1782

- posted by: [Daniel Crenna](https://stackexchange.com/users/-1/772-daniel-crenna) on 2009-10-17
- score: 2

I'll add that a lot of the time, SaaS applications spend a lot of time perfecting the UI of the front door, i.e. your web site tour and call to action pages. Then, when the user finally commits money to use your service, the backend admin area is an uninspired, tabs + sidebar affair that they stole from Basecamp.

Essentially every SaaS backend is the same. You can launch early with a pretty home page and a sparse back end, and iterate on that, but consider making the admin area really shine to retain the customers you managed to capture from your front door.


## Answer 1787

- posted by: [Neil Davidson](https://stackexchange.com/users/-1/210-neil-davidson) on 2009-10-17
- score: 2

It depends what you're trying to do. The following holds for desktop applications too.

In general, if you're solving a really, really difficult problem, are fixing a real pain for your customers and have few competitors then your UI can, frankly, suck. Your customers will make the effort to use your product since its potential is so huge. It doesn't matter if the workflow is awkward or the colours clash - your customers will love you because you've fixed their problem.

If you're not solving a useful problem, or if you've got a lot of competitors, then you need to reduce the friction as much as possible and make your UI as good as you can.

It can often be more important to get the functionality right before the usability. As Doug Engelbart (the inventor of the mouse) said, "If ease of use were the only requirement, we would all be riding tricycles".



## Answer 1812

- posted by: [pbreit](https://stackexchange.com/users/-1/239-pbreit) on 2009-10-18
- score: 2

The more unique the offering, the less important the UI since your differentiation is being driven more by the service itself. However, if your service is similar to several others, you will need to differentiate more on the UI.

Pick the minimum feature set necessary to have a viable offering, put a good UI on it and iterate.


## Answer 1772

- posted by: [Yakov Fain](https://stackexchange.com/users/-1/691-yakov-fain) on 2009-10-17
- score: 1

Unless you are planning to offer yet another search engine, simplistic UI won't cut it these days. Hire a professional designer. It's better to limit the scope for the first release but the views must be eye candy. It's getting even more complicated - just hiring a professional Web designer that spent 10 years creating Web 1.0 sites only is also wrong. Find the one who can show you some RIA that s/he created. Do not cut corners in the UI tier.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
