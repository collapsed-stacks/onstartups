## Private beta real world examples

- posted by: [Thomaschaaf](https://stackexchange.com/users/-1/205-thomaschaaf) on 2009-11-21
- tagged: `beta`, `web`
- score: 0

Our company is currently in development of software, which should help software developers better support their products. Currently we are still in development but are planing to get into private beta in spring of 2010. I have looked at a couple private betas and am trying to find more which are more like my kind of service. When signing up every company gets their own subdomain a lot like fogbugz. 

Which sites have you found to have a cool private beta signup method? Or looked cool?

Some examples I have looked at:

 - http://www.unisonisyou.com/
 - http://web.archive.org/web/20070628204041/http://pownce.com/
 - http://tweetpotato.com/
 - http://wave.google.com
  - http://wave.google.com/help/wave/about.html


## Answer 3954

- posted by: [Brian Deterling](https://stackexchange.com/users/-1/496-brian-deterling) on 2009-11-21
- score: 4

<p>Prefinery is an app specifically for managing your beta process. I believe it provides you with an invitation form.  <a href="http://www.prefinery.com/" rel="nofollow">http://www.prefinery.com/</a></p>



## Answer 3955

- posted by: [Dane](https://stackexchange.com/users/-1/1441-dane) on 2009-11-21
- score: 0

You can look at: https://www.atlassian.com/hosted/HostedEvaluation.jspa?showOptions=false&productId=1

There are several things I really liked about this trial (I'm evaluating Confluence now so I'm actively going through this process).  While it's not a "beta" it has many of the same characteristics

 - The email that you get after creating your evaluation account is very clear and points you to several getting started resources as well as the full documentation.  The info is good enough that I've kept the email as a resource guide.
 - As important as the ease in creating the account the followup has been great.  The followup email does not just contain a contact info for help but also points you to videos and further info.
 - A week or so in I got another follow up email with info on more advanced features.  Rather than bombarding me with all the features right at the start they staggered the info so I had a chance to learn the basics before being confronted with the advanced features.

This evaluation made me realize that the followup process is actually more important than the sign up process.  I would expect this is true for getting feedback from beta customers also.



## Answer 3958

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-11-21
- score: 0

Since you write software, why not just write your own software for managing the beta test?  That way, if you change your requirements then you can just make the change.

For example, you start with assuming everyone (all 10 original beta testers) will use the same version.

Then, you add a new feature, fix some bugs, get more testers, and you decide to try a focus group approach, so you will have three versions that differ slightly, to see which features get the best feedback.

So, when a user logs in they are directed to the correct version of the application

All of this is easy to use in Tomcat, using a filter, and in IIS using the ISAPI filter.

I tend to find that if I have to work around a framework then I would prefer just to write my own. :)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
