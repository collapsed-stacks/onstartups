## Would you sign this liability clause?

- posted by: [Roger](https://stackexchange.com/users/-1/14705-roger) on 2011-12-07
- tagged: `legal`, `legal-documents`
- score: 5

I am going to get this checked by a lawyer, but I was wondering if people generally sign a clause like this (as the Contractor)?

>"The Contractor indemnifies --Company-- for all liability (including but not limited to liability caused by negligence), costs and losses suffered by --Company-- as a result of any claim made or proceedings brought against --Company-- arising from, or as a result of, the performance (including non-performance) of the Services."

Just seems pretty open to me, and they just say that "That's what PI insurance is for".

Thanks.

Update: This is relating to contract programming services, for a project that isn't defined in the contract, so more just hourly contract services.  I'm just not sure that I should be taking full liability for any bug that may happen in the future.


## Answer 33431

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-12-07
- score: 4

No, I would tell them to get lost. Period. This is unreasonable. They do not limit this to gross neglect - you are fully liable for any claim even if you do your job right, as well simple negligence. Develop software, has bug - you fix bug. They wont pay your time fixing the bug. Now, one may say this is "ok for a product." Yes. But when you develop software, bugs are part of the process. So that is why you have testers, unit tests, etc.

Given this formulation you are liable to pay for the work of the project test team unless you provide flawless code. Check in something bad into the build server once (simple negligence) - you are liable for the loss of productivity of the other team members. Now, this is REGULARLY happening during development processes. But here you are liable.

Whoever wrote that did not think about edge cases and either is no lawyer or should be thrown out for gross incompetence.


## Answer 33444

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2011-12-07
- score: 4

You need to have a lawyer review and strike / modify this portion of the agreement. Aside from what everyone else here has said, imagine this:

You work for months on their project and they stop paying you. You keep working, asking for payment. They refuse to pay you. Under the terms of the indemnity clause above, if you stop working for them due to lack of payment, you are liable to them! Does that make sense? You become their indentured servant.

In addition, **any** time someone wants an indemnity clause your attorney should recommend that they indemnify you too.



## Answer 33436

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2011-12-07
- score: 3

Pass it to your PI underwriters and see if they'd be happy for you to sign it. If they don't like it, they'll likely give their reason(s) which you can use in your negotiations.


## Answer 33427

- posted by: [Mike Scott](https://stackexchange.com/users/-1/6167-mike-scott) on 2011-12-07
- score: 1

You need to have conduct of cases against which you are indemnifying the company. Otherwise they can just settle for any price and then send you the bill.


## Answer 33537

- posted by: [Donny Nyamweya](https://stackexchange.com/users/-1/14938-donny-nyamweya) on 2011-12-09
- score: 1

If the details of the project are not on the contract, then make sure that on the addendum that defines the tasks and deliverables of each project make this clause more defined.
Off the top of my head, I would wonder if this means that if you have a mutual NDA with them and the -company- breaks it... does this no-liability clause exempt them from that liability? What if they divulge your NDA-protected information (e.g, you give them a discounted rate and they publish it, your other customers demand the same rate, you loose money...)

As a rule of thumb, whenever I discuss work with a client, I try to send them my contract when I get theirs, or even if they send me theirs, I look through for things such as these that are scary.

Contracts and an agreement, so you do not have to tell them to get lost. Understand your concerns and base them on sound ground (not emotions), and then explain to them (in writing) what is not acceptable to you. More often than not, they will adjust their conditions. Even if the discussion is not conclusive, the fact that you disagreed with the clause in writing is SOME evidence that you did not agree to it. If they want your services and are not arrogant, they will clarify the clause in writing (staple their clarification to the copy you sign and refer to it).


## Answer 33538

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-12-09
- score: 1

> This is relating to contract programming services, for a project that isn't defined in the contract, so more just hourly contract services. I'm just not sure that I should be taking full liability for any bug that may happen in the future.

It's a bad contract. Do not sign. In fact, for services like this, where your work output is mingled with everyone else's on the team, you are liable for circumstances well beyond your act of creating the code. 

Generally, from anecdotes I have read, PI insurance is effective only when you continue to pay the premiums, which for a software consultant can range into the low thousands per year. So if you pay the premiums while you work for such a client, and then stop paying the premiums, you are not covered if they come after you for liability later. PI insurance becomes an annuity payment that you must continue to make into the future. At the going rates commonly found for contract software development many consider it not worth it. 

> Are you saying that the clause needs to be more specific in what I am indemnifying them for, and that the clause is too broad, or just that if there is a case for liability it needs to state something about how it will be resolved and a limit to my liability? 

It will get *very* complicated when you attempt to negotiate a detailed liability agreement. Again, the wisest course of action here is to line out the liability clause and see if they agree to it. 

Essentially, as a contractor, you and most of us do the work equivalent of an employee, for slightly higher rates of pay. Do software development employees take out PI insurance? No. 


## Answer 33618

- posted by: [Darren Cook](https://stackexchange.com/users/-1/14258-darren-cook) on 2011-12-12
- score: 0

The usual way I work (when working as a freelance software developer) is: if the project is for a fixed price, where the spec is clearly defined, I offer to fix bugs for free. I also give the client some examples of the differences between bugs and new features. (E.g. a typo in a menu is a bug, a request for another menu item, or changing what an existing menu item does, is a new feature.)
Also, bugs are inevitable, so I try to allow for this in the quote.

When working on an hourly basis, I explain to the client all future work, including bug fixes, also has to be on the same hourly basis. For clients who are unhappy with this I suggest we thrash out the spec and use a fixed quote.

Sometimes projects have switched from fixed price, to hourly basis. Then it gets a bit more complex, and I just try and keep everything open and honest: if the bug is in the part delivered under the fixed price then I fix it for free, outside the hourly tracking. Source control logs can help here :-)

Not really answering your question but I'm concerned by your client's response. Are they a big company? If so, getting the insurance they suggest sounds like a good idea, and clear all contracts with your insurance company!




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
