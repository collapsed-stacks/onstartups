## What are some best practices for managing user feedback?

- posted by: [Travis Truett](https://stackexchange.com/users/-1/8591-travis-truett) on 2011-08-11
- tagged: `management`, `customer-feedback`
- score: 1

After months and months and months of work, our team finally launched our first application. 

We have been very fortunate to receive a lot of feedback and one of my first "goals" post-launch is to create an effective feedback system so that I can efficiently get meaningful feedback to the development team.  

**Brief background:**

Launched with Mac OS X client.  Team consists of three developers and three non-developers.  Non-developers will be spending a lot of time on the road marketing and receiving word-of-mouth feedback.  Our desired goal is to create workflow so that the non-developers receive all of the raw bug reports and feedback, organize it, sort it, and present it to the development team in a prioritized list.  

While this _seems_ easy and straight forward enough, I would appreciate any help from the community regarding best practices.



## Answer 28641

- posted by: [Lloyd S](https://stackexchange.com/users/-1/12549-lloyd-s) on 2011-08-11
- score: 1

This is based on how we managed our desktop Windows app.

- Have dedicated bug/feature management software that enables prioritisation (we used FogBugz)
- Have your application auto submit any issues caught by your error handling (submitted through FogBugz XML Api)
- Provide email address for support that customers send email to (Fogbugz stores these for you) and we can respond to. Sales guys can also submit bugs through here and be responsible for prioritisation but usually needs a technical view
- Sales guys collate feature requests, once a week or every other week they get discussed and grouped where possible. Each gets a complexity and business benefit score. So easy ones that offer the biggest benefit get delivered first etc

There are alternatives to FogBugz (as you probably know) that is just what we used.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
