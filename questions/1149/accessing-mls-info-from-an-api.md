## Accessing MLS info from an API

- posted by: [kmullings](https://stackexchange.com/users/-1/548-kmullings) on 2009-10-13
- tagged: `software`, `web`, `api`
- score: 5

Are there any applications out there that provide an API for accessing US property listing (MLS) information? [Zillow][1] has property information for most of the country but very little listing information.

Thanks.


  [1]: http://www.zillow.com/


## Answer 1172

- posted by: [dlynton](https://stackexchange.com/users/-1/482-dlynton) on 2009-10-13
- score: 3

Each local MLS market is different. I'm in Houston, and HAR only offers direct API access for broker accounts. Otherwise you have to use an iframe or simply link to their website. I believe other local MLS policies are more lax. What you're looking for is IDX - that is the standard API among MLS services.

Here are some related links: 

http://www.realestatewebmasters.com/thread13976.html

http://www.listingware.com/index.cfm

http://www.verticalagent.com/products/national-mls.aspx

http://www.onboardinformatics.com/


## Answer 1256

- posted by: [mgile](https://stackexchange.com/users/-1/736-mgile) on 2009-10-13
- score: 3

<p>As a follow-on to dlynton's post, the actual standard in play here is called RETS (Real Estate Transaction Standard), which can be found at: <a href="http://www.rets.org/" rel="nofollow">http://www.rets.org/</a></p>

<p>There are open source libraries in C++, PHP, Java and others that can help you write applications to integrate with RETS servers.  But as noted, you are at the mercy of the regional MLS owner, which is different in every area.  </p>

<p>I've seen some services that offer MLS aggregation services so that you can create a nationwide MLS software application, and these typically run about $30-$100 per month for access.</p>



## Answer 1153

- posted by: [Brandon](https://stackexchange.com/users/-1/18-brandon) on 2009-10-13
- score: 1

Probably not for your purposes. The data is owned by the REALTORs and is not made public in the form of an API. If you became a REALTOR or were contracted by a REALTOR, you might be able to access the MLS through an API. 

If you're still interested, perhaps the best thing to do is contact the local Board of REALTORs in your area. Alternatively, find the most tech-savvy REALTOR in your area and contact them directly. They may know more about the details.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
