## Do I really need to buy hardware at all? Cloud vs Lease

- posted by: [mudduckk](https://stackexchange.com/users/-1/3226-mudduckk) on 2010-04-27
- tagged: `lease`, `cloudcrowd`
- score: 2

My technical advisors...the guys that want to write code for me...want to drop about 80K on hardware assets.  Ouch!  Of course a lease comes to mind.  Less ouch!  Yet, I am aware of the cloud which is like getting the functionality of servers but paying for it as if it is a utility.  Pay for what I use - a pure variable cost. Great! :-) Now could somebody explain to me why I would want to do anything else but the cloud?  I mean, I can see why I need workstation/laptops, but can't I get all my other server needs hosted website, database, cache, apps, backups, DNS, Crypto, and mail - and just pay as I go?  

Thank you for your advice.

Malcolm C.


## Answer 10677

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-04-27
- score: 3

and welcome to this site.

I'm sorry, but as a guy who knows a thing or two about the cloud, I don't really see any way to answer your question with the information given.

Cloud hosting has some tradeoffs, there are limits on disk I/O, SQL DB server size, network latency and other things that make it less than ideal for some use cases. You didn't say what your product requires / is; so there is no way for us to advice.

However, for 90+ percent of common web applications (where latency is not a major issue) cloud hosting can be a good fit.

Another thing: It's just a gut feeling, and I wasn't there ... but as you present it, that advisor is giving me .. bad vibes. If a tech walked up to me, and suggested dropping 80,000  USD on hardware purchase for a startup without some very good reasons ... I'd question his competence.

> all my other server needs hosted website, database, cache, apps, backups, DNS, Crypto,

Website, probably. Database, probably. Cache, yes. Apps, well what do you mean by "apps"? Backups, yes. DNS, yes. Crypto, well what do you mean by "crypto".

In case it's not evident, many of the services above you'd want to buy as hosted solutions from specialized providers, not roll your own on a generic cloud computing platform.


## Answer 10671

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-04-27
- score: 2

Do you know already what the capacity you will need to run your business in terms of broadband and storage? If you are moving from one option to another and already have real data then it is one thing. However, if your advisors base their estimates on some case of scenario, then it is a totally different thing.

80K sounds like a major hardware purchase. Why not try to lease with a provider that can scale your capacity based on your real needs? Run it like this for a few months and see what exactly do you need.


## Answer 10695

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-04-28
- score: 1

Maybe if you use a hosted solution they won't let you burn incense around the servers to improve their Chi? 80K = Get a second opinion unless they want to put up half (and take a picture of the expression on their faces when you ask).

Programmers love control and don't want to have to tell you "We can't do that." because of something out of their control. Having 80K worth of hardware at your disposal lets you do just about anything. Have them look into plan B. Maybe you need to find someone who has developed in the cloud?




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
