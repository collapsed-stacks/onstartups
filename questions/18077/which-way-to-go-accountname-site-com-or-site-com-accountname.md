## Which way to go - accountname.site.com or site.com/accountname?

- posted by: [ncakmak](https://stackexchange.com/users/-1/4028-ncakmak) on 2010-12-21
- tagged: `best-practices`
- score: 5

I have recently been tasked with developing an online portal for the real estate agents. I am planning to make the code as generic as I can so that I can use it as a product for the other industry shareholders such as mortgage lenders, small local bankers, closing attorneys, etc..

Each agent will have his or her own content pages (like about the agent, available properties, recently sold, call now, contact, etc.) with specific individual information. As a result, each agent will have a dedicated PURL.

What is the most user-friendly way of creating these types of PURLs?

I know that there are 2 main ways with different approaches:

**accountname.site.com**

Account name can be FirstNameLastName (as long as it is unique), dynamically generated by the server or let the agent decide what it would be with some limitations. I guess this is more like creating a subdomain.

There are great examples to this way:

http://123.wordpress.com

http://123.weebly.com

http://123.blogspot.com

http://123.netlibrary.com

**site.com/accountname**

Similar approaches that I gave above apply here too. Account name can be firstname.lastname (as long as it is unique), dynamically generated by the server or let the agent decide what it would be.

There are great examples to this way too:

http://linkedin.com/456

http://twitter.com/456

http://cvonthe.net/456

http://flavors.me/456

http://ted.com/456

Some are even combining both ways:

http://DealerName.audi.com/SalesmanAccountName

Technically speaking, I will be employing URL Rewrite method (unfortunately on IIS 6) therefore both ways are doable and will probably take same amount of time on my end.

Looking forward to your suggestions.

Thank you!

---

This question is actually an extension of the following question:

http://answers.onstartups.com/questions/17909/offering-different-authentication-ways-to-non-technical-users



## Answer 18078

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-12-21
- score: 6

"accountname.site.com" will get a little unwieldy if you grow to several thousand accounts *and* need multiple frontend hostnames (say multiple load balancers) at the same time. It is possible to handle this with both "site.com/accountname" and with "accountname.site.com", but it's simpler in the former case.

With "login.site.com" or "www.site.com/login/" you have a single DNS record that needs a 'fancy' configuration ("login" or "www" in my example). You can assign multiple IP addresses, or use split horizon DNS for this specific record, or even offload the DNS subzone completely to a 3rd party geo-aware DNS provider.

With "accountname.site.com" each "accountname" could/should be a separate DNS record. Actually this gives you have far more flexibility, but to use that flexibility would require a more complex application, where the account provisioning logic is connected to your public DNS.

But while the above future growth consideration is valid, it may also be premature to worry about it now. You don't have several thousand accounts yet. :-)

**Personally, I like a single place to log in, with a single form** (email address and password) as the simplest option and most common option. The place to log in could be "login.site.com", or just a login form in the top right of your main website (www.site.com).

**There is another thing I think you should consider.** Perhaps your real estate agents would really really want "vanity domains", i.e. "shop.estate-agent-domain.com"? It's common among small business owners to want to 'own' the branding and external marketing. Vanity domains can be accomplished in many ways, the easiest is generally:

 - Have a 'gateway' server, a specific front-end application server with the right software in place to handle many virtual hostnames.
 - Having a single DNS hostname for your gateway server, i.e. "gateway.site.com" 
 - The real estate agents map an hostname of their own choosing as a CNAME to "gateway.site.com", i.e. "shop.estage-agent.com" *points to* "gateway.site.com".
 - Real estate agents configure their domain info inside your application.
 - The application server code on "gateway.site.com" looks in the HTTP 1.1 header for the domain name, and returns the appropriate customer-specific content.

HTH,


## Answer 18090

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-12-21
- score: 6

client.sitename.com.

Here are the reasons:
Each subdomain is treated by search engines as a different site.  Users of your site can add a domain instead of their subdomain by using a CNAME.  This is a lot cleaner than the approach of redirecting .

The challenge you run into with that structure is:
1. You need a static IP so you can do wildcard hostnames. 
2. If you end up offering your own real domain service then make sure you manage your own dns via api, this is important in case your server IP changes or if you need to split up the sites among servers.  Zerigo is good for this. 

Also with the subdomain strucutre you could do some really neat things:  frank.example.com/photos/  or frank.example.com/resume/   versus example.com/frank/resume

Also, you could redirect www.site.com/username to username.site.com with url rewrite redirects. 


## Answer 18080

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-12-21
- score: 0

My doubt is that when using client.zzz.com competition will be more easily to revel the names of you clients. 
For security reasons it will be better to use zzz.com/client


## Answer 18244

- posted by: [ncakmak](https://stackexchange.com/users/-1/4028-ncakmak) on 2010-12-27
- score: 0

Thank you for all of the responses.

I printed all these comments and answers, and showed them to the customer when we met face to face.

We finally ended up with the "accountname.site.com" option because of its future flexibility.

I wish all of you and OnStartups.com members a happy new year!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
