## A question about statistics for Adwords

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-05-03
- tagged: `adwords`, `statistics`
- score: 5

I read your article about significance testing adwords ads using the Pearson's Chi Square formula. It was very well thought out for the layman.

I am far from being a statistician, so I wondred if could clarify a few points:

1. Can you apply this using the standard settings in adwords i.e. For Google to show the more successful ad more often, or should you use the "show ads equally" setting?

2. Can it be used ongoing. So youv'e found a winning ad, ditched the loser and created a new contender. The winning ad already has some clicks. Do you count them or start from a zero baseline for both ads the day you put up the new contender?

Look forward to your comments

Regards,

Keith


## Answer 10883

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-05-05
- score: 3

Thanks Keith, although I hope more people answer too.  :-)

1. You *must* use "show equally" for this to work, but *only if* you want to use my simplified formula.  If you want to show unequally that's fine, but then you need to compute `chi^2` using the (still pretty simple!) formula in the endnote rather than the `D^2` result.
1. You must start the experiment from scratch.  This is because I assume that the experiment shows those ads to the same people.  That in itself is a stretch in adwords because it's not exactly the same people, but rather the same general type of person searching right now with those keywords with your current adwords setup.

Fun related fact: Google's Website Optimizer -- same concept but with your website content rather than adwords -- uses exactly my technique, just with the original math.  (No need for "shortcuts" if the computer is going to compute the answer!)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
