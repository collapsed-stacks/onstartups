## How to calculate avg account lifetime in SaaS model?

- posted by: [Jim](https://stackexchange.com/users/-1/19720-jim) on 2012-09-19
- tagged: `statistics`
- score: 2

I wish I had taken a stats class, but I didn't so I'm hoping someone out there can help me out. 

We sell a product with a recurring monthly fee. I'd like to be able to figure out how long the average customer keeps their account open before cancelling. 

The problem is that at any point in time, most customer accounts are still open and I don't know when in the future they will quit. So I don't know how to write the query if I use existing and cancelled customers. On the flip side, if I only queried customers who already closed their accounts, it seems like my stats would be skewed in a bad direction since it wouldn't take into account any customers who have had their accounts open for a long time (and are still open).

Any easy solutions or formulas for this? If not I can just work off of cancelled accounts.

Thanks!


## Answer 42069

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2012-09-19
- score: 1

I am not statistics expert, but it sounds like it's too early to get an accurate number.  You don't know how long your active ones will stay.

My advice is to just guess.  Use that as a basis until you get some actual numbers.

I would conservatively guess if this is to compare to your cost of acquisition (ie. internal cash flow), or optimistically guess if it's for a pitch deck to investors.


## Answer 42142

- posted by: [Jim](https://stackexchange.com/users/-1/19720-jim) on 2012-09-21
- score: 0

After thinking about it a bit more, I came up with a stat I think will work for me. I figured I'd share it in case anyone else happened across this thread.

Each month I'm going to look at all cancellations over the prior 3 months and will figure out the average length of time those accounts were open. I can then compare that average month by month to see if it is going up, down, or staying the same. 

A 3 month interval (for our business) should be long enough that we'll have enough accounts to get decent numbers but short enough to give us current information. Thanks all for your help.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
