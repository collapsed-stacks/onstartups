## Customer / public Wiki Suggestions

- posted by: [Gregg](https://stackexchange.com/users/-1/18132-gregg) on 2012-05-28
- tagged: `customer-support`
- score: 1

Before launching our startup, we are attempting to have a large portion of the documentation for the product complete.  However, we're a bit stranded when it comes to the best presentation of that information.  We want to go with a wiki but what I'm finding available aren't the most user friendly nor do they look that great out of the box (MediaWiki, for example).

But I want to mention the following as well.  We have the following pieces to customer interaction planned:

1. Support Cases: Probably SaleForce with desk.com
2. Knowledge Base: Ties into the support system.  This is for common questions to common support related issues.
3. Customer/Public Wiki: This is more geared towards the software engineers who will be using our product.  We have an API, and SDK, and we really want to utilize this medium for documenting all those aspects of our product.

3 is where I'd appreciate some advice on possible solutions.  Preferably those that will work in a PHP or Java server stack.


## Answer 39463

- posted by: [futureal](https://stackexchange.com/users/-1/18012-futureal) on 2012-05-29
- score: 2

<p>For (1) and (2), it sounds like you already have the solution planned out. Desk.com integrates the knowledge base functionality with the support system by default, and exposes answers (that you control) to your website with some basic integration. You can <a href="http://www.desk.com/product?__lsa=040f4ad2#sec6" rel="nofollow">read more about that here</a>. </p>

<p>For (3), there are a few things to consider. First, most developers have grown accustomed to basic API/SDK documentation standards, and there is really no good reason to deviate from those. Both <a href="http://www.oracle.com/technetwork/java/javase/documentation/index-jsp-135444.html" rel="nofollow">Javadoc</a> and <a href="http://phpdoc.org/" rel="nofollow">phpDocumentor</a> are capable of generating familiar, browse-able documentation, so make sure your developers include the proper documentation in their code, and then auto-generate new API docs with each release. There is no substitute for this kind of clear, commonly-formatted API documentation.</p>

<p>Were it up to me, you really don't want your users contributing to the <em>documentation itself</em>, but rather contributing things like code samples, "cookbooks", and that sort of thing. If you find that your users need to augment the API documentation itself, chances are your documentation is lacking somehow.</p>

<p>As for a tool to do this, as you suggested a Wiki is often the best way to go. MediaWiki is good in that most people know how to use it, but for a more professional looking and easy-to-use software, I'd suggest <a href="http://www.atlassian.com/software/confluence/overview" rel="nofollow">Confluence from Atlassian</a>. The downside is that this is a much more expensive option; Confluence is priced more for internal use and can be costly to deploy in an unlimited-user situation. There are other options out there as well that may strike a balance between these two.</p>

<p>Finally, it is likely that your users will find issues with your API, create workarounds, develop really cool add-ons, and so on. It is important to manage your user-contributed works in such a way that these facts are tied to specific versions of your software, since as your company hopefully grows, you will eventually have many versions and many users of each version. When you do deploy documentation and/or a collaborative tool, make sure you can easily segregate content by release version. It's also a good idea to expose some or all of your defect tracking solution to end users, both to help them understand what is in progress, and to leverage them as a global QA resource.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
