## GAE for starting a business?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-10
- tagged: `technology`
- score: 0

What are your thoughts on GAE and GWT for starting a startup?


## Answer 384

- posted by: [James Avery](https://stackexchange.com/users/-1/288-james-avery) on 2009-10-10
- score: 2

My main concern with either GAE or Windows Azure is that if you program to their platform you are in essence locked in (unless I am missing something). If you decide you want to move to dedicated servers or another provider you would probably have a significant amount of work in front of you.

That being said if you can accomplish your goals way faster using GAE and get your product out earlier then it could be worth it.


## Answer 517

- posted by: [Vineet](https://stackexchange.com/users/-1/24-vineet) on 2009-10-10
- score: 2

We are doing exactly that: GAE + GWT.

Given that we do alot of Java, the nice thing about using GAE has been that we don't need to worry much about the infrastructure and we know that if we need to our application will scale.

There is the part that you need to be a little careful about - getting locked in to Google's API's. We want to support on-premise deployment so have been a little careful about not using anything specific to Google API's. This part is a little bit of a challenge when doing persistence, but so far we have been able to overcome challenges.

As for getting your data out. I figure this part should not be too hard to implement. Yes, it might take a week to implement and move the data out, but that part is likely something that you want to worry about when you have already shown the product (and business model) to be successful and are trying to optimize costs. At the current stage of evaluating an idea having enough traction and rapidly iterating on the idea (as opposed to the infrastructure, etc) it makes alot of sense.


## Answer 370

- posted by: [Jay](https://stackexchange.com/users/-1/272-jay) on 2009-10-10
- score: 1

I personally wouldn't use it as the core platform for a revenue-generating product.

It would be great for MVP/viability/prototyping though.

The main reasons I have against it are: ease of getting data out, complications over who owns the data and code (you do but you can't access it!), some restrictions on what you can and can't do, and difficulty of porting to a new system if you decide to do so (using Django helps with this). It's easy enough to set up in the cloud for minimal expenditure where you have full control.


## Answer 7244

- posted by: [Abhay Vardhan](https://stackexchange.com/users/-1/2368-abhay-vardhan) on 2010-01-28
- score: 1

I have played around with GAE a bit and on whole have been extremely happy with it. It is very cheap, provides scalability, keeps previous versions of my deployment, has a nice API for all the common tasks. I do not have to worry about keeping the server up 24/7. There is a handy dashboard which lets me look at how the app is doing.

The data lockin is not a big issue. There is an API now to upload or download data (see http://code.google.com/appengine/docs/python/tools/uploadingdata.html)

That said, if there is something that you need (eg library) which is not supported, you are out of luck. Some people also worry about the level of support but that has not been a big problem for me.




## Answer 367

- posted by: [Alexandre Gomes](https://stackexchange.com/users/-1/223-alexandre-gomes) on 2009-10-10
- score: 0

I'm developing a RESTful architecture with GAE and Django (http://code.google.com/p/app-engine-patch/) and javascriptMVC (javascriptmvc.com) for the frontend.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
