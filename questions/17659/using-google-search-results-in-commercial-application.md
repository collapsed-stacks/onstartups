## Using google search results in commercial application

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-12-10
- tagged: `google`
- score: 2

I would like to develop a commercial application that uses the results of the Google AJAX Search API. For example: if user types the word "starbucks breakfast blend", the application will use the Google search API to retrieve all results, mine them in the background, and show results that it 'thinks' are relevant.

Does Google allow commercial applications to live off it's search results? If not, are their alternatives (paid/open source) that I may use?

The code base is primarily in Java.



## Answer 17660

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-10
- score: 1

@neelsheyal, Google allows custom search but for a small fee, otherwise you are very limited in the way you display results.

For free you can use the Google Custom Search:
http://www.google.com/cse/

For a payment you can use Google Site Search:
http://www.google.com/sitesearch/#utm_campaign=en&utm_source=en-ha-na-us_ca-bk&utm_medium=ha&utm_term=google%20site%20search

A better alternative, and the one I use is the Bing Search API.
Specifically the Bing 2.0 API
http://www.bing.com/developers/

The Bing Api Is Free!  Its ad free, and amazingly quick.  There are already some libraries for searching through JSON, C# etc.  But since the results are XML you can process them however you want.  I recently wrapped up a project that used Bing Search using Classic ASP, and we used some Jquery code to make our own version of Instant Search Results which came out very nice. 

With Both Google and Bing you have to do a little bit of programming.  I think you are better off going with the one that is free.

2nd note.  Google indexes far more pages than bing does.  Using the bing search API makes sure we focus on making sure that all search engines index our pages not just google.  It almost forces you to focus on better SEO which is a good thing.

Let me know if you need some code samples. 







## Answer 19407

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-25
- score: 0

Are you sure about this?  I have the same question and here is what I pulled from the Bing site.  This sounds like I can't use it to store results.  I still can't find anything that tells me if I can use Google Ajax Search API either.


From Bing's terms of service: http://www.bing.com/developers/tou.aspx
"2. WHAT RIGHTS DO I HAVE?  Solely to the extent that you are in compliance with all terms of this Agreement, we grant you a non-exclusive, non-transferable, non-sublicenseable license to use the services to: enable your Website or application to obtain Bing results; make limited intermediate copies of the Bing results, solely as necessary to display them on your Website or application; and host and display Bing results on your Website or application.  Your license to use the services is limited, however, to solely your Websites and applications.  You are responsible for your own conduct and content while using the services and for any consequences of this use.  All queries to the Bing services that you provide must be user initiated and refineable by the user.
You will not, and will not permit your users or other third parties to:
 (n) copy, store, or cache any Bing results, except for the intermediate purpose allowed in §2(b);
     (o) commercialize (i.e., sell, rent, or lease) Bing results;
 ....




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
