## Help with Website

- posted by: [Tanvir Chowdhury](https://stackexchange.com/users/-1/3748-tanvir-chowdhury) on 2010-07-29
- tagged: `website`, `bootstrapped`
- score: 1

I'm working on a product that is set to launch in a few months and need to hire a web designer for our site. I've never done this before so I need help. The details for whats needed on the site are bellow;

1. E-commerce website with Shopping cart - For Software that we will be selling via digital download.

2. Company blog. With subdomain; blog.mycompany.com

3. Integrated CMS for site content and also Blog.

4. E-mail opt-in for when a free trial of software is downloaded.

How should I explain what I need to designers that I interview? How can I know that they will create a good SEO site? As you can tell im not a tech guy.

P.S Any idea on price? We're a bootstrapped start up so there is a mediocre budget.

Any and all help would be appreciated. Thanks.


## Answer 13141

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-29
- score: 2

<p>Just a friendly tip: You might get better answers if you post each individual problem as a question with the right tags, instead of lumping putting multiple questions together under the same tags.</p>

<p>To your questions:</p>

<blockquote>
  <p>E-commerce website with Shopping cart</p>
</blockquote>

<p>Think about whether you really need a shopping cart on site. If you only have a few different products, then maybe it's simpler to use one of the hosted value-added payment handling sites. Try to avoid handling (legally protected) credit card numbers yourself, by <a href="http://successfulsoftware.net/2009/10/12/a-survey-of-ecommerce-providers-for-software-vendors/" rel="nofollow">using a 3rd party</a>.</p>

<blockquote>
  <p>Company blog. With subdomain; blog.mycompany.com</p>
</blockquote>

<p>If you're using the same web technology for everything, then www.mycompany.com/blog/ is often a little better than blog.mycompany.com in terms of search engine performance. There is no reason to set up 2 hostnames (www. &amp; blog.) if it's all hosted on the same single server.</p>

<blockquote>
  <p>Integrated CMS for site content and also Blog.</p>
</blockquote>

<p>Self-hosted Wordpress 3 is a strong candidate for this requirement.</p>

<blockquote>
  <p>E-mail opt-in for when a free trial of software is downloaded.</p>
</blockquote>

<p>Often handled by a small HTML form that posts the result to a "newsletter handling service" like MailChimp, or by storing this information together with the order and then manually adding the customer to a newsletter service.</p>

<blockquote>
  <p>How can I know that they will create a good SEO site?</p>
</blockquote>

<p>You don't really, but if you use a good blog &amp; CMS engine like Wordpress 3, then you get many best-practices baked in for free. You'll still have to do lots of work with link building and trust building, but done with quality content and quality backlinks, not on-page tweaks. Also see the <a href="http://answers.onstartups.com/questions/tagged/seo" rel="nofollow">previous posts about SEO</a> here.</p>



## Answer 13139

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2010-07-29
- score: 1

<p>First, you'll need to figure out in more detail what will be on your site. What informational pages will you have (e.g. About Us, FAQ, Contact, Case Studies, etc). List it out, and the more detailed the list, the more accurate any quote will be (as well as cheaper in most cases).</p>

<p>Second, in terms of being well designed, there is some risk that you cannot get rid of, because you haven't seen the design they chose for your site. But you can and should look at other sites the designer/developer has built to get an idea for their style, and only look further at companies that have a style you like.</p>

<p>Third, SEO. At the risk of starting a flame-war, this is one of the most difficult areas to assess. While there are some basics that are easily verifiable, much of what is done for SEO even by companies that are actually quite good at it are impossible to verify independently. As a result, the best way to go here is to start working with a company for which you can get a reference, and watch for results. (For a slightly longer discussion on my opinions of the SEO industry, you can read an article I wrote a while back <a href="http://blog.optimalupgrades.ca/2010/06/the-unvalidated-industry/" rel="nofollow">here</a>.)</p>

<p>Last, price. It really depends where you go, and how much of a custom design you're looking for. A site such as the one you describe can cost from about $1000 to upwards of $10,000 for a fully customized look. My guess is that you would probably be somewhere in the $2,000 to $4,000 range, using a lightly modified template for your site.</p>

<p>If you are interested, feel free to get in touch with me directly about your site for a more precise quote (I do some site development, and would be happy to look at your project ifyou want).</p>



## Answer 16062

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-11-04
- score: 0

> E-commerce website with Shopping cart - For Software that we will be selling via digital download.

As someone else mentioned, if you are really strapped for cash, consider a third-party service for this.  If you have a little money, doing it yourself provides greater integration with the rest of your web presence in terms of branding, SEO, etc. and generally a better UX (User eXperience).

> Company blog. With subdomain; blog.mycompany.com

Again reiterating another's point: mycompany.com/blog is generally better SEO-wise unless you have a good reason to break it off to its own subdomain.

> Integrated CMS for site content and also Blog.
> E-mail opt-in for when a free trial of software is downloaded.

I know that someone else recommended Wordpress.  I don't.  Wordpress is the best blog tool out there, but it is just that: a single-purpose tool.  You aren't building a single-aspect web presence (i.e. just a blog).  Developing a blog on Wordpress with a third-party service to handle your ecommerce, email list, and trial downloads will probably be a little cheaper up front, but when you are ready to grow beyond that you will have to redevelop the entire site from scratch on another platform, and migrate all your products and content.  It's a pain, and depending on how well your third-party service lets you get your data out, if the WP site was done as well as possible, etc. may get expensive.

I recommend using a full-featured, general-purpose CMS like [Drupal](http://drupal.org)[^1].  It's like getting an entire toolbox instead of a single-purpose tool.  Not only can Drupal easily handle your main web site, blog, ecommerce, mailings, and everything else on your list (including having great SEO tools), but **Drupal can do all the things you might want to do later, but haven't thought of yet.**  This means you will not have to go through the bother and expense of redeveloping your whole site on a new platform, no matter what direction your web presence takes down the road, and you can adapt with much more speed and less upheaval in general.

> How should I explain what I need to designers that I interview? How can I know that they will create a good SEO site? As you can tell im not a tech guy.

A good developer (look for someone who uses the title "developer" or "consultant", not "designer" which generally comes with a more limited skill set) will walk you through creating a good site specification.  We don't expect every client to know all about web design: if you knew everything we did, we wouldn't have jobs!  It sounds like you have a decent feature list thought out, so it won't be hard for an experienced consultant to get you where you need to be.  (Based on your list, I could do a 1-hour phone call with you after which we'd not only have your development planned out but an idea of what directions the site might take after launch.  Any consultant who can't doesn't know what he/she is doing.)  A good consultant will also insist on training you as part of the deal.

As for choosing the right consultant: Ask about their experience, get client references, and most importantly: find out whether they are active in their professional community.  A good Drupal consultant gives code, support, documentation, or other tangibles back to the Drupal community (it's not all that altruistic, doing so keeps us up-to-date with changes in our CMS or platform, and lets us help nudge it in directions good for our business).  The same goes for a Wordpress consultant, or someone using another open source platform.

Community contributions indicate skill, speaking at (or even better, organizing and speaking at) conferences indicates the respect of one's peers, good client references indicate good customer service.

> P.S Any idea on price? We're a bootstrapped start up so there is a mediocre budget.

Price is really hard to nail down without going through creating a specification with you.  Here are some general ideas to help you along, though: Under or around $1,000 you will probably need to go third party service for at least your ecommerce stuff.  If you make a few compromises (license a non-exclusive theme or make slight modifications to a good free theme instead of going custom, for example) you can probably do everything you listed on your own Drupal site for the neighborhood of 2-3k (including training!).  If you want a truly custom theme, need logo design, add things that require custom modules (your current list doesn't require any), and get extreme with SEO (not wise for a small bootstrapped start-up, stick with the basics), you'll be up around 10k.

Please note that I don't have nearly enough info. to give you a solid estimate, those above are based on lots of assumptions about your business that may or may not be right.

I hope that helps.

Regards,

Susan


[^1]: I'm probably a little biased being a Drupal developer myself, but maybe not: I run the consulting firm, so we work with whatever I choose, and I chose Drupal for pretty much the same reasons I'm telling you to choose it, plus some DX (Developer eXperience) stuff.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
