## Technical Infrastructure Required for New Startup - questions about server, internet, cloud

- posted by: [ArtemisFowl](https://stackexchange.com/users/-1/11850-artemisfowl) on 2011-07-08
- tagged: `technical`, `infrastructure`, `server`, `cloud`
- score: 0

I'm defining the technical infrastructure required for my start-up

We currently have in our possession a  physical Dell PowerEdge T310 server
http://www.dell.com/us/business/p/poweredge-t310/pd

We will be launching a site/app that utilizes push notifications, check-ins, etc. 

Just wondering how much traffic the server could support? We are utilizing google places API, which handles 100,00 requests/day

At what point should we be thinking about moving into the cloud? Anyone have any suggestions as to any specific services (amazon?)

Also, at what internet speed should we be operating at? I'm looking at Time Warner Cable Business Class

http://www.twcbc.com/


Thanks, 




## Answer 27320

- posted by: [Alain Raynaud](https://stackexchange.com/users/-1/502-alain-raynaud) on 2011-07-08
- score: 2

A detailed discussion of hosting options would be off-topic here, but what is very much on-topic is this: focus on finding customers and stop worrying about scaling until later.

Let's put it more succintly: in all likelihood, during your first month of operations, you'll be serving about 100 visitors a day. Can your current setup handle it? Of course. So, start worrying on more complex hosting once you can detect a growing trend.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
