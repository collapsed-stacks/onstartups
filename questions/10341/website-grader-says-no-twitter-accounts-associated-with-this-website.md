## Website Grader says "No Twitter accounts associated with this website"

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-17
- tagged: `twitter`, `blog`
- score: 3

When I run my blogs through the Website Grader, one of the things I'm dinged for is that no associated Twitter accounts are found. I have Twitter accounts for all my blogs, and the URLs are present in the Twitter profiles. Why would they not be found by the Grader?


## Answer 10744

- posted by: [Zuly Gonzalez](https://stackexchange.com/users/-1/2692-zuly-gonzalez) on 2010-04-30
- score: 2

<p>I had the same exact problem. Here's how you fix it:</p>

<ol>
<li>Run Twitter Grader on your Twitter account first.</li>
<li>Then run your website through Website Grader. </li>
</ol>

<p>If you run Twitter Grader <strong>before</strong> Website Grader, Web Grader should see the Twitter account associated with your website. Courtesy of Colin Warwick from <a href="http://inbound.org/questions/1082/why-doesnt-website-grader-see-my-twitter-account" rel="nofollow">inbound.org</a>.</p>

<p>Btw, my grade didn't improve after Website Grader found my Twitter account.</p>

<p>There's also an <a href="http://success.hubspot.com/content-library/bid/10302/FAQs-Website-Grader" rel="nofollow">FAQ page</a> for Website Grader that discusses other problems someone may have with it. This particular problem isn't addressed in the FAQ though.</p>



## Answer 10351

- posted by: [Chris W. Rea](https://stackexchange.com/users/-1/953-chris-w-rea) on 2010-04-18
- score: 1

<p>While I don't know exactly how Website Grader is implemented, as a software developer I can imagine that it wouldn't be <em>feasible</em> for Website Grader to go through all of the millions of twitter accounts to find the one that has a URL pointing to your blog (unless there's a reverse-lookup API at twitter that I wouldn't be aware of.)</p>

<p>In any case, here are some suggestions I have for you to consider:</p>

<ul>
<li><p><strong>Do you have a link from your web site home page to your twitter profile?</strong></p></li>
<li><p><strong>Is your twitter user name the same as the root of your domain name?</strong><br>
 e.g.&nbsp; <code>mycoolblogsite.com</code> &nbsp;&nbsp;and&nbsp;&nbsp; <code>@mycoolblogsite</code> ?</p></li>
</ul>

<p>I am guessing that Website Grader would use one or both of those methods to initiate the test, and then check that the twitter account located that way also leads back to your site.</p>

<p>I had set up <a href="http://www.basicallymoney.com" rel="nofollow">my site</a> and <a href="http://twitter.com/BasicallyMoney" rel="nofollow">twitter profile</a> consistent with those methods and Website Grader found my twitter account.  So, try each and see which works for you.  BTW, if you find it's one and not the other that does the trick, please come back and report your findings :-)  Good luck.</p>



## Answer 10365

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-19
- score: 0

Unfortunately, both of those considerations are true in my case.
1- There is a link in the Twitter profile connecting it to the blogs. (There is a link on the home pages themselves, and there is a link in the Profiles of my accounts)
2- And the Twitter username is the root of the domain in 3 out of 4 cases (4 separate blogs). One of the domain roots was too long to use a Twitter name, but this can't be the issue I'm having the same problem with the other blogs.

Coud it have something to do with the fact that my blogs are hosted on Wordpress.com? I am not using .wordpress.com domains.  I own all of my own domains, and they are mapped to wordpress.

Any other thoughts?  This is a frustrating issue, because I imagine that having a visible associated Twitter account is a fairly important thing for page ranking and I want to make sure this gets resolved.

Thanks so much for your help!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
