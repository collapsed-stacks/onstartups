## Current web technologies in business point of view

- posted by: [Roberto](https://stackexchange.com/users/-1/18338-roberto) on 2012-06-15
- tagged: `website`, `webdev`, `tools`
- score: 2

I am a software engineer with no experience on web development and I will work on a startup which main product is a website.

We are in the very beggining of things, we are not commited to any technology or tool and have the freedom to pick anything. My task now is to decide which language we will use and then go for the IDE and tools for issue tracking, project management, version control and code review.

**I would like to know what should be considered for choosing the language to build this website, having in mind that the language will drive the choice of IDE and tools.**

I have thought of two points and appreciate comments on them. One is the cost that this "suite" will have now and on the long term.

The other is the option of choosing the best technologies and tools versus choosing one good technology and go all the way with it and things that integrate well to it. Choose the best stuff there is or pursue technology integration for developer performance combo? :)  For example: I could pick .NET and JIRA because we love it or I could go Microsoft all the way and pick .NET with Team Foundation Server and all Microsoft stuff because they are so integrated. What should I consider to answer this? Please note that this is only an example, I'm not saying it is better or JIRA is better.

I also don't know about the languages and frameworks, whether the type or complexity of our project should impact of the decision of language and frameworks. 


## Answer 39933

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-06-15
- score: 8

<p>In my opinion, a startup might consider these points:</p>

<ul>
<li><p><strong>Ease of workflow</strong>: How quickly can a dev build things with the tools. If using MS Foundation then you have chosen a complete workflow. Why should you break that? Jira will not integrate so well as TF, even when it is nice. If using something else like Java, there is no such workflow and you can chose between your components freely (and of course have an effort to do so). Look at: how much stuff is already done when choosing a technology?</p></li>
<li><p><strong>Setup of workflow</strong>: How much does it cost to maintain and setup a workflow? Probably (not a .NET dev here) MS does offer everything out of the box - no maintenance needed. In other worlds you need to take care yourself. Can you afford having around 2 PT just for the whole lifecyce + several hours per month for maintenance (there is always something broken or to be improved).</p></li>
<li><p><strong>Speed of development</strong>: How quickly can developers develop with the tools? .NET has a good workflow, but the Ruby on Rails developers seem to be the quickest devs on earth. They have a different view on workflow because workflow mostly means "development workflow". RoR is quick to develop, Java not so.</p></li>
<li><p><strong>Available programmers</strong>: How many people are around you mastering these technologies? If you need to hire, you'll mostly get Java developers. There are only a few .NET, Ruby on Rails, etc people. Some do PHP. How does it look like in your area?</p></li>
<li><p><strong>State of the art</strong>: Developers (which you want to hire) want exciting stuff. The tools itself get developed when they are exciting. These days it seems Adope (now Apache) Flex is pretty dead. Can you attract people with that? Probably no: Flex does not look good anymore on the CV. These days you need to impress people with JavaScript, HTML5 or probably even Java FX. Check out on the web what's in and hip and has a good quality to attract people. Just don't get too exotic. Only niche tools drive devs away, because nobody knows what they do, and they love to speak about their work.</p></li>
<li><p><strong>Vendor lock in</strong>: With MS you depend on MS. You most likely can't go away. There is Mono, but they depend on the niceness of MS too. With Java it is better. It is Open Source, but still Oracle has its thumbs on it. PHP is as free as you can imagine, but the development of PHP is chaotic. Ruby is very free too, and the language seems to be developed in a nice way.  What might be your option to have less dependencies to other people? Risks are changes of licensing fees or terms, shutdown of projects (like Flash/Flex of Adobe) and so on.</p></li>
<li><p><strong>Price per dev hour</strong>: How much do dev people charge per hour in your platform? SAP people are cracy with their hourly rates, Java people seem to follow. PHP are pretty "cheap" (rate wise).</p></li>
<li><p><strong>Outsource options</strong>: Do you plan to outsource? Some languages like Java are well known in countries with India. Ruby on Rails is probably not. It seem RoR people are mostly from the US (guessing). Analyse the potential outsourcing country.</p></li>
<li><p><strong>Libraries</strong>: Devs don't write everything themselves. In fact most features are baked out of available libs. For example, you want to send an AJAX request? In JavaScript you would probably use jQuery, in Java Commons Net and so on. Are there a wide varieté of libs available? This is one of the biggest advantages of Java: you get everything in multiple flavors. Ruby does have Gems, but it seem those are not so actively maintained like in Java world. In PHP world there is some stuff you need to write yourself. For example, there is only one serios CalDav lib, and even that needs to be hacked when doing something special.</p></li>
<li><p><strong>Fun</strong>: What is just fun? Only when you have fun working, you get good results.</p></li>
<li><p><strong>Coding safety</strong>: Types or not? The one say types are good, others hate it. Huge projects might benefit of typing, sometimes it is annoying and cost time. Yours to choose. My personal opinion: use types when you expect your software to become > 15.000 lines.</p></li>
</ul>

<p>That all being said, you need to evaluate the tools / language etc all yourself. There are heated, emotional discussion on "what is the best language" out there. It does not make sense to repeat these discussion. Instead make up some points like I did and evaluate on them. Lastly <a href="http://www.grobmeier.de/how-i-select-open-source-projects-25012012.html" rel="nofollow">I want to give you a link from my blog on a similar topic</a>. Maybe it is inspiring you too.</p>



## Answer 39956

- posted by: [Chris K](https://stackexchange.com/users/-1/18406-chris-k) on 2012-06-15
- score: 1

@Christian's answer is great and is full of +1 from me. My experience and my take is a bit different. I was briefly a Software Engineer and am now the guy running a somewhat successful e-commerce site. 

My brief answers are in order of narrowing scope: 

 - Embrace someone else's huge project and let them do the hard stuff (ecommerce means running Magento) You aren't inventing Facebook; take a solution and choose what requires the least work to adapt to your needs.
 - Stay FOSS whenever practical, it's saved me at least $100k in software. And I do have Windows machines dedicated to things like Adobe CS6 or Quickbooks.
 - See what the competition (&/or new kids) are doing and understand when it's time to grow.
 - Forget apache, look at new lightweight speedy stuff like nginx / php-fpm.
 - PHP all the way, for classical C guys, it's the easiest to learn + I find it exciting to work in.
 - Use and learn Ubuntu everywhere. It never breaks just because.
 - Ubuntu lets you connect to your site very easily.
 - Amazon EC2 lets you click a button and you have a running new server in about 3 minutes.
 - I use and love Geany editor. A lot like CodeWright from back in the day.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
