## Google Search Appliance (Google mini) for startups

- posted by: [Quintin](https://stackexchange.com/users/-1/2483-quintin) on 2010-02-08
- tagged: `google`
- score: 4



Is [Google Search Appliance][1] a good fit for a startup like Stackoverflow (just an example)? How does it fare?

I haven’t seen many examples or talk about this device being used in the startup circles. I need enhanced search experience with capabilities like stemming, spell check, relevancy, easy of indexing and retrieving and complete customization of the user interface (more than what Solr-Lucene or Autonomy provides today. In fact I am bowled over by Google Search Appliance labs). Also speed is of prime concern. With this in perspective I wonder why GSA is not gaining adoption among the non-enterprise crowd. Is there any reason in particular?

Additionally, do they have flexible pricing models for startups ($30,000 for 500,000 documents seems exorbitant at this time)?  This is to me is the primary deterrent... 


  [1]: http://www.google.com/enterprise/search/gsa.html



## Answer 7817

- posted by: [Doug G](https://stackexchange.com/users/-1/2107-doug-g) on 2010-02-09
- score: 1

I got a demo of it around a 2 years back and it really fell short from an application integration standpoint. It also had limited ability to handle complex permissioning rules as to who can see what data.  We instead implemented a Lucene solution and have been very happy.  You can get similar spell checking like google by loading your index up with multiple versions of each word (ie strip out all vowels etc).

Haven't looked at it since then, so it could have changed a lot in that time.


## Answer 8550

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-02-25
- score: 1

<p>If you want a search engine for just your web site there are <strong>much</strong> more flexible tools than the Google Search Appliance. We use <a href="http://www.wrensoft.com/zoom/index.html" rel="nofollow">Zoom</a> for our web sites. It offers:</p>

<ol>
<li>Complete customization of the results page</li>
<li>You control the search algorithm itself and item relevancy</li>
<li>Very easy indexing</li>
<li>$299 for the Enterprise version</li>
<li>Works with php, ASP, ASP.NET, CGI, or JavaScript</li>
</ol>



## Answer 7803

- posted by: [user161](https://stackexchange.com/users/-1/161-user161) on 2010-02-08
- score: 0

Last time I checked the license did not permit you to use it for a public application's search functionality.  And why bother with it when there are better solutions out there which will be easier to integrate directly into your app?


## Answer 7842

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-02-09
- score: 0

<p>You could take a look at <a href="http://www.microsoft.com/enterprisesearch/en/us/" rel="nofollow">Microsoft's Search offerings</a>. The Express edition is free of charge, runs on Windows, and is pretty easy to install. I don't know if there are any license or technical limitations that would exclude it for public website use.</p>



## Answer 8555

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-02-25
- score: 0

We are building a new service (<a href="http://outsearch.net">http://outsearch.net</a>) that is I think very close to what you are looking for.

It is a SaaS service for building custom search engines, with schema and ranking customization, while keeping everything really easy to use.

We essentially saw this need ourselves. Google custom search has too many constraints and most other decent solutions require "doing it yourself"

Some of the features:

-- Realtime updates / search<br/>
-- Automatic scaling to any size of data -- pay as you go<br/>
-- Autocompletion and spelling suggestions<br/>
-- Public or private search engine<br/>
-- Solr and Lucene compatible<br/>
-- Multiple types and facades<br/>
-- Restful web services<br/>
-- Custom ranking of search results<br/>

At the moment we are getting ready for a private beta. If it sounds interesting, shoot us an email at: team@outsearch.net

We would love to hear your feedback in any case


## Answer 11193

- posted by: [Mark Bao](https://stackexchange.com/users/-1/58-mark-bao) on 2010-05-15
- score: 0

<p>I don't think you should use it for a startup. I highly suggest <a href="http://sphinxsearch.com/" rel="nofollow">Sphinx</a>, which is an open-source full-text search engine. It's used everywhere and is probably the most popular open-source search engine software. It has a ton of companion plugins for various languages, like Ruby, PHP and more.</p>

<p>Alternatively, you can try <a href="http://lucene.apache.org/solr/" rel="nofollow">Apache Solr</a>, which is a Java-based search engine. Also open-source.</p>



## Answer 14748

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-04
- score: 0

You can also try www.searchblox.com which is based on Lucene



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
