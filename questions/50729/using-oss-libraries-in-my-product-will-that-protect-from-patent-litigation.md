## Using OSS libraries in my product - will that protect from patent litigation?

- posted by: [Gupshup](https://stackexchange.com/users/-1/27447-gupshup) on 2013-09-02
- tagged: `intellectual-property`, `patent`, `open-source`, `software-licensing`
- score: 0

I am working on an innovative product that uses a GNU GPL licensed library and per GPL needs open-source my work as well. Could that protect me from patent litigation?

I am worried since my former partner has filed for an overly broad patent - in fact it claims the above library as its IP as well - I am very sure the patent might not hold up in close examination. I am conflicted if I should challenge this patent by disclosing to the USPTO.

However since patent litigation is so expensive, and could put the brakes on my fledgling company, I feel this might be a shakedown from a vengeful man with deep pockets.

Would open-sourcing my code, preempt patent litigation?


## Answer 50733

- posted by: [adrianh](https://stackexchange.com/users/-1/4599-adrianh) on 2013-09-02
- score: 2

Short answer no. Especially if the code is related to the work being claimed. Code being open sourced does not automatically protect it from patents.

You need to go talk to an IP lawyer.


## Answer 50747

- posted by: [Chelonian](https://stackexchange.com/users/-1/12506-chelonian) on 2013-09-02
- score: 1

> Would open-sourcing my code, preempt patent litigation?

Unfortunately, nothing exists in the universe to prevent *any* litigation; at least in the U.S., as you must already realize, anyone can sue anyone for anything.  More specifically in your case, no, something being open sourced doesn't confer patent litigation invulnerability, magically blocking litigation before it actually gets started.  And it doesn't even mean that you will win in court if it goes to that; there is currently no mechanism in patent law that goes like this:  "Oh, the software that violates the patent is *open source*?  Oh, why didn't you say so!  It's immune!  You can violate the patent with impunity.  Have fun."  

What does allow a defense, in court or through USPTO's defined processes, are the traditional ways to invalidate a patent:  prior art or showing that you don't actually infringe any of the claims.

For more on patent suits vs. OSS suits, read up about the JMRI case, in which the patent holder wound up *losing* a lawsuit to the OSS developer for infringing the Artistic License (which may be applicable in your situation):

 - http://en.wikipedia.org/wiki/Jacobsen_v._Katzer 

 - http://jmri.sourceforge.net/k/History.shtml  





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
