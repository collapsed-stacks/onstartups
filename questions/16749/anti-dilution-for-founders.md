## Anti-dilution for founders?

- posted by: [Filippo Diotalevi](https://stackexchange.com/users/-1/4482-filippo-diotalevi) on 2010-11-19
- tagged: `finance`
- score: 3

I read that it is common/possible for investors to ask for anti-dilution clauses.

Is there a way a co-founder can protect himself against dilution? Of course, dilution will eventually happen during later rounds of financing, but it is possible/common for example to require that all co-founders are equally diluted in later round of financing?

*Update*

*The specific case could be that some shares are issued and they're distributed to investors and some, not all, cofounders (f.i. as a bonus). In this case the other cofounders (the ones that didn't received shares) are more diluted than the others. 
Is that possible? In the case, how can someone prevent that?*




## Answer 16759

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2010-11-20
- score: 8

What you're suggesting is mathematically impossible.

First, let's start by looking at how an anti-dilution clause works by using a super simple example.

1. The founder sets himself up a company and declares that it will have 100 shares. He owns them all, so he owns 100%.

2. He sells 20 of those shares to an invester. Now the investor owns 20% and he owns 80%.

3. Later he wants to raise more money, so he issues 20 more shares. Now there are 120 shares outstanding. So:

  * The newest investor has 20/120 = 16.67%.
  
  * The original investor has 20/120 = 16.67%.
 
  * The founder has 80/120 = 66.67%.  

4. The original investor is grumpy about this. He wanted to own 20% and to KEEP ON owning 20%. So he uses his anti-dilution clause allowing him to purchase more shares to get back up to 20%. Everybody launches Excel and runs Goal Seek to figure out how many shares he has to get. They discover that if they issue another 5 shares and sell them to the old investor:

  * The newest investor will have 20/125 = 16%
  
  * The original investor will have 25/125 = 20%
  
  * That leaves the founder with 80/125 = 64%.

If you're asking, "how can the founders protect themselves against dilution the same way," well, they can't, because there's nobody else to take percentage points FROM, and the percentage has to add up to 100%.

Now, if you're asking "how can you make sure all the co-founders are **equally** diluted," well, that's essentially automatic. Everyone without an anti-dilution right will naturally end up owning a smaller percentage of the company, equally, when new shares are issued. 

This is just the nature of how percentages work; it has nothing to do with startup finance :)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
