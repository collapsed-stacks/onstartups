## Legal implications of hosting a server overseas?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-03
- tagged: `legal`, `hosting`
- score: 1

I'm American, planning to incorporate a small business in the US or form an LLC for the liability protection.

I pay an American company for my own virtual hosting service, with the goal of running a very small online business. Technically, the virtual server can be located anywhere this company has offices. Currently, it is located in the UK.

My questions are:

1. Do I have to register my business in the UK as well? Even if I'm not targeting users from this country? In the future, some paypal/credit card transaction might occur there.

2. Would this apply if the virtual server were located in a different state than where I  live in the US (registering my business in another state just because my server is there)?

3. What happens with things like Akamai and distributed hosting - where your website and/or copies of it could be moving around the world dynamically? I can't imagine you would have to register in every possible country your website might be served from.


I was just wondering what the implications are, especially to #1 and #2.

Thanks



## Answer 13884

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-09-04
- score: 2

<p>I'm absolutely not an attorney, and this is not qualified legal advice. That said, I don't think the world is as easy as Bhargav and NetTecture's comments above indicate.</p>

<p><strong>First, of course it is <em>legal</em> to host a server overseas.</strong> Obviously.</p>

<p>The finer point is which legislation you are subject to, when it comes to stuff like customer's privacy, email advertisements/spam, personally identifiable information (especially credit card information), and taxation (sales taxes a.k.a. VAT in particular).</p>

<p>I'm a citizen of the EU. I'm pretty sure I could argue in court over here that you are subject to the <a href="http://en.wikipedia.org/wiki/Data_Protection_Directive" rel="nofollow">EU's data privacy laws</a> when doing business with me. After all I am a EU citizen, and the server that physically stores my data is also inside the EU. If you're a US company with a server on US ground, then I would have a harder time arguing that EU's data privacy laws apply, and the <a href="http://en.wikipedia.org/wiki/Safe_Harbor_Principles" rel="nofollow">Safe Harbor Principles</a> would seem a better fit.</p>

<p><strong>Is this something to worry about?</strong> I a decade in the business I have not heard of a startup getting into trouble over which jurisdiction its servers are hosted in. I would not worry about this; instead I would invest in sound principles on data handling. I.e. have good Terms of Service, don't store credit card information yourself but offload that to a 3rd party, and don't ever spam or resell email addresses. Regarding taxation -- it's a huge topic, one that I will not try to answer.</p>

<p><strong>To your questions:</strong></p>

<blockquote>
  <p>Do I have to register my business in the UK as well?</p>
</blockquote>

<p>What I have seen so far is: Almost all smaller US companies don't create subsidiary companies in the EU at first. Then when they grow 'large', they create subsidiaries over here -- f.x Amazon, Paypal and others have subsidiaries. If you get lots of sales in EU, you might need to register a company here to better serve your customers, or to comply with EU VAT laws. But not just because a virtual server is here.</p>

<blockquote>
  <p>What happens with things like Akamai and distributed hosting - where your website and/or copies of it could be moving around the world dynamically?</p>
</blockquote>

<p>Honestly, I don't think the laws have caught up with technology on this one. But in most cases, what Akamai would cache globally is less important stuff such as website CSS or images. The important information, such as personally identifiable information, is usually not spread around the globe but resides in a single (or max 2) datacenter(s).</p>



## Answer 13886

- posted by: [Dana Shultz](https://stackexchange.com/users/-1/1841-dana-shultz) on 2010-09-04
- score: 1

<p>I cannot address the UK. I can address the US, especially CA, where I am licensed.</p>

<p>Let's assume that your server were in CA and your business was formed in another state. As discussed in the post "<a href="http://dana.sh/aQUtLS" rel="nofollow">Doing Business in CA? Be Sure to Register</a>", the test for having to register in CA is whether your business is "entering into repeated and successive transactions of its business in this state, other than interstate or foreign commerce".</p>

<p>The test, thus, is whether you would have "repeated and successive" transactions within CA. (Interstate and foreign commerce are excluded because those are outside what a state can govern.) You have not provided enough facts about your business for me to hazard a guess as to whether this test would be satisfied.</p>

<p>Other states use various tests to determine whether contacts with the state are sufficient to require registration.</p>

<p>I believe that the practical answer to your question is as follows: Even if the test in a given state were satisfied, if you do not have an office in that state, it is unlikely that the state will find out about your business, <em>unless</em> the nature of the business is such that the transactions are subject to taxation by that state.</p>

<p>Disclaimer: This post does not constitute legal advice and does not establish an attorney-client relationship.</p>



## Answer 13873

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-09-03
- score: 0

I'm not an attorney and this is for entertainment purposes only.  Seek legal councel prior to making any decisions.

Your buying a service from a company and so responsiblity falls to the other firm on any permit requirements for their operation at each location.  You are not operating anything in these companies but paying someone for a service.  There is nothing to get a permit for.

http://www.business.gov/register/steps-to-register.html 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
