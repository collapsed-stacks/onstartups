## How should I structure my development environment from a high-level?

- posted by: [marcamillion](https://stackexchange.com/users/-1/160-marcamillion) on 2009-10-10
- tagged: `development`
- score: 3

So I guess the follow-on question for this will be to jump into some of the specifics, but I have never worked on a software development team in a professional capacity and am building a web startup.

How do I structure my entire development environment on a bootstrapped/startup budget? What are the things I will need? There will be two coders and 1 designer (all cofounders including myself). 

I know I will need a Version Control System, for us to manage the development, but from there what next? 

Do I need a development, staging & production server. If so, how do I setup all of those on one server without having to rent/buy 3 different servers? Even better yet, how do I setup that sort of environment on a cheaper cloud offering like the grid hosting solution from www.mediatemple.net . Is that possible/desirable?

Do I have to worry about server monitoring with tools like Nagios from now, and where can I learn about architectures that will scale - because I keep reading about people making the wrong choices early and it being a huge headache when they need to scale. How do I avoid those types of mistakes?

Ideally, I would like to release early & release often - like the guys at www.getdropbox.com do so wonderfully.

Thanks.

[Edit]

Thanks guys for all the great feedback. 


## Answer 257

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-10
- score: 3

The setup you *need* is entirely dependent on the development model you intend to start with, and how you plan to manage scaling.  From a high level, the specific technology needed is  irrelevant until you're nearing a production release.  The absolute important components are:

 - Communication/tracking: How likes/dislikes/improvements/features/bugs/goals for the product are made available and tracked.  Bug/Ticketing systems (Jira, Trac, etc.) are the typical method.  Early integration with using an actual system will make everyone's life easier, rather than relying on individual to-do lists, notes from meetings and emails.

 - Collaboration: How do the developers and designer work on all aspects of the system simultaneously.  This is the revision control system.  Let the developers decide, just start with one early on and you'll save a ton of heartache later on (the only time I've had hard drives crash completely is when there is data on them that is not available anywhere else).

 - Progress: A method for each member of the team to be able to quantify what is done versus what still needs to be done.  There are many approaches, from milestones with tickets assigned to it, to a checklist of features to ad-hoc reporting based on functionality levels (I know those all sound similar, but it's the approaches from completely detailed to general overview).

A staged buildup of equipment is what I would go with.  Start with someone's spare/old computer (laptop or desktop, anything that can get a server load on it) and let the developers set up your initial tracking platform.  Once you have something real to show (ie, the machine is definitely not the right resource or you need a good, everyone can see it setup), compare costs of hosted vs. purchased.  There are several companies that provide VPS setups for very good prices (my personal favorite the base package is $10 a month and every facet is upgradable and doubles each increment at $5 increments, look for flexible providers that let you up the parts you need (memory independent of CPU time independent of bandwidth).

Once you're ready for the first showing, the developers can provide the best feedback for the setup you really need.  After the initial rush, I would strongly suggest finding a reasonably priced consultant or an associate with an extensive systems administration background.  Have them look at your architecture and go through with the developers where the most painful scalability and management issues will be at.  Don't have them do any of the work, this is to get an understanding of what your problem areas will be before you get there.  You can then plan for when, where, how and why you'll change the underlying system.


## Answer 311

- posted by: [Elad Kehat](https://stackexchange.com/users/-1/189-elad-kehat) on 2009-10-10
- score: 2

Try to host everything on the cloud. Avoid the hassle of doing admin.<br>
You can find some great solutions that are free to start with, and will only cost you (a little) once your project grows.<br>

Some tools:<br>
Google apps for collaboration - email, calendar, docs etc. all for free (and everybody on your team probably uses gmail already anyway). Can't wait to put my hands on wave...<br>
Skype is a great for free voice if you don't all work in the same space.<br>
I highly recommend Pivotal Tracker (pivotaltracker.com) for agile project management, ticketing etc.<br>
We use beanstalk (beanstalkapp.com) for version control (svn) and they're OK.<br>

Hosting:<br>
I'd like to join the other answers here - absolutely use Amazon (EC2, S3 etc.). Don't even think of spending money on buying or even leasing dedicated servers elsewhere.<br>
AppEngine is also an option, but then you're pretty much stuck on their platform.

Regarding staging production etc., you don't need that if you use EC2 (or some other cloud provider). Check this out: http://hivetech.wordpress.com/tag/staging/

Finally, do not spend any time on serious monitoring solutions etc. - until you actually have some traffic... Getting traffic (=customers) in the first place is much more difficult then making sure you can service them later. Take Twitter as an example - if the product is compelling enough, you'd be able to fix your performance failures later.




## Answer 238

- posted by: [Van Nguyen](https://stackexchange.com/users/-1/121-van-nguyen) on 2009-10-10
- score: 0

It is usually best to delay moving onto the cloud until you have your tech down.  Its not necessarily any less complicated.  Since you're asking this, you know enough to get by but you probably need a proper CTO who knows this stuff in and out.  

You can setup multiple servers on a single machine using virtual machines.  If you do end up going cloud, I recommend either Rackspace or if you go to EC2 (pay for the reserved instances as they are over 50% cheaper).  

For you, I suggest doing it in house at first, with a cheap <600$ linux box to test out your ideas.  That's if you're at least serious enough to buy one of those (you could use someone else's computer but unless they have multiple hard drives, disk contention will ruin their day).  If its not worth spending 600$, if you plan it, you could use say EC2 for a few hours and test without spending more than a few hundred.  

Google things like Continuous Integration, version control hooks, and TDD (slow but may be worth it for you, it depends).  


## Answer 245

- posted by: [Julie King](https://stackexchange.com/users/-1/11-julie-king) on 2009-10-10
- score: 0

Try hosting your development code in-house on a cheap server and set-up a low-cost account online. Also, look at frameworks like Zend to get development right from the outset.


## Answer 251

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-10
- score: 0

For a basic proper development platform, you will need the followings

1. a source code version control system
2. a platform for development
3. a platform for testing 
4. a platform for integration test (if system involved interfacing others system)
5. a team development platform (like Visual Studio 2008 with Team Foundation Server)

As a startup on a budget, you use Virtual environment like Virtual PC or VMware.
You only need one powerful server.



## Answer 282

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-10
- score: 0

You can try eApps hosting. They offer complete linux server (with root access) for under $20/mo. I've been using it for last 4 months without any issues.


## Answer 29321

- posted by: [Walter Heck](https://stackexchange.com/users/-1/12983-walter-heck) on 2011-08-27
- score: 0

Just to throw some real-world examples out there from a bootstrapped startup, here's what we use:

* redmine (http://redmine.org) for issue tracking and wiki, couldn't live without it!
* git through github (http://github.com/tribily for version control. No hassle having an in-house code repository and super easy management of users and teams. If you pay 20$ you also get private repo's, so worth it!
* puppet for structured system administration, makes every change transparent and accountable, as well as making scaling very easy.
* physical servers at www.hetzner.com. Our product stores a lot of historical data  in teh database that needs to be instantly accessible at any time, so we need large disks. We use Hetzner because they are cheap, environmentally friendly and they allow us to reserve rackspaces adjacent to the ones we use. You can reserve as many as you want for as long as you want for 10EU/1U/month, totally worth it. We have three physical servers there that just run the production environment, I don't want testing or development environments anywhere near our production environment :)

Hope this helps :)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
