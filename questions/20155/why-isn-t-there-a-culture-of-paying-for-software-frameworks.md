## Why isn't there a culture of paying for software frameworks?

- posted by: [Marty Pitt](https://stackexchange.com/users/-1/7475-marty-pitt) on 2011-02-12
- tagged: `business`, `pricing`, `business-model`
- score: 1

Note:  Cross-posted at [programmers.stackexchange.com][1]


One of the side effects of the recent trend of "Lean" startups, and the app store era, is that consumers are more acclimatised to paying small prices for small games / products.

Eg.:
 
  -  Online SAAS that charges ~$5 / month (the basecamp style of product)
  -  Games which are short, fun, and cheap ($0.99 from the app store)

This market has been defined by "doing one thing well, and charging people for it."  DHH of Rails / 37 Signals fame argues that if your website isn't going to make money, don't bother making it.

Why doesn't the same rule apply to frameworks?

There are lots of software framework projects out there - many which are mature and feature-rich, which offer developers significant value, yet there doesn't seem to be a market or culture of paying for these.

It seems that the projects which do charge money are often things like UI component toolsets, and are often marginalized in favour of free alternatives.  

Why is this?

Surely programmers / businesses see the value in contributing back to projects such as Ruby, Rails, Hibernate, Spring, Ant, Groovy, Gradle, (the list goes on).  I'm not suggesting that these frameworks should start charging immediately, but that there must be a meaningful business model that would allow the developers to earn money from the time they invest developing the framework.

Any thoughts as to why this model hasn't emerged / succeeded?


  [1]: http://programmers.stackexchange.com/questions/47059/why-isnt-there-a-culture-of-paying-for-frameworks


## Answer 20156

- posted by: [bhanu prasad](https://stackexchange.com/users/-1/7050-bhanu-prasad) on 2011-02-12
- score: 2

Actually i don feel that they should charge for the development work which programmers are investing.  I feel that they are earning money for the time which  they are investing on opensource through clients.They are getting paid by the clients for the consulting work and it is indirectly a revenue generator for the developers. In addition to that they are getting lots and lots of contacts and recommendations for their open source contributions if their work is very good. It is a type of marketing strategy where people are investing time but not money. 


## Answer 20195

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2011-02-13
- score: 1

The primary reason for this is **People by solutions, not frameworks**.

As a general rule of thumb, the closer your software product is to an activity that actively generates revenue (or protects it) the easier it is to monetize.  Base level frameworks, like ASP.NET or Rails are so far from the money that they are extraordinarily hard to monetize.  Even higher level business frameworks that are several steps closer to revenue (think CRM frameworks, accounting libraries, etc.) are hard and have really long sales cycles.

Conversely, people will pay to not have to read documentation or understand the details behind a problem even when it's already solved.  We have a healthy set of customers for our flagship product that primarily purchased because we have a wizard that wires everything up and they just don't have to think about how any of it goes.  They could get the same information from MSDN and manually eidting XML, but they prefer a GUI wizard so it's one less thing to think about.

Secondarily, **people are generally terrible at extrapolating benefits from features**. The more directly you can speak to their exact benefit the more likely they'll happily pay for something. The more focused your product is the easier it is for people to see how it solves something exactly and fits into this model.  The less focused, the more you're asking them to come up with how it provides value for them.  


## Answer 20157

- posted by: [ShaneG](https://stackexchange.com/users/-1/3074-shaneg) on 2011-02-12
- score: 0

For open source projects code changes are often referred back (mainly for bug fixes and less commonly for feature improvements). Quite often though specific extensions are not suitable for general use and not included in any new releases. Larger organisations also tend to donate toward a clearly defined development team (if one exists) - check the logos displayed on the home page of any particular open source project.

For closed source projects the problem seems to be that you are asked to hand over money without getting any opportunity to test the framework prior to committing to the financial responsibility (or the test version is so limited you can't really test it at all). Many new mobile game frameworks seem to follow this model - great demos on the website with no opportunity to download a test version of the framework to implement your own idea. Given that a lot of mobile applications are created by individual developers who can't really shell out a few grand for a framework hoping it will work, they are more likely to develop the functionality for themselves (even if it is less efficient).

If you are concerned about this (funding for open source projects) you can always donate a percentage of your revenue back to the products you are based on.

Regards,
ShaneG


## Answer 20160

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2011-02-12
- score: 0

There are couple of reasons. First commercial projects tends to die and leave you vulnerable but even if used open source framework die you can keep fixing / improving.

Closed source frameworks can be tricky, I used some, when you stuck, you stuck. You need to get support from commercial people.

There are some things that you really want to follow the crowd, IMHO frameworks are like this. You don't want to use a framework unless it's got good user base, because you need help, sample code etc.

For all these reasons launching a product on top of a commercial framework is risky unless that framework officially supported by a big guy like MS, Sun etc.

*P.S. Paying the open source frameworks is something else and AFAIK there are many companies with donations. Also not a framework but I know that Yahoo! donated a good share to Perl's inventor just because they were using it.*


## Answer 20161

- posted by: [Gennady Vanin Novosibirsk](https://stackexchange.com/users/-1/7476-gennady-vanin-novosibirsk) on 2011-02-12
- score: 0

Except very big monsters like Microsoft, Oracle, Goofle, etc. the majority of IT company models is not sustaibnable on development and selling it sown software products. And this is not what most consumers need. Not just bare product but some guarantees, support services and certain work done.    

There are different business models but the main trend that companies, even big ones, earn money on support, services, consultancy, re-selling the products of others and providing the services, expertise of support to them.  

So, it is not products that earn money, and which are frequently given away for free, but services to them.  
   


## Answer 20207

- posted by: [Samat Jain](https://stackexchange.com/users/-1/7194-samat-jain) on 2011-02-14
- score: 0

Frameworks are like standards. That is, if you have to pay for them, no one will adopt or use them.

This is true of all industries, but doubly so the technology/software/IT industries—where NIH (Not Invented Here) syndrome is rampant.

There are exceptions of course, particularly when there are "monopolies" involved (I use the term *very* loosely here), like Adobe Flash. It became popular because, besides some well-done business deals to get it included with operating systems, it was really the "only" way to get fancy video and animation on the web (there are a lot of parallels to the H.264 debate, but I disgress). However, witness the open web movement and HTML5: people want to move away from Flash like the plague. 

Commercial frameworks have business models difficult to sustain or make work.


## Answer 20227

- posted by: [Qyuubi](https://stackexchange.com/users/-1/7233-qyuubi) on 2011-02-14
- score: 0

Simply because it's better business model to make sure of large user base and charge for services, support and IDEs (like the VS). 
 
Ensuring a large user base and hence increasing the value of the code dependent on the framework is the goal.  

This doesn't quite apply to open source projects but then those projects are not about making money directly anyways.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
