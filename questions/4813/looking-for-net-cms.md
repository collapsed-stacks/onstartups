## Looking for .NET CMS

- posted by: [Dimitri](https://stackexchange.com/users/-1/1850-dimitri) on 2009-12-09
- tagged: `website`, `technology`, `application`
- score: 3

I'm looking for .NET content management system.

I've done some research and found a lot of software (like Telerik's Sitefinity or DotNetNuke), but I don't want to make wrong decision. Please advice.


## Answer 6244

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-01-09
- score: 5

We were part of a program that evaluated Sitefinity and DNN, and ultimately selected Sitefinity.  This particular project was to replace an existing business system with a new system that met the business application needs of the prior system plus added content management, customer-specific portal capabilities and other traditional CMS features.  This meant that the underlying CMS was going to have extensive business functionality implemented on top of it.  

The project is currently about at its midpoint - half published, half still being implemented but the choice of Sitefinity has panned out well; Good support and release management has made it easy to accommodate updates from the vendor into a rigorous configuration management process so the team can safely take advantage of updates from the vendor while simultaneously (and aggressively) adding new custom functionality.

In the end one key piece of advice I'd have is pick one based on what's most important to you and then go forward without any regard to those you didn't pick.  There are hundreds of ways you could get this done and each has their trade offs.  Just make your call and then move on to providing value.  If you get absolutely jammed up with something that doesn't appear that it will work, try a focused side project with an alternative technology first to validate that life really is better before porting.  It's very easy to trade the problems you know for a new system that has problems hiding in the dark; what you don't know you don't know can really hurt.


## Answer 22042

- posted by: [Stuart](https://stackexchange.com/users/-1/8316-stuart) on 2011-03-22
- score: 2

What is the site you are building.

The best CMS to choose is really dependent on what your site requires.

- DNN is a solid general performer and has a **lot** of commercial extensions available - but I've personally really not enjoyed extending it recently - just find it too unwieldy to get look and feel right everywhere.
- Umbraco comes with a lot of recommendations.
- Orchard is the rising star from Microsoft - but is built around "Wordpress" like functionality at its core - so if your core is also a blogging/news site then this is a good choice.
- Commerce platforms like nopCommerce provide good CMS functionality alongside excellent eCommerce tools.
- there are commercial-only offerings like Telerik SiteFinity/Community Server available - but I've personally steered clear of these so far.

It all depends on what you need. 

**Sort out your site requirements before you select the CMS**


## Answer 4819

- posted by: [Frank](https://stackexchange.com/users/-1/1827-frank) on 2009-12-09
- score: 1

The place I am currently contracting at uses ektron and it works but as Guillaume said, trying to extend it is difficult, use open source if you can.  They tried to do something a little different with the menuing system and what should have been a few lines of code in the source turned out to be a complicated nightly process.  You might also want to checkout this one, it is open source c# and does the very basic out of the box:

http://www.mojoportal.com/home.aspx

You also have the option of rolling your own with .Net.  There is a great manning book that explains how to use the web parts in .net 2.0, which is what sharepoint 2007 is built on.

http://www.manning.com/neimke/




## Answer 4820

- posted by: [Steve Wortham](https://stackexchange.com/users/-1/1791-steve-wortham) on 2009-12-09
- score: 1

<p>There are a couple I've been researching that may interest you:</p>

<p><a href="http://umbraco.org/" rel="nofollow">Umbraco</a> and <a href="http://orchard.codeplex.com/" rel="nofollow">Orchard</a> </p>

<p>Both have the distinction of being heavily customizable.  Both are open source and have free versions.  But Umbraco also has paid versions that include support.  </p>

<p>And although Orchard seems promising, it looks like Umbraco is a much more complete and mature product at the moment.  If I were to pick one that has the best chance of being supported for years to come, I'd choose Umbraco.</p>



## Answer 4836

- posted by: [Puk](https://stackexchange.com/users/-1/1859-puk) on 2009-12-09
- score: 1

Having just delivered a large multi site platform over Microsoft's internet enabled version of SharePoint (MOSS) - I would not recommend going that route. Many features that you would expect to be available (Rich Text editing, multilingual support, code release processes) had to be hadn crafted.

If repeating the project I would seriously consider SiteCore. It has the advantage of being in continuous development for around 10 years and have many important features integrated already (personalisation, page optimisation, SEO tools, forms without developer input, easy landing pages, forums, blogs...). I have no affiliation.

Yes I guess you loose some flexibility  over a pure open source option, but if you are in a position to focus more on content than unique business functionality then you don't need the flexibility. Any new functionality developed carries a code risk and maintenance burden. After a few years of evolution you can easily find yourself with a dense weed garden of code that no wants to touch. In fact I've seen an inexperienced team achieve that in under a year.




## Answer 6493

- posted by: [Chris Dansie](https://stackexchange.com/users/-1/2053-chris-dansie) on 2010-01-13
- score: 1

I've heard and seen good things about http://www.kentico.com/. You might give that a try.


## Answer 22030

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-03-22
- score: 1

<p>I've used <a href="http://umbraco.com/" rel="nofollow">Umbraco</a> before and found it to be pretty good for a .NET CMS.</p>



## Answer 4815

- posted by: [Guillaume Justier](https://stackexchange.com/users/-1/1636-guillaume-justier) on 2009-12-09
- score: 0

It mainly depends on four things, but since I don't know if this is for a client project or for an internal project (because the criteria would be different).


**1. Your budget**

Depending on the size of the project, you might find that spending thousands of dollars on a CMS is not an option, so open-source would be the way.
 If it's a client project the cost of the CMS will have to be factored in your quotation, and you could price yourself out if you don't choose wisely.

**2. Preconceived ideas**

I run a web agency, and we program in both MS languages and PHP, depending on the project. Well, some clients insist on one technology (usually microsoft) because they don't know PHP and they fear something free won't be as good. The same could apply to CMS: Your client might be wary of DotNetNuke because it's free ("so it can't be as good"). In that case you can either try to educate them, or choose a commercial CMS.

**3. Flexibility required**

At my agency we almost always go for open-source. Not for the price, but for the flexibility: If there is a feature missing we can develop it. If we go for a commercial solution, your options are limited if a feature is missing (you have to wait for the vendor to implement it).

**4. Support required**

You (or your client) might feel more comfortable with phone support, in that case you most likely need to go commercial.


For what it's worth, we investigated .NET CMS a while back, and we would have gone for DotNetNuke (for reason 3 above). Commercially, we looked at http://www.ektron.com/cms400.aspx and they were very helpful in installing demo versions, etc.. The project didn't happen in the end, so we didn't implement any CMS live, so I can't comment on the after sales support.



## Answer 22108

- posted by: [ct1](https://stackexchange.com/users/-1/8765-ct1) on 2011-03-23
- score: 0

N2CMS is very good CMS (my preferred). It works with MVC and various databases. But the documentation is poor, I found it not easy to develop for. 
MojoPortal is also very nice.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
