## Membership software

- posted by: [Blind Rooster](https://stackexchange.com/users/-1/13656-blind-rooster) on 2011-10-03
- tagged: `software`, `credit-cards`, `memberships`
- score: 1

I am looking to create a business who's customers buy units of our product. It might even evolve to a membership situation where they are buying units on a scheduled basis each month. I want these units to be verified via an 800 number that the store would call in to and then deduct the number of units being used at the time. Any thoughts on software that could track that sort of thing? Or is there  a way to use a "re-loadable" credit card of sorts? Thank you in advance for any thoughts or suggestions.
Brian


## Answer 31084

- posted by: [Rob R](https://stackexchange.com/users/-1/13692-rob-r) on 2011-10-05
- score: 1

<p>If I understand correctly, you are looking for software that will both handle the credit card, which in time may warrant scheduled charges, and possibly a membership section.</p>

<p>I think an API, may be a decent option for yourself. Something such as, <a href="https://stripe.com/" rel="nofollow">Stripe</a></p>

<p>That way, you can basically code around another piece of software, such as a CMS that may allow you to easily build a member section.</p>

<p>I think overall, you may need to develop(or hire a developer) to build a custom solution as your requirements are not very standard. However, you may be able to get by on what was provided above.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
