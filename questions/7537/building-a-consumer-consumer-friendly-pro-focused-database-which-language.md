## Building a consumer consumer-friendly, pro-focused database: Which language?

- posted by: [AAE](https://stackexchange.com/users/-1/2085-aae) on 2010-02-03
- tagged: `database`, `infrastructure`
- score: 0

I want to build a consumer-friendly, pro-focused database with a layered interface (free vs. subscription) not unlike IMDb/IMDbPro. However, I am not a developer and have no idea if it's better to work in Ruby or PHP or Python or.... I've worked with developers enough to know that things can go horribly wrong re: speed/flexibility/scalability/etc. if wise choices aren't made early on. (Case in point may even be IMDb, which began as a listserv. Not sure what they're built on now, but I know from former employees that it's less than ideal and way too big to retrofit.) I've put this question to a lot of people and get answers like, "It's really just a matter of personal preference," but I don't entirely believe that. Can anyone point me toward some guidelines re: identifying some structural models for this database?


## Answer 7538

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2010-02-03
- score: 2

The wisest choice you can make early on is to get a good developer involved.  Given good design, the actual platform is rather inconsequential (ie, people like to say "PHP doesn't scale", but no one told that to the Facebook people, Facebook currently runs on PHP).  It hink every programming language/database has at least one major implementation out there that "proves" that the platform can handle the load (ie, This forums software, also used in StackOverflow.com uses .NET, Twitter uses RoR, etc...).  The key is good design, and good design comes from good designers.

See this for a better discussion: <http://answers.onstartups.com/questions/831/how-to-pick-a-platform-for-a-startup-web-2-0-app>

If you do a search in this site for "best platform" you will see other answers to the same question you pose.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
