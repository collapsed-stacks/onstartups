## Implementation partners-protecting source code

- posted by: [user8226](https://stackexchange.com/users/-1/8226-user8226) on 2013-03-06
- tagged: `legal`, `intellectual-property`, `outsourcing`, `technology`, `legal-documents`
- score: 1

I have an existing SAAS platform and I am in the process of working with multiple implementation partners or vendors for some enhancements. How do I make sure my source code is protected? Some of these vendors are in south Asia as well and I am NOT sure how NDA will be helpful.

Other option is to break the source code into different components and provide access to only one component to each vendor. Is this makes sense or this is something I don't need to worry about.

Thank you


## Answer 47870

- posted by: [Elenesski](https://stackexchange.com/users/-1/23572-elenesski) on 2013-03-06
- score: 2

This is more of a technical question, and the answer is more about software architecture, but what you need to do is create a decoupled environment that uses a facade.

Decoupled software is all about software that isn't coupled.  Coupling is explained here: http://en.wikipedia.org/wiki/Coupling_%28computer_programming%29

And facades are a design pattern that allows you to create a interface that hides the details of the code below, like an API, described here: http://en.wikipedia.org/wiki/Facade_pattern

So what you do is never give your source code to the people you don't trust.  Instead, you give them a compiled library with an API (the Facade).  Their code and yours too, needs to be architected in a way that neither is not dependent on the other in order to operate; as soon as their is a dependency, the code is coupled.  It's a good practice to do this anyway, because if you discover their code is sub-standard, you can replace what they wrote with another library as long as the other library writes to the same facade/api.

A facade will go a long way to decoupling the code.

Hope that helps.


## Answer 47874

- posted by: [Shadi Moadad](https://stackexchange.com/users/-1/25352-shadi-moadad) on 2013-03-06
- score: 1

Here are few ideas on how this can be solved:

 - For software that doesn't require a build (e.g. scripts like php, python, shell...). Give them access to a small part of the service where they can upload their changes without having access to the full system.
 - For software that require a build before they can deployed: provide them with access to VCS with permissions on the sections they are allowed to work on and once they commit to the VCS they can build and deploy on your test server via some kind of continuous build system like "Hudson". This remote build/deploy could be a bit counter productive thus if possible, give them compiled & obfuscated libraries that they can link to in order to test their work



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
