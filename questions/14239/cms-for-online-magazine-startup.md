## CMS for online magazine startup?

- posted by: [Alexandru Trandafir Catalin](https://stackexchange.com/users/-1/4208-alexandru-trandafir-catalin) on 2010-09-22
- tagged: `website`, `software`, `technology`, `open-source`, `cms`
- score: 6

I want to start an online magazine website and I'd like to know what platform to use.

Something like Wordpress, Drupal, and other CMS systems, any recommendations? 



## Answer 14240

- posted by: [ewalk](https://stackexchange.com/users/-1/4317-ewalk) on 2010-09-22
- score: 12

<p><a href="http://wordpress.org" rel="nofollow">WordPress</a> with a free theme such as <a href="http://wordpress.org/extend/themes/magazine-basic" rel="nofollow">Magazine Basic</a> installed, is good solution if you are looking to make your magazine publicly accessible and do no want to program. </p>

<p>If you have more specific needs and would have programmer resources available, the Django programming framework can offer a great starting point for building a magazine that is adapted to your business needs. Many online editions of news papers are build leveraging this software.</p>



## Answer 14434

- posted by: [Marna Friedman](https://stackexchange.com/users/-1/4444-marna-friedman) on 2010-09-26
- score: 3

<p>I believe that WordPress is your best option, and you can even check out the <a href="http://wordpress.stackexchange.com/">WordPress Stack Exchange site</a> for answers to questions you have once you set up your site.  As far as a theme to use, I suggest looking at StudioPress themes, their service is outstanding!  WordPress is the most popular CMS being used, and because of this, I think offers the most options and access to assistance.</p>



## Answer 14421

- posted by: [bigown](https://stackexchange.com/users/-1/4193-bigown) on 2010-09-25
- score: 2

<p>Probably you will need something more sophisticated like <a href="http://www.drupal.org" rel="nofollow">Drupal</a> or <a href="http://www.joomla.org" rel="nofollow">Joomla</a>.</p>

<p>You can look for a web publisher software like <a href="http://www.krangcms.com" rel="nofollow">Krang</a>. It's more specialized.</p>



## Answer 20984

- posted by: [darrenp](https://stackexchange.com/users/-1/8195-darrenp) on 2011-03-01
- score: 2

<p>The big difference between something like Wordpress and Drupal is contributing users. Wordpress is more suitable for the sole contributor and Drupal is ideal for multiple contributors. So if you plan to have multiple writers then you really need to go with something like Drupal.</p>

<p><a href="http://drupal.org/drupal-7.0" rel="nofollow">Drupal 7</a> was recently released and it's quite the upgrade. They worked really hard on usability. </p>

<p>A great way to try Drupal 7 is with <a href="http://www.drupalgardens.com" rel="nofollow">Drupal Gardens</a>. It's a hosted solution by Acquia (founded by Mr Drupal himself). You can have a site up and running within minutes for free. Their pricing is very reasonable if you grow out of the Free plan or you can export your site and host it somewhere else at any time.</p>

<p>I think you should ignore religious arguments about PHP, Ruby, Python etc. Your starting a magazine not a software company. So you need to focus on getting the right tool to solve your needs. Programming language really doesn't matter.</p>

<p>Frameworks will give you a little more flexibility to do anything you want but you then also have to do everything. That flexibility would allow you to do bad things just as much as good. You'll spend valuable time and money developing very common components that have been done hundreds of times before. Using a tool you'll get the benefit of thousands of hours of other developers optimization and as long as it's open source your really not giving up any flexibility. Underneath any tool is a framework and programming language that you can tweak until your heart is content.</p>



## Answer 20879

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-27
- score: 1

<p>It is worth briefly understanding the differences between content management systems (Drupal, Wordpress, Joomla) and development frameworks (Django, Rails, Symfony, Zend). You always have more flexibility with a framework, and the technical architecture is usually much cleaner (which is good for large, complex projects). But a CMS is usually the way to go, since replicating the features of Wordpress etc in a framework will take months (if not years) of solid development. Why reinvent the wheel?</p>

<p>Wordpress used to be a blogging tool - and is very good at that - but these days resembles a fully-fledged CMS. I like it a lot; it is easy to use and easy to hack. There are loads of plugins and themes available, mostly free of charge.</p>

<p>@denysonique - Django and Rails are certainly popular, but one has to take into account the availability and cost of developers. PHP has been around for a lot longer, as has Wordpress, and accordingly I'd wager that more devs are available, and the respective ecosystems are much larger. (Disclaimer: I'm a PHP dev, though keep meaning to read the Rails books on my shelf!)</p>

<p>Edit: @Julian: I'm not familiar with Silverstripe, but Wordpress can do that out of the box. WP calls this <a href="http://www.rlmseo.com/blog/wordpress-custom-fields/" rel="nofollow">custom fields</a>, and it's very easy to use.</p>



## Answer 14477

- posted by: [Julian](https://stackexchange.com/users/-1/4465-julian) on 2010-09-27
- score: 0

<p>My favourite for this stuff is <a href="http://www.silverstripe.org" rel="nofollow">Silverstripe</a> -- PHP-based with immense flexibility around custom article types (adding additional metadata / fields to an article -- a traditional weak point with things like Joomla). See <a href="http://demo.silverstripe.com/" rel="nofollow">demo</a></p>



## Answer 18591

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-06
- score: 0

Personally I wouldn't recommend anything based on PHP, now Django and Ruby On Rails is the way to go. A blog can be built in Django in literally 5 minutes. 

Wordpress? Wordpress is a blogging platform, right? Because it seems to be a CMS…

Drupal, I used to use drupal and it is not too bad, anyway PHP based software is not the best idea

Django was born in a news agency!

If you don't have the skills or devs to write your own Django or RoR blog then you can use WP… but when you become successful, think about migrating to other better platforms such as the ones I mentioned.


## Answer 18594

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2011-01-06
- score: 0

drupal / joomla are better suited for magazines - finer grained control of pages, sections, content blocks, modules.  Wordpress *is* easier, and magazine type templates abound, but once you get started you'll hit article placement limitations pretty quickly. Start considering a gallery, directory, classified section - and then you start to push wordpress well beyond its initial capabilities. 

Don't get me wrong - wordpress is great. But use the right tool for the right job - joomla, drupal, silverstripe all are much more than a blogging system.  



## Answer 20943

- posted by: [Andy Cook](https://stackexchange.com/users/-1/6493-andy-cook) on 2011-02-28
- score: 0

<p>This is a really old thread, but I thought I'd throw in my two cents:</p>

<p>Use Wordpress and a premium theme from ThemeForest. <a href="http://themeforest.net/category/wordpress/blog-magazine" rel="nofollow">Here's</a> a link to magazine-style layouts. There's about 150 that you can preview.</p>



## Answer 24483

- posted by: [Sam](https://stackexchange.com/users/-1/10234-sam) on 2011-05-05
- score: 0

Wordpress is great for this application. Get a magazine oriented theme and you've got a solid out of the box magazine site.

If you will have user contributed content however, you may want too look at Joomla or Drupal.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
