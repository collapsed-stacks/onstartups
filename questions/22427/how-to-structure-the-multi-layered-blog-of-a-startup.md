## How to structure the multi-layered(?) blog of a startup

- posted by: [Igorek](https://stackexchange.com/users/-1/4395-igorek) on 2011-03-28
- tagged: `website`, `blog`, `seo`
- score: 2

So, this is likely more of an "information architecture" sort of a question... but I admit, in the last 20years of internet revolution, I've been on the frontier of pretty much every new wave... except blogging... I'm not an expert on intricacies of RSS/SEO/underlying blog-enabling technologies... etc... 

Is there a primer for people like me?  

Having said that, I'm looking for practical advice on how do structure all the blogging content and make it available to my visitors on an easy-to-consume basis? I'm afraid that if I put everything together in one big timeline, people will miss important news and get lost in unimportant stuff.

I have a SaaS product.  Landing website is a MVC.NET2 site.  Blogging software is installed on the same web-server and is BlogEngine.NET.  I would like to blog about a number of categories, some for purpose of letting visitors know about my product, some for purpose of driving SEO traffic, some for purpose of letting my users keep up with latest news.  Categories are something like this (would love some practical advice here too btw)

1) Company news.  These entries I want visible on the home page.

2) Newsletters.  I send out newsletters every week or two.  I'd rather not pollute home page with their content but I still would like them to be available for RSS subscribers and for users to read

3) Media mentions.  There are times when websites mention/talk about/review our product.  I'd love to have my visitors know about this

4) There is plenty of experience that we have accumulated in the vertical industry we're in.  I'd love to see this experience shared via light-weight practical tip-like sort of blog entries.  This will also hopefully start generating organic traffic via SEO

5) Perhaps there will be other opportunities/categories to blog about

I'm somewhat confused how companies are able to structure their blogs and keep things straight and easily findable.  There are pages and posts, but I don't believe any hierarchy exists except categories and tags... but do visitors ever use those consistently?

How do I submit only certain categories (the sharing of experience part of the blog posts) to other sites that aggregate this sort-of content?  If I blog about Windows Azure tips & tricks or newsletters, I certainly would not want the posts with my company news being submitted to Azure-related technical websites... 


## Answer 22428

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-03-28
- score: 1

<p>Well as it happens we have </p>

<ul>
<li>2 blogs running, <a href="http://www.redgum.com.au/blog.html" rel="nofollow">Business centric</a> and <a href="http://www.redgum.com.au/technical-blog/blog.html" rel="nofollow">Technical</a>.</li>
<li>A news feed for press releases</li>
</ul>

<p>and people are welcome to open their own blogs as well but they generally just use the technical blog.</p>

<p>That said most people find us through google so time isn't as important a factor. 
We do got some through twitter and facebook, the occasional one through posts here like the ones above.</p>

<p>What I started out intending to say was it doesn't really matter as most people will find you through google or direct links so how you catagorise it on your site is purely for aesthetic reasons.</p>

<p>... that is unless you wish to submit your RSS feeds to specific content aggragators where the topic is important, then its better to just use specific tagging and make the RSS URL off the tags.</p>



## Answer 27600

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-07-17
- score: 1

<p><strong>First, just a thought:</strong> It's obvious that Wordpress is the market share winner in blog engines. It might be a consideration to use Wordpress instead of your .NET blog engine.</p>

<p><strong>Regarding information structure:</strong> The most important thing is to make it useable for your end users. Some ideas:</p>

<ul>
<li>Give your blog a moderate number of categories (5-10). Place each post in the most appropriate category -- try to avoid making posts which belong in multiple categories (split larger posts up if that's a good fit). Link to the category indexes from the home page.</li>
<li>One quick (just first draft) list of categories for you could be: General, Newsletter, Media, and [your-vertical-name] (for domain-specific 'articles')</li>
<li>Be sure that your blog engine plays nice with the SEO -- that it avoids duplicate content penalties fx.</li>
</ul>

<blockquote>
  <p>How do I submit only certain categories</p>
</blockquote>

<p>When a blogger comments on a post, the <a href="https://secure.wikimedia.org/wikipedia/en/wiki/TrackBack" rel="nofollow">"TrackBack"</a> is tied to the post permalink -- so this is unique for each post.</p>

<p>When submitting RSS feeds to simple aggregators, you just submit the feed from the relevant category. (Good blog engines match the feed to the page you're on, so the feed linked to from the "Newsletters" category only contains newsletters.)</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
