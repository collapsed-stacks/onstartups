## Code Review & System (Re)Architecture

- posted by: [Yuck](https://stackexchange.com/users/-1/11398-yuck) on 2011-06-28
- tagged: `outsourcing`, `management`, `project-management`, `team`
- score: 1

I've recently been brought on with a small startup to serve as their technical advisor to a group of developers offshore.  The product is an ASP .NET WebForms application.  One of my first tasks was to complete a code review, looking specifically for areas that perform poorly or may have bugs. I quickly found that the team has been working without any clear roadmap - code is hacked together to accommodate new feature requests as they come in.

I'm going to suggest that the code is refactored into several smaller projects and assemblies, with each serving a clear responsibility.  The developers have a wealth of knowledge on the product and so I need to be especially careful about how I approach this.  The last thing I need is stressed out coders or hurt feelings.  Still, we can't afford to continue on as in the past.  And the refactor needs to happen sooner rather than later.

Can anyone offer suggestions on how I can present the problems without making their hard work sound like a terrible mess?  If additional information is needed I can provide it - to a point.  I am working under an NDA so the detail will need to be obfuscated.


## Answer 26891

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-06-28
- score: 4

A good start would be to limit yourself to asking questions instead of giving answers.

"Why is this code all in one file?"

"What are some ways you could make the code easier for new developers to understand?"

Etc. Your questions can be pretty leading but you're just asking questions, which prevents people from going on the defensive.


## Answer 26899

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2011-06-29
- score: 3

You state that you were tasked to look for code that:

> perform[ed] poorly

or 

> may have bugs

I think you are a little bit off the reservation on this one with the desire to have beautiful more maintainable code.  

You won't win points with management taking time away from new features to rewrite working code.  However, I am sure they will all understand that the future maintainability of the codebase is important.

Why don't you start with profiling some code or picking some code that has defects and doing the kinds of re-factoring that you desire.  If you get your hands dirty and lead by example it might help.  Standing on a soap box and talking about refactoring and coding practices does not go over well - but if you show that the results are beneficial you might get some people to do the talking for you. 

Pick your battles.  Look for low-hanging fruit.  Be careful.




## Answer 26915

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-06-29
- score: 2

I'm currently reading Dale Carnegie's *How to Win Friends and Influence People*.  Despite the cony title, the book is full of fantastic insights that help you in this kind of situation.  Here is a summary of some of them:

 - Don't criticize the code or people's work.  That will make them defensive and reluctant to change.
 - Try to have a discussion with your employees in a way such that the changes you want become their ideas.  Let them take credit for the ideas and they will run with it.
 - Get really excited about the desired changes and show them the benefits of them.  If you can transfer this excitement to your employees, they will want to make it happen.

My simple statements don't do Carnegie justice, but I hope you find them helpful.


## Answer 26896

- posted by: [Dan Williams](https://stackexchange.com/users/-1/2138-dan-williams) on 2011-06-28
- score: 0

You also might want to try being as honest as you can with them:

"I don't want to come off like a jerk, but the reason I was hired is to provide some clear direction for the code base, at times this may sound like criticism, but it's not.  It's an overwhelming job, and I'll need your expertise with the code to help me get it done.  I really, don't want to offend anyone, but I'm sure as everyone knows, there are times when you have to pull a project back to center."

Meh, something like that anyway.  People like to "help" others, makes them feel needed instead of just being told what to do and is often a better attitude for both sides anyway.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
