## How to be data-driven startup (and handle spiders from search engines)?

- posted by: [Hendro Wijaya](https://stackexchange.com/users/-1/115-hendro-wijaya) on 2009-11-15
- tagged: `ab-testing`, `metrics`, `analytics`
- score: 6

I am curious on how some of you adopt data-driven approach to your startups.

Recently, i did an experiment with simple AB testing tool like A/Bingo:
http://www.bingocardcreator.com/abingo/

Through that, i found that majority of our traffics are search engine's spider. 

Example: instead of 100 visitors with 10% conversion rate (10 users), it become 10000 visitors and 0.001%. 9900 "visitors" are spiders.

How do you handle that? Any tools you would recommend?

It would be great if you have any reference to blog post or article that explain in detail on how to adopt data-driven approach to startups.

PS. Have been reading heaps about Dave McClure AARRR, Eric Ries, Andrew Chen, Mix Panel etc. I am looking for "more specific, with real-world scenario" kind of example.

Thank you.


## Answer 3656

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2009-11-15
- score: 1

<p>I think robots.txt works well with "genuine" bots, and evil bots can be handled using htaccess rules.</p>

<p>See robots.txt examples from some top sites -</p>

<ul>
<li><a href="http://www.webmasterworld.com/robots.txt" rel="nofollow">Webmaster world</a> This one is hilarious</li>
<li><a href="http://forums.digitalpoint.com/robots.txt" rel="nofollow">Digital point forums</a></li>
<li><a href="http://stackoverflow.com/robots.txt" rel="nofollow">Stackoverflow</a></li>
</ul>

<p>See this for .htaccess rules - <a href="http://www.webmasterworld.com/forum13/687.htm" rel="nofollow">http://www.webmasterworld.com/forum13/687.htm</a></p>



## Answer 3666

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-15
- score: 1

Use a web analytics tool that's Javascript-based -- those aren't triggered by search bots.

Beyond that, you'll have to discard all results from search engines.  Maybe Patrick can help make that change to A/Bingo.

P.S. +1 on the robots.txt



## Answer 3773

- posted by: [Hendro Wijaya](https://stackexchange.com/users/-1/115-hendro-wijaya) on 2009-11-18
- score: 0

<p>Here's what i found recently about adopting data-driven method. it helps articulate the concept a bit:</p>

<ul>
<li><a href="http://www.ashmaurya.com/2009/11/how-i-am-measuring-productmarket-fit/" rel="nofollow">How i am measuring product market fit</a></li>
<li><a href="http://www.ashmaurya.com/2009/11/from-minimum-viable-product-to-landing-pages/" rel="nofollow">From minimum viable product to landing pages</a></li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
