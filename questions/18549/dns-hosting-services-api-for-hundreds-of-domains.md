## DNS Hosting Services (+API) - For Hundreds of Domains?

- posted by: [Alex Cook](https://stackexchange.com/users/-1/6128-alex-cook) on 2011-01-05
- tagged: `domain`, `dns`
- score: 2

This is a follow up question to [http://answers.onstartups.com/questions/7600/dns-hosting-services][1] - hopefully it's okay that I post like this.

I'm running a business app where users move their site to our platform, and looking for a better solution for DNS hosting.

Does anyone recommend a DNS hosting service which is good for managing 100+ domains?

I'm currently using virtualmin and hosting my own DNS server - which I definitely don't want to do moving forward. It's automated now since we're using virtualmin, but it's not a good idea to host DNS on the same server as our web server.

DNSMadeEasy and other solutions like it make you manually create each record one at a time - which won't be possible for me since I'm looking to host 100-200 domains. Looking for a service that lets me create records via API or lets me directly edit the records file. 

I wonder why so many hosts and DNS services make you enter in each DNS record one-at-a-time through a gui...

Thanks all!


  [1]: http://answers.onstartups.com/questions/7600/dns-hosting-services


## Answer 18551

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2011-01-05
- score: 2

<p>Well, if you want a straightforward rest api, <a href="http://www.zerigo.com/managed-dns" rel="nofollow">zerigo</a> is a possibility. Dyn's <a href="http://dyn.com/enterprise-dynect-platform" rel="nofollow">dynect</a> soap api is also good.  Or use <a href="http://packages.debian.org/search?keywords=dbndns" rel="nofollow">dbndns</a> + mysql and program your own.</p>



## Answer 18590

- posted by: [Radek](https://stackexchange.com/users/-1/6382-radek) on 2011-01-06
- score: 2

Sounds like Amazon Route 53 should suit perfectly your requirements:

 - it is a webservice so you can automate it using API
 - as with every other Amazon AWS it will automatically scale for you with traffic
 - Route 53 is a relatively new service by the time of writing this so I cannot say how reliable it is but from my experience with other amazon aws products it should be great

See: http://aws.amazon.com/route53/


## Answer 18566

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-05
- score: 1

<p>Many registrars (companies that sell domains) offer that for free. Your existing one may be offering that already. Ask him.</p>

<p>I use <a href="http://www.gandi.net" rel="nofollow">Gandi</a> and <a href="http://www.ovh.com" rel="nofollow">OVH</a> to manage hundreds of domains. Gandi has an extensive API. I aslo use <a href="http://www.opensrs.com" rel="nofollow">opensrs</a> a lot.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
