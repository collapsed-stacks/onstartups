## Are there any good monetization strategies for webservice/API providers?

- posted by: [John MacIntyre](https://stackexchange.com/users/-1/760-john-macintyre) on 2009-11-24
- tagged: `webservices`, `api`, `monetization`
- score: 2

I often have ideas for a webservice ... as in a live internet programming API (Application Programmable Interface) for other websites. Ideally, I'd like to allow access to the API for free in order to gain more websites using it.

But how can I possibly monetize this? How can I even cover my costs? ... any ideas?

EDIT: Thanks for answers so far, but sorry I should have been more clear.  

A few API monetization strategies that I can think of:

 1. Develop a highly specialized API which does some calculation which most people wouldn't even know how to program.
 2. Develop an API which somehow captures information, which can be aggregated and sold.
 3. Develop an API to add value to another existing monetizable product.

But what I'm asking about mostly is; How can I turn 'commodity like' functionality into an API, which I could make money from.  

For example; how could [myopenid.com][1] OR [gravatar.com][2] monetize?  I don't expect websites are paying for these services.


  [1]: http://myopenid.com
  [2]: http://gravatar.com


## Answer 4117

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-24
- score: 4

It really depends on the ideas and the value to others, not on the fact that it's a web API.

There are places you can post new web APIs for exposure, but of course that's not money.

Requiring an account (with security token) makes it possible to track use for later monetization, so that part is not hard (or at least, you just have to do it once).

The real question is: **What service is worth paying for?**  How can you charge?  Amazon uses a micro-payment model -- people seem to like that (and you could use Amazon payments to run that model as well).  Or free until a limit of API calls/day or /month or bandwidth or whatever makes sense for the service.  That way it's free to try but if it's in real use I start paying.

There's tons of services out there of all types!  So in general it's a sound business model.


## Answer 4132

- posted by: [Joe A](https://stackexchange.com/users/-1/60-joe-a) on 2009-11-25
- score: 2

You could offer a free plan that had a cap of X calls per day. At the same time, offer a paid version that gives them X*10 calls per day up to a certain amount then like $0.10 per call after that. Also, you could consider requiring the free users to place a logo like "powered by YourAPI.com" somewhere on their website in order to gain market traction. 

If you API has any real value, the free users would eventually up-convert to the paid model. Your target is obviously website operators, not kiddies and tweens on MySpace. I doubt you should have a problem monetizing your service from these users.





## Answer 4385

- posted by: [Olivier Lalonde](https://stackexchange.com/users/-1/1030-olivier-lalonde) on 2009-11-30
- score: 0

You might want to take a look at http://mashery.com/. They have some white papers and I believe they offer free consulting.

> Having an API strategy is only part of
> the puzzle. Contact Mashery today for
> an assessment of your business
> strategy.
> 
> Mashery is the leading provider of API
> management services enabling companies
> to easily leverage web services as a
> distribution channel.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
