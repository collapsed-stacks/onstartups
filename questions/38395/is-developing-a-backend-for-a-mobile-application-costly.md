## Is developing a backend for a mobile application costly?

- posted by: [newth](https://stackexchange.com/users/-1/17602-newth) on 2012-04-20
- tagged: `saas`, `mobile`, `mobile-apps`, `cloud`
- score: 4

I'm developing mobile apps for a time and I feel I'm spending nearly 50% of my time for backend development, choosing the technology, etc.

Now I have a new idea for a mobile startup. I want to prototype it quickly.

Is using a cloud backend service like Parse and Kinvey viable, so I can focus on what matters most - which is the application itself? 


## Answer 38416

- posted by: [Mihaly Borbely](https://stackexchange.com/users/-1/13257-mihaly-borbely) on 2012-04-21
- score: 1

Great question and good point about focusing on the app itself. There are more and more BAAS companies every day, and it might be a good idea to consider them, although I haven't looked into their prices.

On the other hand, if you want to prototype fast, and cheap in the same time, why don't you just forget about the scalability issues of your backend altogether? After all, prototyping is all about iterating, with minimal server load. Any cheap (or even free) LAMP server will do. Write minimal throwaway backend code, and finalize when getting close to market fit.

The quality of your backend will be very important later on, but while prototyping, I don't see a reason why wouldn't you get away with a simple default php-mysql setup. For many usecases, even a textfile will do as database in the early days. :)

That said, I'm not a professional developer, so I might have overlooked some aspects here.


## Answer 38577

- posted by: [Nick Stevens](https://stackexchange.com/users/-1/15902-nick-stevens) on 2012-04-27
- score: 1

Using Parse or Cloudmine is perfectly viable, and does indeed allow you to focus on the product rather than a complex backend. In many situations, such a flexible solution might actually be preferable to creating a backend that may need to change significantly as the product changes during it's early stages.


## Answer 38411

- posted by: [Genadinik](https://stackexchange.com/users/-1/8929-genadinik) on 2012-04-21
- score: 0

I think it would be roughly the same price as developing a backend for a regular web application.

I made a mobile app before which used a backend server and db.  It was identical to a regular web application.

Best,
Alex



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
