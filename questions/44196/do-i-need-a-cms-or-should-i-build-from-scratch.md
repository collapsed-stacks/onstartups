## Do I need a CMS or should I build from scratch?

- posted by: [JDH](https://stackexchange.com/users/-1/13136-jdh) on 2012-11-13
- tagged: `development`
- score: 4

I am working on my first web application, and can't figure out whether I should use a CMS like Joomla or Wordpress, or have the site built from scratch. For some background, the site will be sort of a smorgasboard of features in a healthcare related industry, with a directory attached. I don't want to ever be limited by what i can do as far as design, or development, and have many more features planned, but nothing technologically ground-breaking by any means. 

I am interested in a CMS because I understand that building certain parts, (logins, registrations) things like that, go much quicker. However, aren't there sort of "out of the box" scripts for things like this that can be used even if I build from scratch with PHP? I am also interested in a CMS because from what I've read it seems that it will be easier to bring on new developers and have them know what everything does and understand the code, but aren't there ways I could build from scratch and just maintain a clean code base that is well commented and not run in to the problem of confusion from future developers? 

Ideally, I would like to build from scratch, I just want to make sure I am not losing the 2 benefits of having out of the box solutions for quick building, and an easily maintainable and scalable code base. Any advice on which I should use?

EDIT: I am fairly technologically savvy, have a strong grasp of html/css/javascript and ftp


## Answer 44197

- posted by: [Anonymous](https://stackexchange.com/users/-1/11482-anonymous) on 2012-11-13
- score: 7

<p>I would suggest you look into learning a framework.</p>

<p>There is a 'scale' between starting from scratch and building on-top of an existing application and each end of the scale has it's pros and cons.</p>

<p><strong>Building from scratch</strong></p>

<ul>
<li>Alot of things to consider (routing, security, organization, error handling, authentication, templating, etc).</li>
<li>Ultimate control and <em>understanding</em> over the way your app works.</li>
<li>May be restricting in terms of expansion. Nobody else out there will be familiar with <strong>your</strong> code, just the concepts it's built upon.</li>
</ul>

<p><strong>Adapting a CMS/other software to do your bidding</strong></p>

<ul>
<li>There may be a slightly higher learning curve for you to begin with. You need to learn how it works to expand it.</li>
<li>Some things may not be possible depending on the way the application is built.</li>
<li>It's easier to look for others that are familiar with the base software to join you, should you need to expand.</li>
</ul>

<p><strong>And the sweet spot/where my recommendation lies - a framework</strong></p>

<ul>
<li>Frameworks take care of a lot of the aforementioned complexities that come with building your own app.</li>
<li>Popular frameworks will be more thoroughly tested than something you could ever produce yourself.</li>
<li>Frameworks abstract away the time consuming complexities and allow you to be the most productive in building the app in question.</li>
</ul>

<p>For popular PHP frameworks, see <a href="http://symfony.com/" rel="nofollow">Symfony</a>, <a href="http://codeigniter.com/" rel="nofollow">CodeIgniter</a>, <a href="http://framework.zend.com/" rel="nofollow">Zend</a>, <a href="http://cakephp.org/" rel="nofollow">CakePHP</a>, <a href="http://laravel.com/" rel="nofollow">Laravel</a>, <a href="http://fuelphp.com/" rel="nofollow">FuelPHP</a> and <a href="http://www.yiiframework.com/" rel="nofollow">Yii</a>.</p>



## Answer 44231

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-11-15
- score: 1

<p><strong>Alternative view:</strong> Beyond devolving into a CMS vs Framework vs Language choice, I would offer the following views:</p>

<ol>
<li>Execution/launch trumps theory  </li>
<li><a href="http://c2.com/cgi/wiki?PrematureOptimization" rel="nofollow">Premature optimization is the root of all evil</a></li>
</ol>

<p>You mention that this is your first web application, you are tech savvy, and that your solution is a "smorgasbord of features" combined with a directory.  </p>

<p>This sounds more like a market validation effort than an architecture effort (nothing wrong with that, btw).  Since CMS'es - Joomla / Drupal et al. - all have mature directory components, why not just put together a sprint project and see if you can deliver the desired functionality with that? Then show it to your intended customer base and get their feedback.</p>

<p>Worrying about "easily maintainable and scalable code base" is premature at this point - getting something in front of a prospective customer for validation is more important. </p>

<p>I can also argue about frameworks vs CMS vs Languages - but getting business traction and then revisiting the technical decision when you have specific (vs smorgasbord) requirements will be an easier task.</p>

<p>Good luck with your effort.</p>



## Answer 44226

- posted by: [Maikel](https://stackexchange.com/users/-1/21567-maikel) on 2012-11-15
- score: 0

I would take a look at something Like ExpressionEngine.

It's a CMS, without being a 'website manager'. This means that instead of 'pages and posts' you can create custom datatypes. You can then create custom entry forms for each (eg image, file, bool, ...) and do manipulations (eg create thumbnail). This means you can have a completely different data model for 'authors' and 'book'. And just bring them together in a single view. Real separation of content and layout.

ExpressionEngine is built on top of CodeIgniter framework so you can simple write new parts when (if) you need them using all the framework functionality (eg the login modules etc).

Downside is, it's not free. But definitely check it out and see if it fits your datastructure. 
http://expressionengine.com/

To get a glimpse at how the development proces works, this is a good beginner example:
http://www.train-ee.com/courseware/free-tutorials/category/building-a-portfolio-site



## Answer 44229

- posted by: [MaddHacker](https://stackexchange.com/users/-1/17914-maddhacker) on 2012-11-15
- score: 0

You can approach this issue in a number of ways.  Most importantly, you need to look at costs.  Always remember, you can have something 1) fast, 2) cheap or 3) correctly done, now pick 2.

If you want something fast and cheap, a CMS is great, but it might not be correct for your businesses.

If you want something fast and correctly done, a custom solution might be your answer, but it won't be cheap

If you want something cheap and correctly done, it will take time.

etc.

If you have a clear vision of what you want this to do, then I would always suggest a solution that involves customization.  A framework is nice, but has it's own set of rules and restrictions, to a point.  The most flexible solution is one that is built from the ground up.

IMHO, if I was looking at this solution, I would look at several things:

 1. How much money do I have?
  
  If you don't have much money, a CMS is great.  If you're willing and able to do the work yourself, a framework will give you more of a base, but you'll need to spend time/money to get it working.

 2. How soon do I want this to be in operation?

  If you want something quickly, CMS will be fastest.  Most hosting companies can get one running in a matter of minutes, and you can customise and start going very quickly.  A framework (PHP based) will be easier to host that something else (Ruby/Rails, Java/Spring) but will not be nearly as secure or as fast.

 3. What are my top requirements?

   - Security

     Don't use PHP, and keep in mind any pre-built software will have more common vulnerabilities than any custom software.  CMS platforms, especially open source, all share vulnerabilities (since the source is published).  A framework will have some common vulnerabilities, and the custom built solution will only have the issues you write into it.  The nice part is, the more you get away from a set of pre-built published code, the less likely standard issues will be there (as long as you have a reasonable knowledge of what you're doing).

   - Speed

     Don't use PHP, it is the slowest language out there right now.  Also keep in mind any pre-built software will have to be more flexible and support more use cases, so speed typically will be slower.  The more you have that is pre-built and generic (for all consumers of the software) the slower your load times will be.  As a side note, do remember that Google does care about load time when considering page rank.

   - Rapid launch

     Pre-built is the way to go, the more custom something is, the longer it takes to build.

   - Cost

     Pre-built is the cheapest, then frameworks then custom.  PHP is the cheapest language (hosting and writing), Java will be most expensive.

   - Other User/Business requirements

     This covers everything from login, to edit, to image management.  Basically, what are the business rules you care about most?  Does the CMS offer all of the things you need/require?  If not, analyse the cost of adding those now, versus the cost of waiting to add them upfront.

Personally, most of my contract work related to development is because a system written in a slow, insecure language (typically PHP) needs to be faster, more flexible and more secure.  The problem is, those solutions are more expensive to both build and host.  If you can do it yourself, just run some analysis on the business vs the options, or talk to a friend/contractor Business Analyst.  The point of the BA job is to understand what you need, and evaluate options for you.  Without more information on what you're doing, that's about all I can help with.

Hope this helps, do let me know if this is unclear.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
