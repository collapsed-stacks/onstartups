## How should I launch an API demo as an MVP?

- posted by: [Joseph Turian](https://stackexchange.com/users/-1/423-joseph-turian) on 2012-01-08
- tagged: `market-research`, `demo`, `api`, `mvp`
- score: 0

I have an API that I would like to launch as an MVP, to gauge market interest.
It extracts keywords from text.

Goals:

  1. Acquire users on my mailing list, so I can market other products and services from my consultancy.
  1. Gauge potential interest in charging for the API on a per-subscription basis.
  1. Gauge potential interest in people having the service customized for their particular data. (The API is for general web text, but people might want it for high-value technical domains, on which the demo will not work well.)

Here is a competing API.
They allow you to test the technology from the web (not from an API). If you register, there is a free plan with a low usage limit, and paid plans for more usage.

What is the correct way to launch my demo? Each launch strategy has potential benefits and disadvantages for each goal:
 

 1. Just put the API up, explain that it's a temporary demo and ask
    people on the honor system not to make more than 1K requests per
    day. Benefits: Low barrier for testing. Disadvantages: Doesn't
    acquire users for my mailing list, might get abused.
 1. As before, but
    also ask that users sign up for my mailing list.
 1. As before, but
    don't allow users to try the API until they sign up for my mailing
    list.
 1. Force users to create an account on my system. Advantages:
    Since users are signed up, it is easier to get them to start paying.
    Can directly prevent abuse. Looks more professional. Disadvantages:
    The highest barrier to trying my API means fewer people test it. (I
    can encourage them by posting sample output though.) Extra coding
    time. Less forgiveness from users for kinks I still need to work
    out (e.g. isn't scalable to multiple concurrent requests).
 1. Copy the competitor's approach, i.e. demo through a web interface and force users to sign up for a free or paid plan for API access. Benefits: Easy to demo. More clear to the user that abuse is not allowed. Disadvantages: I have to code up something that allows me to sign up users, should they want to sign up. Alternately, I could collect their email addresses.

What are your thoughts on the difference approaches?


## Answer 34559

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-01-08
- score: 2

Here are my three suggestions:

1) No matter what else you do, have some way to collect email addresses. A page like "If you would like to be part of our beta test please enter your email address..."

2) At this point a web based test interface that anyone can try without signing up or providing an email address is a good idea. One doesn't need to make an API call to determine the quality of your keyword extraction, a web interface like Alchemy will work just fine.

3) To prevent abuse, no matter if a HTML or API based test interface, simply throttle requests. You can either limit the number of requests from a particular TCP/IP address (4 per min perhaps) or make each request take a minimum of 15 seconds to respond. If you do have throttling then say so and tell people that they can contact you to arrange for a tryal that is not throttled.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
