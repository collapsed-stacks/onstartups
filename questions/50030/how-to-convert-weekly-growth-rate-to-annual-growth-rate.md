## How to convert weekly growth rate to annual growth rate

- posted by: [Omranic](https://stackexchange.com/users/-1/17941-omranic) on 2013-07-24
- tagged: `growth`
- score: 0

Our startup had projected a weekly growth rate of 10%, for the sake of future financial estimations/projections, how can we calculate annual/semi-annual/quarter growth rate?
I've already searched the web with no accurate conversion formula or calculation theory! I'm a bit novice in such financial fields anyway..

It's mentioned by Paul Graham at the following link that 10% weekly growth rate equals 142.0x annually, what that means and how it can be calculated?!
http://paulgraham.com/growth.html


## Answer 50031

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2013-07-25
- score: 2

There are 52 weeks in a year, so you need to increase the amount you start with by 10% and do that 52 times. 

In other words, 1.10 x 1.10 x 1.10 x ... x 1.10 (with 52 of them), or if you're mathematical, then that's equal to 1.1^52 (1.1 to the power of 52).

Most calculators can calculate 1.1^52 quite easily and it comes out to 142.042932



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
