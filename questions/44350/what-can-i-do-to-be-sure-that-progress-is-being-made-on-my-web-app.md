## What can I do to be sure that progress is being made on my web app?

- posted by: [yangt09](https://stackexchange.com/users/-1/21693-yangt09) on 2012-11-20
- tagged: `developers`
- score: 2

I hired a developer 1.5 months ago, and I'm having serious doubts due to the lack of progress. The project cost is $2k and I paid half so far. 

So far what has been completed is just the front-end design/theme. I have not yet been able to see any functionality. He keeps saying back-end takes time. I do understand it takes time, but should he at least be able to show me some basic functions besides just the page layout by now? I just want to know functions are being worked on.

My next payment is coming up in few weeks, and I'm not sure what to do.

Is this the normal process? What can I do to be sure that progress is being made on my project?




## Answer 44364

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-11-20
- score: 6

There is an easy way to check the progress.

Where is the source code? If he worked on the backend he can show some source code. In addition, **ask him to push the source code to a tool like bitbucket.org**. It is free for a small team (github requires to pay even for a single private repo). The benefit: you can see all the changes, step by step. And when they have been done.

If he is not serious, he will say he doesn't use source version control systems. Maybe he argues because of the low budget and the time. But actually there is NO reason NOT to use it. git/hg/svn is absolutely necessary for every developer and every project. No way round. 

That said, he might also argue he is using SVN and not git/hg as supported by Bitbucket. There are several SVN hoster out there to which he can move the repo. 

Don't be afraid: even when you cannot read source code, you can identify changes with these tools. They all provide web interfaces where you can login and see what happened. If you have a friend with basic programming skills, he can easily spot changes in an instant and tell you if these are fake changes or real implementation work.

If he doesn't share the source code with you, he most likely don't have one. Tell him that you'll only send out another payment until you can see some progress on the source code.

He is right at one thing: backend sometimes takes its time. But this does not reflect in the source code. It is probably the case there is nothing really useful you can show to a customer. But in source code there must be changes. 

Another point: even when there is nothing "useful" to show: you should be able to see *some* features at specific point. For example, you should be able to see a working login after f.e. 1 week. If he says he needs to ramp up the framework first you should see some features after 3 weeks. To see absolutely nothing is very unlikely.

Besides the source code control **you can use tools like trello.com or agilezen.com or kanbanery.com** etc. In that tools you can list all the task which need to be done. The developer should even put technical things there, like: "installing database", "installing framework", etc. When a task is done the task card needs to be moved to finished. If that happened, changes in the source code are visible.

My tip: immediately take back control of your project. If necessary, hire a second, independent developer for a few hours to look at what has happened so far.


## Answer 44352

- posted by: [Aseem Gautam](https://stackexchange.com/users/-1/17251-aseem-gautam) on 2012-11-20
- score: 2

I have seen some Indian software companies hiring UI devs and quickly showing a working prototype but then delaying the actual development. Problem is lack of skill/time/manpower. 

In this kind of a scenario the end product is often quite buggy with quite inefficient code. 

Is the developer skilled for both UI/Front end and Back end development? I think he might be a UI developer and further outsourced back-end work. Did you scanned his resume carefully or authenticated his skills? If not, its not too late to find it out now.

Only pay if you are confident about the progress. Plus I don't understand why you released the 50% payment already. Its always better to divide the project into 4-5 phases when dealing with unknown persons and no or minimum advance(bargain hard here)!!

Your the client, be tough. Think about the $$ that you have right now and not about what is gone. Make sure you have all the UI related source files, in case you need to find another developer to complete the project.


## Answer 44362

- posted by: [Montagist](https://stackexchange.com/users/-1/21698-montagist) on 2012-11-20
- score: 2

I don't know about the complexity of your project, but $2k is fairly low - especially spread over 1.5 to 3 months - so I would say this is probably a side project they're taking on. Your project may not be their focus and you may have a decent wait ahead because of this.

If your project is a rather complicated one then the aforementioned goes even more so, with the addition that this developer may never finish.

Depending on what it is you've asked them to develop, there could indeed be ways to see the backend progress being made even if it's not yet connected to the site. For example, if they're building a "shopping cart" of some kind, it may be possible to just see a list printed in plain text that adds the totals or something like this. This all depends, however, on whether they're using some pre-made piece of software or platform (then it may be harder if they aren't digging that deeply into the backend as opposed to just configuring it, etc), as well as a number of others factors that might make seeing progress difficult.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
