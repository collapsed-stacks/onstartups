## How to redirect to another website with tracking?

- posted by: [Chris](https://stackexchange.com/users/-1/412-chris) on 2011-04-29
- tagged: `marketing`, `website`, `analytics`
- score: 3

Our website promotes a web-based application that's actually on another site (in the ebay.com apps center). When someone hits the "sign up" button on our website, it implements a redirect as it takes that visitor to eBay's apps center to actually sign up for the product. We do that so we can pass information to Google Analytics about the source of those individuals. So i can tell X people from SEM clicked over to the eBay Apps Center and Y people from a banner ad clicked over, etc. Otherwise all source information is stripped out as they go through ebay.com.

The question (finally) - this redirect takes 5 seconds which seems like an eternity. Is there any standard for doing this type of redirect implementation that perhaps we're not doing correctly?

Any help greatly appreciated,
Chris


## Answer 28153

- posted by: [Will Ko](https://stackexchange.com/users/-1/12272-will-ko) on 2011-07-31
- score: 1

Bit.ly tracks link redirection analytics.

You can also try embedding your target site wrapped in an iFrame with the main HTML still retaining your tracking codes.


## Answer 30787

- posted by: [Brian Karas](https://stackexchange.com/users/-1/8465-brian-karas) on 2011-09-29
- score: 1

If you're doing the redirect with Apache rewrite rules, then look at the "RewriteLog" settings.  You can log apache redirects to a file, which you would then later parse to get details on the redirects you served up.

The redirects should be almost instant, I don't know why they are taking 5 seconds.

If the above isn't helpful, tell me how exactly you are doing the redirs and maybe I can think of something more specific to your application.



## Answer 33378

- posted by: [Anagio](https://stackexchange.com/users/-1/14857-anagio) on 2011-12-06
- score: 1

Try event tracking in analytics if you are not already it may be quicker than your current method of tracking. And is the redirect happening client side or server side? I would use server side header redirect on click of the signup button. Or post the form with AJAX and redirect the visitor maybe the form loading is taking longer to complete?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
