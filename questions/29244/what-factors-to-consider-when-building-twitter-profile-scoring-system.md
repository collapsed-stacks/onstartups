## What factors to consider when building twitter profile scoring system?

- posted by: [Safran Ali](https://stackexchange.com/users/-1/12811-safran-ali) on 2011-08-25
- tagged: `twitter`, `profile`
- score: 1

I am considering building a startup that provides a user with twitter profile score i.e. how good is someone twitter profile before someone follow them. I have basic consideration about what factors to involve, like:

 - followers a profile have
 - how many people they following
 - tweets per day
 - tweets quality
 - re-tweeting of their tweets
 - how good is their profile i.e.
    - does it include description?
    - profile age
    - does it have picture in it?
    - do they provide url in their profile description?
    - do their page include a background image?

these are the basic criteria I came up with but I am pretty sure that's not enough, it's ok to build the basic tool but for building an extensive profile scoring it requires extra. So I was wondering that anyone provide me with what extra attribute should i consider to build a really good profile scoring site for twitter user?


## Answer 29246

- posted by: [Lloyd S](https://stackexchange.com/users/-1/12549-lloyd-s) on 2011-08-25
- score: 3

The first thing I would consider is how is the service you are offering going to be any better than the available options:

- http://klout.com/corp/kscore
- http://www.twitterscore.info/

Your above seems pretty complete in terms of data you can glean, you could probably do with weighting frequency of updates of followers/following,


## Answer 29282

- posted by: [Tom](https://stackexchange.com/users/-1/12953-tom) on 2011-08-26
- score: 3

The question is how're you going to monetize this? I've often thought of creating something similar for free, which gives users a badge they can put on their website or blog, and that they can tweet about. The aim would be to promote a paid Twitter SaaS I run. For this, I would copy existing metrics, but make the graphics super-sparkly. So, in my mind, this would be part of a bigger marketing plan.

I think you should start by thinking about the bigger picture: what can you promote by creating this tool. After that you can decide whether you need super-clever metrics, or can get by with standard ones.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
