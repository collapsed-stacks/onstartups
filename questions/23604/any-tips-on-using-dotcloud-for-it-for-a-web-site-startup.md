## Any tips on using DotCloud for IT for a web site startup?

- posted by: [Warren E. Hart](https://stackexchange.com/users/-1/2058-warren-e-hart) on 2011-04-18
- tagged: `it`, `cloud`, `applications`
- score: 4

I came across [DotCloud][1] this weekend. It looks like an awesome way to build a web based startup with pre-configured modules. 

Here's how they position themselves:

"Assemble your stack from pre-configured and heavily tested components. We support major application servers, databases and message buses. If we don't support it, ask."

I went through their FAQ and tutorials - looks pretty solid. They offer a broad range of components already - from Apache to Casandra to Hadoop to Python and lots more. 

Has anyone used it and do you have any tips / suggestions? 

Thanks. 


  [1]: http://www.dotcloud.com/


## Answer 23704

- posted by: [edralph](https://stackexchange.com/users/-1/9362-edralph) on 2011-04-20
- score: 3

<p>Over the last 10 years I've helped take a web based startup to $1bn market cap in 10 years.  Being responsible for the in-house software development, sys-admins and the co-located infrastructure meant that we had to worry about <em>everything</em>.  Sometimes that hurts.</p>

<h2>Platform as a Service</h2>

<p><a href="http://www.dotcloud.com" rel="nofollow">DotCloud</a>, <a href="http://www.heroku.com" rel="nofollow">Heroku</a> and <a href="http://www.phpfog.com" rel="nofollow">PHPFog</a> are a few of the new breed of services known as PaaS - platform as a service.  If I were starting a web-based company today, I would be seriously considering using one of these platforms so that I don't have to worry about IT infrastructure.</p>

<h2>Why not rent dedicated servers...</h2>

<p>You may be thinking though that by renting a dedicated server you're not worrying about the infrastructure.  Perhaps not so much while a single dedicated server is enough.  But if your business succeeds, you'll probably need more than one server.  Then you have to start thinking about load balancers and then you'll need to start thinking about CDNs like <a href="http://www.akamai.com" rel="nofollow">Akamai</a>.  You'll need to worry about off-site data backup and disaster recovery.  There are tons of things that can keep you up at night.  </p>

<h2>Keep your headcount focused</h2>

<p>PaaS packages up your infrastructure so that all you need at your end are developers that push their code up to the platform.  When the web-app starts groaning, you go into the control panel and increase the resources available to your app.  No messing around with renting/buying another server, no worrying about load balancing algorithms and wondering why session persistence doesn't work.  No need for infrastructure folks.  Sorry sys-admins.
Adopting PaaS means that the first developer you hire can be just that - a developer - they don't need to know that much about web infrastructure and how to assemble lamp stacks etc.  You can focus on getting a good developer; give them the tools and the PaaS and away you go.  Focus your headcount on your product, not support.</p>

<h2>Isn't PaaS risky for my new business?</h2>

<p>PaaS is new ground.  Some of these companies won't make it but I believe that the idea will succeed in the long run and they'll be here to stay.  Despite the risk of your chosen PaaS provider going under, the risk to you is minimal.  In that scenario all you need is to have another PaaS provider that supports the same development environment as you and if you are unhappy with your primary provider, just push your codebase to the other provider and you're up and running again.</p>



## Answer 23643

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2011-04-19
- score: 2

<p>Amazon offers a similar platform as a service, <a href="http://aws.amazon.com/elasticbeanstalk/" rel="nofollow">Elastic Beanstalk</a>. DotCloud does just use Amazon EC2 btw.</p>

<p>But <a href="https://elasticserver.com/" rel="nofollow">Elastic Server</a> offers the same idea, one layer up. You put together the platform using standard packages, but you can get the same server packaged for Amazon, Xen, VMWare, etc. It's generic components on a generic platform, about as abstracted as you can get...</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
