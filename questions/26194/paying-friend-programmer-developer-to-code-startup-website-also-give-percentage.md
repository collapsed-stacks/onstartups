## Paying Friend/Programmer/Developer to code Startup Website. Also give Percentage? How to keep Accountable?

- posted by: [Zach](https://stackexchange.com/users/-1/11163-zach) on 2011-06-11
- tagged: `partner`, `employees`, `salary`, `shares`
- score: 2

I have an income and a website idea. I know nothing about programming. I have a friend who is a programmer, comp-sci major, and so to get my idea created into a website I am paying them an hourly wage for coding work. They want an income over the summer and I would prefer to keep as large a part of the website/company as I can. 

1st issue: I agreed to pay my friend a certain wage for work. My friend has been working a couple weeks and has over 100 hours of work in. There is no prototype yet, and I am not sure how to analyze the code or tell whether I am getting a good output for my money. How should I keep them accountable for their work? For part of this time we have not been in the same physical location and so I want to be sure that the hours they've given himself for the amount of work done makes sense. 

Sidequestion 1 - Any comments as to the best way to keep track of employees hours, something better than having them write down hours worked each day. 

Sidequestion 2 - My friend thinks he can do all the necessary coding, but should I hire a second programmer or outsource some coding to make things more cost-efficient. He could outsource tasks anyone could do and save the big problems for himself... or have two programmers compete with each other for tasks somehow

2nd issue: To improve motivation, I was thinking about lowering the hourly wage and giving some percentage (vesting) of the company to my friend. The company is in its initial stage and I have not figured out any profit projections or anything like that, so I was wondering how to figure out how much percentage to give for the amount I would lower the wage. 


## Answer 26196

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-06-11
- score: 4

1st Issue: you need to break down things to small action items on a functional level. Lets say  you want to build a twitter client. You could break down things into:

 - Login/Logout
 - Send Twitter message
 - Show all Twitter message
 - Search for a Twitter message

Paint a wireframe for this (on paper, or there are tools out there).
You friend will add some technical task items to you list, like:

 - Logging
 - Create base framework
 - Create layout
 - make executable for macs
etc.

Now you can compile "stories" of these items. You first story probably will be a very technical one, like: "create framework" and "logging".

Once you have all the stories, your friend should give you an estimation for each task. I can imagine the first story might take a good while, like 2 weeks or so. The "Usability story" with several tasks on usability might take 1 week.

You'll need a planning tool or an excel sheet to organize that. After each task your friend has fulfilled, he must give you the original time. You can then learn how long things need. On the other hand you'll learn how long you can expect the future things to take.

What I describe here is "agile Programming". You can use tools like Jira or Kanbanery.com for that.

WIth such a plan you have a good understanding on whats going on. YOu post reads to me that you pay but don't have a clue how far you are. That will help here.

As your friend should use a version control system, you should ask for access. Even if you don't understand the code, it is very relaxing to see if there is progress. You friend should commit several times a day to the source control, you should be able to see the changes. If he doesn't commit you have either a problem on code level (you should do your commits as small as possible and atomar) or he simply does not work at all.


Sidequestion 1: Use tools like "Jira/Greenhopper". Read about Scrum.

Sidequestion 2: 2 programmers might increase efficiency. But its not a given fact. 2 programmers need to collaborate and communicate. Please have that in mind -you need to make sure they do it at that level. On the other hand its very motivating for people to have somebody else to speak to. And you always try to make things quickly, because the other can understand how long it really took. But there also might be implications - you friends money will finally be earned by somebody else. He might worry about that.


2nd issue: Sorry, I am not good to ask that. Is he the type of person working as a ceo? If not, you could make a bonus paying at the end of the project (or at the end of a story). This is also motivating and you don't need to give out a percentage. I would give out a fixed bonus like for example 2500$ for the prototype and 5000$ for the working project. You can make it dependend from time: ready until 15.06. 5000$, to 01.07. just 4000$ and so on.

Hope that gives you some inspiration.

Cheers
Christian


## Answer 26195

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2011-06-11
- score: 3

This is one reason why so many people on this site push the "you need a technical co-founder" view.  There is no way for a non-programmer to evaluate the productivity of a programmer.

Too often people try to use lines of code, number of bugs, etc. as proxies for a sufficient volume of quality code production, but doing so encourages bad behavior.  Why write simple, elegant code when it is shorter than easier-to-write long kludgy code?  Why enter bugs into the system if they will be held against you?  You get the idea.

In the end, a programmer has been productive when things are getting done and the code is of good quality.  Without being a coder yourself, you have no baseline for how long a task should take, nor any way to evaluate the quality of the code.

If I were you, I'd consider making this or some other qualified person your technical co-founder so that someone on the decision-making team has a background in the stuff the product is made out of (code).



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
