## Plan B In Case Development Source Goes Away

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-13
- tagged: `development`, `strategy`
- score: 2

I’m building a SaaS product. My coding is outsourced to a development company I’ve worked with for years and have had great success with (on other projects). I have no issues with them and hope our relationship continues well into the future.  

My question is this. What do I need to do to have a Plan B in case something unforeseen happens to my development company? I’m not talking about them stealing the IP, I mean what happens if they cease to exist?  What sort of contingency plan do I need to create that addresses a scenario whereby my third party development team can no longer support my product development? 

Bringing development in-house is not an option for now. I’m bootstrapping the new product and prefer to use a third party development source.  Do I need to vault the source code somewhere now? It's a PHP/MySQL based application. Thoughts? 



## Answer 1176

- posted by: [Del Putnam](https://stackexchange.com/users/-1/671-del-putnam) on 2009-10-13
- score: 3

You should ensure that you always have a safe copy of the most recent version of all of the code.  Find out what sort of source control system your contractor uses.  Ask for access to that.  See if they can periodically give you a full backup of the section of their source control system that houses your code.

If you aren't technically inclined, then try to find someone who is to help you.  Either set up an automated job (or do it manually) to periodically acquire the most recent version of all of the source code.

This situation has actually happened to me.  I have had to take over code that was developed by a third party.  It is never a fun thing to do, but it is certainly possible.  If the code works, I'm sure you will be able to find some other developers who can pick through it and figure it out.  It may not be a fun task, and I'm sure you will find some "gotchas" in there, but a good developer will be able to help you with this.

To understand your risk, you may want to review the company's financials or talk to some references.

To mitigate any risk, perhaps you could find a technically minded person whom you trust and who would be willing to help out once in a while for a small fee.  You could then work with that person to basically "audit" any source documentation and architecture diagrams that your contractor may have.

You might also be able to get the contractors to review their code with this person.  That way you will have someone who can point any new contractors or other developers in the right direction if your current contractors "go away".

Let me know what you end up doing.  I'm sure others have this same need.


## Answer 1170

- posted by: [Arpit Tambi](https://stackexchange.com/users/-1/309-arpit-tambi) on 2009-10-13
- score: 1

I hope you have full control over domain registry and hosting.

Do you backup often? Keep regular backups.

Is code well-documented? I'm sure it won't be. Documentation will help new developers to quickly take over the code.

May be you should seek advice from your current developers ;)


## Answer 1185

- posted by: [Scott](https://stackexchange.com/users/-1/88-scott) on 2009-10-13
- score: 0

Agreeing with Del (and, I hope, adding some nuance):

 1. On a daily basis, you need to ensure that you have a fresh copy of all the source code squirreled away where the developers can't reach it.  That means that the repository they are using isn't good enough:  you need a vault to which they do not have access.  This would be true even if you were developing in-house.

 2. I want to reinforce Del's point that if you don't have the skills to do code reviews yourself, you need to bring in somebody who can do so once in a while.  It doesn't have to be very expensive.  Again, this would be true whether your developers were in-house or not. Code review is an absolutely vital process that ensures that what you're developing will remain robust, secure, efficient, and appropriately documented.




 


## Answer 1186

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-10-13
- score: 0

Great answers above.

If they're not using version control, you shouldn't be contracting with them.  Since they're good, I assume they are.  So you should have backups of the entire version control system.

If the platform you're developing on is virtual, perhaps you could snag nightly backups of the entire image.

**If you're that worried, find another consulting company right now.**  Don't let them write code of course, but interview them, call their references, make sure they know the specific technologies you're using, and have your existing company draw up a "transition plan" which you could execute should they disappear.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
