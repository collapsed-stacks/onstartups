## What happens if you write a "bad invalid EULA"?

- posted by: [Stu R](https://stackexchange.com/users/-1/9313-stu-r) on 2011-04-12
- tagged: `terms-and-conditions`
- score: 6

[From this answer](http://answers.onstartups.com/questions/23199/how-do-i-protect-myself-when-offering-software-and-training/23200#23200) someone wrote

> In my EULA I also include that the
> maximum liability shall not exceed the
> purchase price of the software

and a comment saying

> also a good example of a bad invalid eula in most countries

Do i need to worry about writing unenforceable things in my EULA? Is the rest of an EULA enforceable if i have a few invalid or unenforceable terms in my EULA?



## Answer 23221

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-12
- score: 4

You should put a severability clause in your EULA to protect your self in this kind of situation.  Nearly every EULA has one, so just adapt one that is out there.  You should avoid clauses that are blatantly unenforceable (giving up first child for violation) but anything that you commonly see in other EULA's (including a clause that limits damages to the price paid) is fair game.

The law relating to what is valid/invalid in a EULA is very unclear.  Companies do the best to protect themselves as much as possible, but no one really knows what it truly enforceable until you have a lawsuit over it.

An atty can always argue that one invalid clause will invalidate the whole EULA and you won't know the answer until you go to court.  (Note that this can still happen even if you do have a severability clause.)


## Answer 23214

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-04-12
- score: 3

(Not a lawyer)

Generally No, each point in the contract should stand on its own, unless another point contradicts it.

But the law is complete rubbish and open to the interpretation of the highest bidder (most expensive lawyer ... the one who can BS the best) ... learnt that the hard way. "Right" makes very little difference, its perception and money. How can people view it and how much money are you prepared to throw at defending it. 

When we started, we had a company walk with $x00K because we had $0 to chase them with (they had it all) and their lawyer found a claim they could make (BS though it was) that meant we had to prove our side rather than rely on our existing contract and previous payment history and the deliverables they were still using ... it was cheaper to try it on with a lawyer then pay what they owed ... (oh, don't give source code till you have been paid, use escrow) ... 7 years later they were shut down and imprisoned by ASIC our governments corporations body which was satisfying, but we never got paid.

So therefore

Basically if I was attacking your EULA I would use the invalid points in it to reduce the validity of your contract and try and get it annulled. 

That said putting those clauses in there stops people trying it on and gives you "layers of defense", that you can fight them off with ... Limiting the liablity is something they have to fight and get a ruling on before proceeding, costing them and makes them think.

For me contracts like a computer program, your just writing the rules and baking in the security upfront. If the hacker works out the cheat, your still comprimised, they still nail you. 

... the other (and real point I as intending to make) is, how much are you clients going to care if there is an issue? 

If your the key to their business and they lose $20M per hour when your software is down, the you want to cover yourself damn well and charge them accordingly. On the other hand if all that is going to happen is they get annoyed and either come back in 2 hours or start using another service then you EULA doesn't have to be quite so iron clad, just enough to cover the usual items.

**Tests for effort put into a contract**:

 - Are they going to get money by suing me? Yes / No
 - Are they going to save money by suing me? Yes / No
 - Is the amount they end up with significantly greater than their cost of suing me? Yes / No
 - Are they likely to win their claim? Yes / No 

If the answers are Yes, then spend lot on the contract with an appropirate Lawyer. We have a specific Software IP lawyer we use for the majority of our work but that may not be appropriate for you. 

If No, get a standard EULA that matches your situation and get a Lawyer to refine it for your specific nuances.

(Again, not a lawyer)



## Answer 23212

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-04-12
- score: 0

Depends on the rest of the Eula and the jurisdiction in place. Do you have a clause declaring the eula partially valid if a part turns out invalid / unenforcable? If not - there goes the eula. Also note that all loss limitations are a hard thing. There are some areas where by law you can not limit liability. Gross neglect is one, which logically includes not fixing defects in a product, or having sub-standard testing in place (which is a funny one given most developers dont really do any testing - so the standard is quite low).

Ask a lawyer.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
