## Tracking User Actions on Landing Pages

- posted by: [Chris W.](https://stackexchange.com/users/-1/13188-chris-w) on 2011-06-21
- tagged: `marketing`, `webservices`, `webapp`, `ab-testing`
- score: 3

I'm developing a web application. It's months away from completion but I would like to build a landing page to show to potential customers to explain things and gauge their interest--basically collecting their email address and if they feel like it additional information like names + addresses.

I was planning on building this myself, but it seems like something like this must already exist, either as a web-service or as a pre-existing framework I can use.

The features I require:

- to display a fairly static page and potentially a series of pages
- collect emails (and additional customer data)
- track their actions--e.g., they got through the first two pages but didnt fill out the final page.

Sweet extras:

- Built-in support for A/B testing.

<hr>

On a side note, I'm using Django to build my app, so if this thing integrates with Django in some way (e.g., it's a Django App) then that would be even more awesome!


## Answer 27876

- posted by: [Andy Cook](https://stackexchange.com/users/-1/6493-andy-cook) on 2011-07-22
- score: 3

<p>You could use the following services:</p>

<ul>
<li><a href="http://unbounce.com/" rel="nofollow">Unbounce</a> or <a href="http://launchrock.com/" rel="nofollow">LaunchRock</a> to setup the initial landing page</li>
<li><a href="http://www.google.com/analytics/" rel="nofollow">Google Analytics</a> to track how many people are coming to your site (I know Unbounce tracks this as well)</li>
<li><a href="http://mouseflow.com/" rel="nofollow">MouseFlow</a> to actually be able to watch</li>
</ul>

<p>You can also use <a href="http://theclicktest.com/" rel="nofollow">ClickTest</a> and <a href="http://fivesecondtest.com/" rel="nofollow">5SecondTest</a> to tweak your landing pages as well.</p>



## Answer 27881

- posted by: [Bryan Marble](https://stackexchange.com/users/-1/4228-bryan-marble) on 2011-07-22
- score: 2

LunchRock has been great for building an e-mail list quickly, but you'll also have to manually import the list into your email management software (I've heard great things about MailChimp, but have been using Hubspot for mine).  As for workflow tracking, you should be able to do basic tracking using Google Analytics.  In this use case, I'd suggest creating your own solution if you're quick enough in django.  Off the shelf solutions won't allow you the necessary granularity to really figure out what's going on.  Besides, once you actually get to the point that you launch your app, if you're using a service, you're likely going to have to continue using the service to serve your static pages, or else have to go through some careful migration to avoid losing the SEO credit you've built up.

I've used LaunchRock by redirecting mydomain.com to the LaunchRock page to get the initial list started, a wordpress blog on blog.mydomain.com to start building content and organic search traffic, and I have static pages/landing pages hosted as part of my application at mydomain.com/my-landing-page where I can easily control analytics and bare-bones a/b testing.


## Answer 27852

- posted by: [John Plummer](https://stackexchange.com/users/-1/4891-john-plummer) on 2011-07-22
- score: 1

I would use Wordpress as the framework with the Mailchimp plugin to collect emails and Google Analytics for tracking.

There is also a Wordpress plugin for Google Website Optimizer, I have no experience with it though.


## Answer 26596

- posted by: [Joseph Fung](https://stackexchange.com/users/-1/1669-joseph-fung) on 2011-06-22
- score: 0

We've used mouseflow.com for projects like this with some very positive results.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
