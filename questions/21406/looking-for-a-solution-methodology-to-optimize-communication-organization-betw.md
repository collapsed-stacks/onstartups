## Looking for a solution/methodology to optimize communication & organization between sales and tech-support/development teams

- posted by: [Danny](https://stackexchange.com/users/-1/2578-danny) on 2011-03-11
- tagged: `customer-support`, `business-process`, `organization`, `communication`
- score: 0

Before I get into the question, I’d like to mention that this is my first venture where I am a decision maker, it's been great but as you will see below, due to some inexperience, I am stumped as to what I should do with the following challenges:

Currently we are 5 employees: 1 sales, 2 developers, 1 tech support and 1 accounting.

I am responsible for Sales/Marketing/Customer Service. 

We started the business about 4 years ago but about 10 months we started picking up the pace and since then began restructuring so that we can get better organized and become more efficient. 

One of the challenges we face has to do with internal communication between sales and our Tech support/Development people. 

Here is the breakdown:


• When errors within the system are reported by our customer, typically it is conveyed to us via e-mail or telephone, and then we share that information with our development people. We then get told by the development folks that they will get working on it, however without providing us with a deadline. In addition, often times several days (sometimes more than 1 week) pass and we don’t hear anything from them.( they are swamped with work) So we then typically have to follow up with them, (this also creates another problem, because we are also super busy and, at times, can forget about this specific error problem in the first place, allowing even more time to pass before a fix has been created.)

• When customers provide us with their feedback about how we can improve our software, we capture the details in an email/word doc, then share it with the development folks and from then on we pretty much hear nothing. We believe this information is very valuable however we still have not come up with an intelligent process to ensure that information is always on top of mind as we continue the evolution of our software.

• The main channels that our customers contact us for support/error related purposes are through email, phone and a live chat module that we integrated into our software app. Currently, I have 1 person that is responsible for handling all of these support inquiries. However, I have no clear way to measure and monitor if he is doing a great job. Up until now, given our size and relatively small client base, my main indicator was our renewal rate, which has been very high, as well as that every now and then I touch base with the customer to see how they are. However this is not an adequate process and rather than depend on that, I need to be certain that I can be aware of his performance without micromanaging.

In summary, what I am looking for, is a solution where not only can we capture, monitor and execute the development related tasks that need to be carried out, but also for myself as an owner of this business to have some sort of measuring capability so I can be assured that my people are carrying out the tasks. This way, I can focus 95% of my time on selling and marketing the product and 5% on making sure that the tech support and development folks are doing what they need to do, WITHOUT MICROMANAGING THEM AND SENDING EMAILS BACK AND FORTH EVERY OTHER DAY.

I also want to add that since we have been growing more and more rapidly we have now attracted the interest of some pretty big distributors in our area and before I sign contracts with them I want to have the confidence that whenever they will need support from us, that we have a solid process/system in place. 

If you need any more details please feel free to let me know and thank you in advance!!

-Danny



## Answer 31386

- posted by: [Lorenzo Solano](https://stackexchange.com/users/-1/13814-lorenzo-solano) on 2011-10-12
- score: 2

<h3><strong>In a few words: Product Development + Agile Mythologies (Scrum + XP) + Software tools</strong></h3>

<p>Your organization is a good candidate for Agile methodologies. You can use Scrum to management tasks. You'll, definitively, need some tools like bug tracking system (Bugzilla, Jira, or other), but they are not all the solution. The e-mail or direct conversation are not a good candidate to manage your bugs or new changes. You can check my blog - Bad Communication Habits, to better explain your current problem and how Scrum roles resolve it.</p>

<blockquote>
  <p>• When customers provide us with their feedback about how we can
  improve our software,  we capture ..., then share it with the
  development folks and from then on we pretty much hear nothing. We
  believe this information is very valuable.</p>
</blockquote>

<p>As you point out on this statement, this information is really very valuable, your problem is that you are missing the role of Product Management. You have a couple of developers resolving issues and implementing new tasks but they are not looking at the big picture. You can read about Product Management and Customers Development from the following sources:</p>

<ul>
<li><a href="http://steveblank.com/about/" rel="nofollow">Steve Blank</a> (Product Development): The Four Steps to the Epiphany</li>
<li>The Silicon Valley Product Group (SVPG): Inspired: How To Create Products Customers Love</li>
</ul>

<p><strong>Sorry about missing links:</strong></p>

<p>Since I don't have enough reputation points I can not include all links. But you can eassilly look for all references on Google:</p>

<ul>
<li>Search for <a href="http://www.bugzilla.org" rel="nofollow">Bugzilla</a> and <a href="http://atlassian.com" rel="nofollow">Jira</a> (from Atlassian)</li>
<li><a href="http://steveblank.com/about/" rel="nofollow">The Four Steps to the Epiphany</a> (Steve's book)</li>
<li>The Silicon Valley Product Group (SVPG) (their company site), and</li>
<li>Inspired: How To Create Products Customers Love (SVPG's book)</li>
</ul>



## Answer 31387

- posted by: [jrullmann](https://stackexchange.com/users/-1/13802-jrullmann) on 2011-10-12
- score: 2

<p>We use a free bug tracking tool called <a href="http://www.mantisbt.org/" rel="nofollow">Mantis</a> to solve a lot of those problems.  The development team uses the system to track the work that they need to do, and the sales, marketing, and support teams prioritize the issues.  The development team works on the highest priority items, and the system provides various ways to communicate progress to the whole company (including a web site and emails).</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
