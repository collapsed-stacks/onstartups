## SaaS Startups: When Should You Separate User Controls To Web?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2010-10-06
- tagged: `business-process`
- score: 1

I am currently doing a SaaS startup.

Basically, I have a Java application in which the user does the work.

The work is saved on server, and jobs are run on the server.

I was originally thinking of making the job management, user management interfaces on a web UI. So the user would simply login to the web interface, view which jobs are running, and have the ability to cancel, stop, delete jobs, and other features.

However, I am thinking wether this is necessary or not, since previously mentinoed features like accessing user's current running tasks, ability to pause, stop, delete tasks can be written directly into the Java application.

I am envisioning a process in which the user can directly login through the Java application, and manage all of their jobs instead of having to access the main site.

For now, I don't see any real advantage or value created by separating the job management on the web. That means once the user creates a job, user needs to login on to the members area on the website. If new job needs to be created, then the user needs to start the Java application again. This seems very inefficient.

Why not include the entire server job management and monitoring all inside the same Java application ?

However, the trend seems to be, SaaS startups are separating the two tiers. 


## Answer 14796

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-10-06
- score: 1

Will it make your application easier to download and install without the job and user management parts? Do you see having to update this interface frequently? Then a web app may be more appropriate. 

Sometimes users like the convenience of a web app since they don't have to install. If a user is away from their PC, they may want to use a mobile device to check on things.

If you are considering moving the entire user interface to the web, the admin parts may be a good start. I wouldn't separate them just to be like other SaaS startups. You're already having to distribute and install your app, what's to be gained?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
