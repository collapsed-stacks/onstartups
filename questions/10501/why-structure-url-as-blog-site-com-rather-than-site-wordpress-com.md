## Why structure url as blog.site.com, rather than site/wordpress.com?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-22
- tagged: `blog`, `domain`
- score: 5

I was one of your recipients of $20 at the New Comm Forum yesterday, and I went out and bought your book with it! You clearly know a LOT! 

I told my Tech Director last night that we should restructure our blog url according to your specs, and he said "why"? He said it's not that easy and there should be a good reason. Please advise. Thanks, Jennifer http://www.rhythmstrummer.com


## Answer 10508

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-04-22
- score: 5

<p>and welcome to this site. :-)</p>

<p>You should not use <code>http://company.wordpress.com</code> or <code>http://company.blogger.com</code> -- it looks unprofessional.</p>

<p>If it's possible, then the classic advice is to keep as much content as possible on just one domain name, i.e. www.company.com/blog/ .(company.com is one domain name, www.company.com is another, and blog.company.com would be another domain again.) The reason is that search engines calculate 'authority' (Pagerank etc) based on inbound links, and inbound links are counted on a per domain basis. Thus having multiple domains leads to your 'authority' being diluted/reduced.</p>

<p>However, there is another argument to consider. www.company.com must point to a specific set of IP addresses, i.e. specific servers. Sometimes it can be very advantageous for operations to use another name like blog.company.com , and let it point to a completely different IP address -- f.x. keep "www." on a hosting provider who is good at general hosting, and keep "blog." on another provider who specializes in blog hosting.</p>

<p>As I understand this <a href="http://videos.webpronews.com/2008/11/18/matt-cutts-on-changes-at-google/" rel="nofollow">interview with Matt Cutts</a> (~8 minutes in), the differences in sub-folders versus sub-domains has been diminished in Google's rankings. Maybe other (older) search engines still care a lot, but Google does not see the difference as large as they used to.</p>

<p>Thus you should select either <code>http://blog.company.com</code> <strong>or</strong> <code>http://www.company.com/blog/</code>
based on a reasoned assessment of SEO properties, and what is more manageable for your day to day operation of your website infrastructure. In general, www.company.com/blog/ is "best", but only if it doesn't require large effort to set up.</p>

<p>Another thing is you should not move your current blog URL without good reason, a good effort into providing redirects for all published blog pages.</p>

<p>Another question is to "www." or not. Here is <a href="http://www.codinghorror.com/blog/archives/001109.html" rel="nofollow">one fair opinion</a> -- above all, just be consistent.</p>



## Answer 10505

- posted by: [Hector Ramos](https://stackexchange.com/users/-1/514-hector-ramos) on 2010-04-22
- score: 4

Are you asking if blog.site.com is better than site.wordpress.com?
Or www.site.com/wordpress.com (?)

You should really try for blog.site.com. You are driving traffic to your homepage, not wordpress's. Yes, it's still your blog on both URLs, but why not make the URL part of your branding?

A subdomain at wordpress.com doesn't look professional, IMHO.


## Answer 10506

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-04-22
- score: 2

I am not quite sure what do you mean by "site/wordpress.com".
For SEO reasons I prefer domain.com/blog instead of blog.domain.com
I even prefer domain.com. where domain pages and blog post are managed by WP.


## Answer 10515

- posted by: [Scott Bennett-McLeish](https://stackexchange.com/users/-1/3208-scott-bennett-mcleish) on 2010-04-22
- score: 2

<p>Another thing to consider is what type of service you're providing. If you're a provider of a real-time service that if it goes down it will matter immediately to your customers, then you may also lose your blog.</p>

<p>Having your blog on a separate domain/sub-domain i.e. blog.company.com (and obviously hosted elsewhere) will allow you to update your customers with what is going on, what you're doing to restore service etc.</p>

<p>Lenny Rachitsky has covered a lot about ways to keep your customers informed on his blog <a href="http://transparentuptime.com" rel="nofollow">transparentuptime.com</a>.</p>



## Answer 24756

- posted by: [Sem Services](https://stackexchange.com/users/-1/10384-sem-services) on 2011-05-11
- score: -1

You can also use site.com/blog but blog.site.com is good option. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
