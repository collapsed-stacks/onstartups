## Why are so few commercial products (sold, downloadable software) built on ruby on rails?

- posted by: [Blankman](https://stackexchange.com/users/-1/4860-blankman) on 2010-10-19
- tagged: `software`
- score: 2

Is there a reason why there are so few commercial products that are build using Ruby on Rails?

Is there market so small where it doesn't make sense?
Is deployment an issue?

<b>Update</b>
I'm referring to software you purchase, and install on your own servers.


## Answer 15316

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-10-20
- score: 5

**There are several reasons** why Ruby / Ruby on Rails is not that popular for on-premises software (as opposed to hosted/SaaS software):

 1. **The Ruby runtime environment (compiler etc) is not good.** I mean this in the nicest way possible, but there really is no more polite way of saying it -- it isn't good. Getting it installed, tuned to perform fast, on multiple platforms (incl Windows), and with proper character encoding handling (fx UTF-8), is not simple. The Ruby community is hoping that a new dominant runtime will emerge, fx running on top of Java's VM, but so far it hasn't happened.

 2. Ruby is not compiled (by default it is interpreted, not compiled to bytecode fx) and the obfuscator scene for Ruby is un-developed. Thus if you send your Ruby application to someone else, that **means giving him all your source code.**

 3. **Poor libraries support.** Ruby has Rails for web applications, and Rails is truly nice. But outside Rails/webapps, Ruby actually doesn't have that many good libraries available (charting, datastore access, data warehousing, etc). Of course Ruby has many libraries available for it, but not nearly as many as fx Java or .NET have.


## Answer 15300

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2010-10-19
- score: 1

I think there's quite a few actually: http://isitrails.com (this site's database apparently has over 4500 Rails sites). For what it's worth, my site is built using Rails, and I'm building my software product using Rails.

I don't think there's much correlation between market size and the development platform. I'd say that Rails deployment is still harder than, say, PHP deployment and not as widely supported by hosting providers. On the other hand, I'm not sure there's anything like Engine Yard or Heroku for PHP.


## Answer 15305

- posted by: [viv](https://stackexchange.com/users/-1/2665-viv) on 2010-10-19
- score: 1

37signals product are entirely built on Rails and they are like the hottest startup in town - I think it's an amazing language and the closest to agile techniques


## Answer 15324

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-10-20
- score: 0

i tried installing rails on my .net machine for test development.  Gave up after 4 hours.  Rails, Django programming on a windows enviorment is tough.  Plus when you build commercial products for sale your goal is to be profitable as soon as possible. Its less expensive to hire a php prrogrammer if your aim is to build software packages that run on a clients web server.

For desktop apps, rails does not do that.  A great choice that is often neglected for real desktop apps is AIR.  I love air because of its use of webkit browser, and use it often for AJAX only apps.


## Answer 15372

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-21
- score: 0

<p><a href="http://www.amt.in" rel="nofollow">AMT</a> offers Ruby on Rails web development services. Our dedicated team of developers can create web 2.0 applications using latest Ruby on Rails web services.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
