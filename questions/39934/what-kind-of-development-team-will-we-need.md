## What kind of development team will we need?

- posted by: [Derek](https://stackexchange.com/users/-1/18409-derek) on 2012-06-15
- tagged: `website`, `development`, `code`
- score: 1

How many developers would it take to build another Facebook?  Or at least a trimmed down version.  Can one good developer do it, or would we need a large team?  I have three partners, none of us has much tech experience aside from building the occasional Joomla or WordPress site.  Our inexperience is painfully clear.  Our idea is a social network with many of the same features as a Facebook, however very different as well. We are finally at the point where we are ready to start looking for a developer/s and we are trying to figure out what kind of team we need.  Any help and/or input would be greatly appreciated!



## Answer 39937

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-06-15
- score: 4

It all depends on how many users you expect and how quick you grow. Facebook has millions of users and this reflect on the data storage (among others). While you can use a simple MySQL database for a Drupal driven site, you need to think different when developing a Facebook clone. You probably need to look into software like Hadoop which is highly complex and requires devs with good skills in math. Scaling software in that dimensions is not easy.

I do not know what features you want to see, but I would say three devs is a minimumwhen starting with such a software: 

- one operating systems, deployment, build, clustering etc
- one building backend including hadoop
- one building the frontend

All the devs must know how to work in such an environment. They should be able to discuss problems in each others fields, even when they are not working in it. You'll soon realize that once the bootstrap system runs you might need more people to operate. 

Facebook btw does currently employ 3000 people. Please do consider that and the fact that Facebook is one of the biggest software clusters out there.

On a side comment, I really hope you have evaluated your market well. It will not be cheap to develop this and others - like Google with G+ - wrote "something like facebook with similar features but better" too. I can imagine a more niche related social platform is a bit easier to develop, because you don't need to think in clustering, Hadoop and other complex terms.


## Answer 39940

- posted by: [frenchie](https://stackexchange.com/users/-1/15155-frenchie) on 2012-06-15
- score: 4

**Building ANOTHER Facebook?** How many developers would you need to build something that can be launch-ready? With today's tools, most likely less than 5 initially but that's not the main reason I decided to answer.

**Some people successfully achieve failure.** Suppose you do manage to build a site, and that technically speaking, it works. Now what? Fast forward to the point of launch and think that building ANOTHER Facebook, or even something of a much much smaller scale, **is not a technical problem but a marketing problem.**


## Answer 39975

- posted by: [Wolf5370](https://stackexchange.com/users/-1/18438-wolf5370) on 2012-06-17
- score: 1

OK, so the question isn't about building another FB clone (MySpace ? - of course that came first though, maybe Google+). but about resources to build something that scales to FB size. Assuming you can cover the hardware/hosting costs (which could be enormous for such a user base), then really it depends on how quickly you want it.

FB is not technically very difficulty - if you remove the apps etc, then its not difficult at all. The real prize is the scalability - this means good database design (again ignoring the hardware/load balancing etc). I would suggest a minimum (i.e. without time constraints - say over 6 months to a year) - Project manager, systems analyst/dev lead/designer, good DBA, backend DB coder, backend service designer/coder, web coders (a least 3 of), graphic artist/designer and testers (can reuse, but better to not test what you code). That is just technical staff, on top of that, good (legit) SEO company, publicist/pr/advertising company, lawyers (can be temporary), accountant, business analyst/manager/you. 

The real hurdles is not recoding it - you could outsource that for a few thousand dollars probably, but building a paying user base (or non paying user base and paying advertising user base) and scaling it to accommodate a large user base.


## Answer 39977

- posted by: [JohnZ](https://stackexchange.com/users/-1/18439-johnz) on 2012-06-17
- score: 1

Facebook is a complex product, and one of the major challenges is handling the scalability of millions and near billions of users.  That's a very significant challenge.  You won't have that problem for several years, I'm guessing, especially if it's a niche product. 

What I'd advise, is build the simplest possible thing you can, and figure out other ways to get the idea out to real users before spending tons of money building it just to find out that people aren't interested in exactly what you built, but rather something *like* it.

That being said, for any decent web app, I'd recommend at least the following:

    1 Illustrator/Graphic Designer for making stuff pretty
    1 Web Designer for making the layout of your pages beautiful and flow from page to page
    2 Backend Developers for actually building the logic
    1 SysOps Guy to handle setting up all your servers and installing software etc. to save your devs time

With this team working full-time, I'd expect you could have something for beta within 3 months, and a product ready to test on the market by 6 months.  It won't be the best thing ever, but it will have decent functionality, and your illustrator/designer will make it look really shiny so you can grab those customers, and get them to give you a chance.

By the end of your first year, your 2 backend developers will be starting to be overworked, so you'll probably need to hire a few more, based on your customer base.  

Get traction first and foremost, and good luck!


## Answer 39954

- posted by: [OrionDarkwood](https://stackexchange.com/users/-1/18174-oriondarkwood) on 2012-06-15
- score: 0

I won't answer you question but I would ask myself What does this Facebook clone do that isn't already there? A major trick in startups is rather than fight in existing markets, define new markets. However sometimes you have to fight in a existing market and if you do you have to have something that no one can offer or no one else can do as cheaply.

I would sit down and define exactly what you want this Facebook clone (let's call your app - MyApp) to do. Then I would research what is out there that can partially or wholly do what MyApp is theoretically going to do. If you find that there are things then tweak MyApp specifications.

Once you have that done, then research what is the most effective way to craft MyApp (I am oddball in that I view application development as a work of art, not building a bridge).

After that then decide how fast you need it done, and how skilled of employees are you going to need.

Then you will have the answer to your question.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
