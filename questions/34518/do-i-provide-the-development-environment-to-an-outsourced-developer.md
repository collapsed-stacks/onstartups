## Do I provide the development environment to an outsourced developer

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2012-01-07
- tagged: `development`, `saas`, `outsourcing`
- score: 0

If SaaS development is to be outsourced, do i need to provide the development environment for the developer, I mean is it pretty much a standard thing to do? Or a choice made out of personal preference.

By development environment I mean the hosted environment. 


## Answer 34521

- posted by: [dnbrv](https://stackexchange.com/users/-1/15284-dnbrv) on 2012-01-07
- score: 2

An outsourced developer should have their own tools of trade. The fee you're paying them is supposed to cover all of their operational expenses. After all, when you hire a plumber or a carpenter you don't buy them tools every time.


## Answer 34526

- posted by: [Ray](https://stackexchange.com/users/-1/15462-ray) on 2012-01-07
- score: 2

I'd say it depends. While I agree with @dnbrv to a certain extent, it isn't always possible for a developer to replicate your environment. And if they had to, you can bet that it would easily drive up your operating costs. In your case, if it's feasible and cost effective, there is no need to outsource the development environment.


## Answer 34530

- posted by: [Vasiliy](https://stackexchange.com/users/-1/14038-vasiliy) on 2012-01-07
- score: 1

My initial thought when you mention development environment is that it should be similar to your production environment. I am not a programming expert, but it might be best to just allow the "outsourcee" (not a word) to use your environment. This will help eliminate some issues when development code is moved to production code because the developer will be using the same environment for both. Otherwise there is a possibility of developing an application in one environment (with a set of options turned on/off) and then having issues to resolve when the application is moved to another environment (with a different set of options turned on/off).


## Answer 34535

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2012-01-07
- score: 1

There are a number of aspects to this.

If the work is hourly and is not being delivered to you as a productized thing, then you should probably supply the environment for development. 

This is even in light of the "tools of the trade" argument. I view it more as staff augmentation, and you are essentially the employer of the moment. 

One big factor to consider is version control and control of the source code. If you don't own the environment that the developer works within, then versioning is anybody's guess. 

Another factor - slowly disappearing with open source stacks - is the cost of the tools. A few years ago, Delphi Enterprise Edition was priced at around $3000. No way I'd buy it out of my own pocket for an hourly assignment at commodity rates. So be realistic about what burden you expect the freelancer to take on. 


## Answer 34568

- posted by: [Joe Augenbraun](https://stackexchange.com/users/-1/15477-joe-augenbraun) on 2012-01-08
- score: 0

My preferred model is that the contract says that the developer develops on their own machines, and then when the work is complete they transfer to your hosted environment.  I think it saves everyone hassle.  

But I've seen contracts that do it other ways too.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
