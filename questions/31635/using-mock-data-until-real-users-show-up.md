## Using mock data until real users show up

- posted by: [Jared](https://stackexchange.com/users/-1/13910-jared) on 2011-10-19
- tagged: `beta`, `data`, `demo`, `users`
- score: 2

I just beta launched my website and right now there is only one user signed up for my service (it's only been a day and I'm not marketing it yet). It is highly data driven so without much context, users can't get a feel for the offering or give me feedback before I start marketing the website more.

I wrote a mock data generator that I've been using in development and it works really well, it gives a feel for what the website is with a decent size user base. I'm thinking of running this in production, but adding some type of obvious and apparent tag that says this profile / data is sample data. As more users join, I'll scale back the mock data.

Does anyone have any experience with this or thoughts on this approach?


## Answer 31646

- posted by: [Abhishek Sakhaparia](https://stackexchange.com/users/-1/11673-abhishek-sakhaparia) on 2011-10-20
- score: 1

Your idea seems very good. I would just like to suggest some minor changes.

You said you launched the beta with mock data (distinctly id'ed, of course), with actual users being added as per your plan, which your mock beta. For the next step, instead of gradually reducing the mock data, give users the option to move to the live / commercial version of the application with the same accounts, before taking the mock data completely offline.


## Answer 31653

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-10-20
- score: 0

Is there no way you can create some initial buzz? It seems like you will need to get a lot of people in quickly to get things going. Even though mock data will show how the site works, I am guessing the site doesn't really have much value until real people are using it.

I would consider some way to get an initial influx of people, be it paid or other marketing.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
