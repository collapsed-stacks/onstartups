## Platform / Language question for Photo site with mobile support

- posted by: [Seenu](https://stackexchange.com/users/-1/2809-seenu) on 2010-03-16
- tagged: `platforms`, `technology`, `web2.0`
- score: 4

This is a newbie question :-) Wasn't sure if StackOverflow or one of its sister sites would be a better place to ask, but thought I'd go ahead anyway here first.

A friend and I are toying around with an idea for a photo-sharing service. The service would be heavily mobile centric (uploading/sharing/viewing pictures from your phone), but will have a website component also. Our backgrounds are almost entirely in mobile software development, although we both have some Java (J2SE) experience.

This is not a super urgent thing for us, so we're willing to spend some time learning a new language/platform if necessary.

The fundamental question for us is what would be best for building a service like this? At a very high level, our basic requirements are:

1. A web-service API by which users can upload/retrieve/share/manage pictures from their phone-based applications

2. A spiffy website where they can do the same - in terms of responsivity/interactivity, we'd like it to be similar to flickr or tumblr

Right now, we're being faced with a Java vs. Ruby vs. PHP decision. One part of me wants to get going in Java so that we can have an implementation up. But on the other hand, I don't want to discover too late that it's not the most optimal and have to throw away and restart - like I mentioned before, we're willing to invest the time/effort to learn something new before kicking this off.

The major constraint for us is money. We're Mac-based and don't want to invest in a Windows machine just to be able to try ASP.NET - hence discounting that even though we can get free licenses through BizSpark.

So what I'm requesting for is advice based on your experience or stuff you've seen in the past - please do share!

Mods - Please retag as you see fit.

Cheers
-seenu

The most linked "Java vs. Ruby vs. PHP" discussion we've seen on the web is [this CMSWire article] [1] describing a talk given by Tim Bray.

We're also looking at [this post] [2] for some guidance.



  [1]: http://www.cmswire.com/cms/industry-news/php-vs-java-vs-ruby-000887.php

  [2]: http://answers.onstartups.com/questions/831/how-to-pick-a-platform-for-a-startup-web-2-0-app


## Answer 9284

- posted by: [Jacob](https://stackexchange.com/users/-1/2355-jacob) on 2010-03-16
- score: 3

I'm a Python guy, so I say Python/Django is the way to go. Of course the ROR crowd will say that Ruby is the best choice, the PHP coders will think PHP is best, and I think you can see the pattern. The truth is any of these languages will be capable of doing what you need to do. 

If you really want to learn a new language and/or framework I would suggest either Ruby on Rails or Django. Both have an active and helpful community, and at least on the Django side the documentation is good (I haven't looked at the ROR docs). Keep in mind that with a framework you're learning both a new language and a framework, so it will take longer than if you're just learning a language.

On the other hand, if this is a business venture I'd say go with what you know. Get a prototype done and get some feedback from your users. What language have you used for mobile development?


## Answer 9289

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-03-16
- score: 3

First things:

 1. The qualities of the platform matter much less than the qualities of the people. There are no (major) platforms so crappy that it justifies throwing out all code and starting from scratch.
 2. Skilled **developers with lots of experience on the platform** is the best predictor there is for successful development.

Regarding "starting from scratch", I could imagine a few rare situations -- extremely rare indeed -- where codebases written in the slower languages (Ruby, Visual Basic) could justifiably be re-implemented in faster languages to save on machine time. Taking an existing codebase in the other direction, from C#/Java to Python/Ruby is not something that I have ever seen done.

There is only **one other potentially strategy-changing issue** that I can see, and that's **exit scenario**. Youtube was built more or less to be flipped to Google. If you know beforehand who you want to buy your company, then pick the platform that integrates best with their existing infrastructure. But how often is this known beforehand...

So in your current situation, I would suggest that you use **whatever webapp framework for Java you're most familiar with now**.

If you really want to play around first, then consider looking at Python (Django or Turbogears) or Rails, but expect to throw the first version out. If you choose a non-Java framework, then it should largely be determined by your personal tastes, i.e. which language and framework 'feels' best for you.


## Answer 9285

- posted by: [Abhay Vardhan](https://stackexchange.com/users/-1/2368-abhay-vardhan) on 2010-03-16
- score: 1

If you want fast, iterative development, my recommendation is to go with Python or Ruby. These are much faster to work with, offer a pleasant but powerful environment and are OK in terms of performance. Java is possible but I find my progress to be much faster in Python/Ruby.

Regarding Python vs. Ruby, I see advantages and disadvantages of both. Python has a bigger community and a larger number of libraries but Ruby on Rails is just a awesome solution for webapps with everything packaged nicely and ready to go.


## Answer 9297

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-03-17
- score: 0

<p>Yes, repeating.  Your skills are more important than the platform..</p>

<p>If you desire a framework, why not consider <a href="http://www.grails.org/" rel="nofollow">Grails</a>? </p>

<p><a href="http://en.wikipedia.org/wiki/Groovy_%28programming_language%29" rel="nofollow">Groovy</a> is very familiar to java type developers (here are the <a href="http://groovy.codehaus.org/Differences+from+Java" rel="nofollow">differences</a>) , and Grails was originally named groovy on grails.</p>

<p>Definitely worth looking at given your background.</p>

<p>Good luck!</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
