## SaaS Solution and Hosted Solution... is there a difference? (Enterprise)

- posted by: [Big Tuna](https://stackexchange.com/users/-1/1702-big-tuna) on 2011-02-19
- tagged: `saas`, `enterprise`
- score: 1

When it comes to enterprise software, would you say there is a difference between a hosted solution and an SaaS solution?  Or are they the same thing? 

If there are differences and you offered a "hosted" solution would you still use a "subscription" based pricing model?


## Answer 20528

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-02-21
- score: 4

Hosted and SaaS are different:
  - Hosted means the software you access is not on your own infrastructure, it is "hosted" by someone else. That means that you could have bought a bunch of software and have them hosted. This is not SaaS.
  - SaaS is software that you pay as you go (as a service) and there lies the difference.

Now let's bring a bit of confusion: A SaaS application is usually hosted.. But a Hosted solution is not necessarily a SaaS solution.

To answer you question about subscription, SaaS is "pay as you go", so it is subscription based (otherwise the provider wouldn't be able to stop the "service" if you stop paying). But a hosted solution will have a subscription on the hosting part, not necessarily on the software you access (and that is hosted).

Let me know if you need more clarity.


## Answer 20496

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-20
- score: 0

An hosted solution is usually what offer SaaS providers.




## Answer 20503

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-20
- score: 0

A "Hosted" solution is when a third-party is used to house IT infrastructure, be it hardware-only (customer owns, loads, and runs the apps), software-only (1 or 2 separate 3rd parties may be involved, one provides the remote cloud (aka data center) and one provides the remote application management (usually one 3rd party hires the other, but some companies have remote management of apps that are located at an internal location).

SaaS is software-based, butit too can appear in various ways, inlcuded hosted SaaS. Take a video SaaS vendor (stores IP video remotely for others). It can look like a software-only hosting option where the vendor runs the video app,but customer finds colocation space to host it. Or the SaaS vendor can also own the data center, and sell the app by the computing slice charging you both for the hardwar cpu cycles used and the number of users on the app or the number of computing cycles that the app takes.  So SaaS can be billed for software-only, or both hardware and software.


## Answer 20546

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-02-21
- score: 0

These are both slippery terms, and there's definitely overlap.

SaaS generally implies that the provider has a system somewhere in the cloud, and that as a customer I pay for software features and utilisation rather than for the platform hosting as such.

Hosted solutions are often software that you could install for yourself, and as an option you can access the service through the cloud. It's commmon - but not universal - to find that payment for hosted services mirrors the underlying software's pricing structures plus structures common in 'raw' hosting.

But the difference is really more a matter of convention than anything. I've certainly seen companies who seem totally SaaS to me position their services as 'hosted' in order to connect better with enterprises who like 'cloud,' know what 'hosting' is but are not decided about SaaS. And I've seen common software packaged up with hosting and called SaaS to differentiate from commodity hosts.


## Answer 20548

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2011-02-21
- score: 0

Definitions vary all over the place, so your results may vary. This works for me.

> **Hosting** - running and maintaining a computer system on someone's behalf.
> 
> 
> **SaaS** - Software-as-a-Service is a model of software deployment whereby a
> provider licenses an application to
> customers for use as a service on
> demand. One example of SaaS is the
> Salesforce.com CRM application.
> 
> **IaaS** - Infrastructure-as-a-Service is the delivery of computer
> infrastructure (typically a platform
> virtualization environment) as a
> service. Rather than purchasing
> servers, software, data center space
> or network equipment, clients instead
> buy those resources as a fully
> outsourced service. One such example
> of this is the Amazon web services.
> 
> **PaaS** - Platform-as a-Service is the delivery of a computing platform
> and solution stack as a service. It
> facilitates the deployment of
> applications without the cost and
> complexity of buying and managing the
> underlying hardware and software
> layers. PaaS provides the facilities
> required to support the complete
> lifecycle of building and delivering
> web applications and services. An
> example of this would the GoogleApps
> or Heroku.

So, whether its SaaS, IaaS, Paas - its all "hosted" - that is, running somewhere other than on your hardware, and you pay for it (of course, there are hybrid solutions that incorporate your hardware + their hardware, but let's keep it simple for now.) 

How you pay - per use, monthly, quarterly, annually - is a condition defined by the provider and not a deciding factor on what type of provider it is.  


## Answer 20606

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-02-22
- score: 0

Most software vendors that offer hosted solutions will install their software on a server and network that they manage for you. In the enterprise, a company may want to start with a hosted solution and then bring it in-house as their company and infrastructure grows (We're hiring a network admin and buying servers for other purposes, might as well bring the app in-house and save money and get a better connection.). Some companies may prefer this option instead of purely SAAS with no chance bringing the data in-house.

You can buy an annual contract for the software and then pay monthly for the additional hosting. Number of users is generally tied into the cost.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
