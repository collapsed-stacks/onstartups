## What kind of software can be patented?

- posted by: [Abe Miessler](https://stackexchange.com/users/-1/4318-abe-miessler) on 2011-04-24
- tagged: `software`, `patent`
- score: 3

I've heard that only algorithms that are "non-obvious" can be patented.  What does this mean?

Can someone give me examples of software that is patentable and software that is not?


## Answer 23940

- posted by: [Matt](https://stackexchange.com/users/-1/8784-matt) on 2011-04-24
- score: 2

<p>Non obvious?  The requirement is simply that someone skilled in the discipline judges it non-obvious.  That seems to be an odd hurdle given that someone was granted a patent on use of XOR to create a graphical cursor. (google "xor patent" - Autodesk had to pay $25k to use something that had been used for years).  If that can be granted a patent, nigh on anything can.</p>

<p>You'll find some background over at <a href="http://www.oss-watch.ac.uk/resources/softwarepatents.xml" rel="nofollow">OSS Watch</a></p>



## Answer 26691

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-06-24
- score: 2

There is an [extensive discussion of the non-obvious principle](http://en.wikipedia.org/wiki/Inventive_step_and_non-obviousness) on Wikipedia.

What it means is pretty simple: if a skilled practitioner familiar with the current state of the art would consider that the patent's claimed solution to a problem is obvious, it should not be patentable.

For example, every working programmer understands that the way to solve the problem of "doubling each number in an array" would be to write a loop, iterate over each item, and double each item by multiplying it by two. Therefore a patent using that method would not be valid.

However, almost no programmer knows how to solve the problem of "given a NP-complete problem, solve it in polynomial time", so if you figured out how to do that, you might be able to patent it. It certainly wouldn't fail the "obvious" test!

Much of the dispute around software patents seems to stem from the fact that the US patent office has not been very intelligent in determining whether methods are obvious to skilled programmers, and they have granted an immense number of patents for extraordinarily obvious things.


## Answer 23941

- posted by: [chmike](https://stackexchange.com/users/-1/9453-chmike) on 2011-04-24
- score: 1

It depends of your country. In europe algorithms and programs can't be patented. But a technical solution involving a program run by a computer will be ok. A system involving multiple computers and devices would be ok. I saw a french patent for a Video On Demand system. 

So technical solutions may be pattented, but not a software. The cursor xor is a technical solution. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
