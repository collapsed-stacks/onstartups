## Estimate Hosting Fees

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-13
- tagged: `hosting`, `costs`
- score: 1

Is there a good resource for estimating the cost of app hosting? I am bidding on a project that will likely receive a large amount of traffic (100,000 uniques/mo is reasonable). The app is fairly simple, read from db and print to screen. How do I accurately bid on hosting and bandwidth?


## Answer 12733

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-13
- score: 1

<p>To the best of my knowledge, there are no resources that can spit out a number for you. There are too many variables, not the least of which is the speed of your code.</p>

<p>The canonical answer is:</p>

<ul>
<li>Model how your user visits will be spread out in time, i.e. "100 k users per month, with 10 pages/session, evenly distributed across US business hours". Then figure out how many requests per second you need to handle. Add 25% to this for safety.</li>
<li>Figure out how many requests per second each type of server can handle, from actual measurement on the application, or at least a very similar application that you have built in the past.</li>
<li>Do the math.</li>
</ul>

<p>Be sure that your data store (database server, file server) can handle the load. Web app servers can be made stateless, and can fairly easily be scaled via a HTTP load balancer. Data stores (databases) are inherently statefull, and therefore much harder to scale beyond a single server.</p>

<p>This older post on the <a href="http://highscalability.com/stack-overflow-architecture" rel="nofollow">Stack Overflow architecture shows how few servers</a> can often handle a big load. But keep in mind, this is for a site written in (fast, well optimized) C# / ASP.NET MVC.</p>

<p>Regarding the contract, be sure to put reasonably provisions in there to limit the scope of the hosting agreement, and allow you to renegotiate if/when the usage exceeds a certain threshold.</p>

<blockquote>
  <p>receive a large amount of traffic (100,000 uniques/mo is reasonable)</p>
</blockquote>

<p>That's not much, but it all depends on how the user visits are spread out, how fast your application logic is, and if there are other considerations such as search engines to take into account. Just as an example, your load could be as low as 0.51 pages per second on average; assuming <code>(100,000 users/month * 10 pages/visit) / (18 hours/day * 30 days/month * 3600 seconds/hour)</code>.</p>

<p>You might want to ask the same question on Serverfault, with more technical detail than you included here.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
