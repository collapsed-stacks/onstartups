## Can I give Google Analytics data to my customers?

- posted by: [Daxon](https://stackexchange.com/users/-1/12333-daxon) on 2011-07-30
- tagged: `google`, `analytics`, `business-services`, `api`
- score: 2

Can I give Google Analytics data from the API as a free gift feature to my customers that are paying for a monthly subscription service? Or would this be outside of Googles terms of service.


## Answer 28992

- posted by: [JonDiPietro](https://stackexchange.com/users/-1/11642-jondipietro) on 2011-08-18
- score: 2

The short answer is, "yes." You can add anyone you want to an analytics account so that they can access the data. Also, you can set up automated reports to be emailed to them on a regular basis.

However, I think think there is a danger to listing this as a "free gift" because it is already free. If your customers gain access to this feature and realize that they could be accessing it for free without you, it may create ill will. I'm just saying be careful how you present it to them.


## Answer 28993

- posted by: [Craig Saboe](https://stackexchange.com/users/-1/12715-craig-saboe) on 2011-08-18
- score: 1

As Jon pointed out, you can have regular reports emailed to customers. The great thing about this (as opposed to giving direct access) is that you can create simplified reports that are easy for non-technical people to grasp - and you retain control.

Also, you don't need to reveal who's providing the service - Google does insert a "Google Analytics" at the very bottom-right of the report, but I'm not sure if you can remove this or not. Not a lot of your customers might realize this or even care.

Thirdly, there are other options besides Google Analytics - your hosting provider (if you're using shared hosting or reseller accounts) often will give you access to your logs and stuff as well as some software for processing that. Check that out as well.

Lastly, you can check out the open source Piwik app; it's a PHP app that offers a lot of analytics functionality, and you can rebrand it yourself. I liked what I saw when I evaluated it a while back - check that out as well.

Hope this helps!


## Answer 29058

- posted by: [Alex](https://stackexchange.com/users/-1/12744-alex) on 2011-08-19
- score: 0

<p>Depending on how many users you have accessing it on behalf of your account, you may quickly run into the <a href="http://code.google.com/apis/analytics/docs/gdata/gdataDeveloperGuide.html#quota" rel="nofollow">limits put on the API</a>. Basically it states:</p>

<p>Each API request is limited to a maximum number of 10,000 entries per response. The default is 1,000 entries per response and can be increased using the max-results query parameters.</p>

<p><strong>Data Feed</strong></p>

<ul>
<li>10,000 requests per 24 hours per web property (i.e., all the profiles/table IDs within one web property). This quota is replenished every midnight, Pacific Time.</li>
<li>10 requests in any given 1-second period (10 qps) per IP address across all Data Export API queries</li>
<li>4 concurrent requests at any given time per IP address (i.e., you must wait until your 1st request completes before making a 5th request)</li>
</ul>

<p><strong>Account Feed</strong></p>

<ul>
<li>10 requests in any given 1-second period (10 qps) per IP address
across all Data Export API queries</li>
</ul>

<p>If your customer base is large enough that this may be an issue, your best option may be to just pull the data yourself and then generate your own automated reports for them.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
