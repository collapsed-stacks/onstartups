## What do I need to know about storing people's money in accounts for my website

- posted by: [JonF](https://stackexchange.com/users/-1/11225-jonf) on 2011-12-13
- tagged: `website`, `research`, `merchant-account`, `accounting-method`
- score: 1

I am developing a website where users will be able to transfer money to their account on the website.  They'll eventually be spending some money and withdrawing money back into their accounts original bank account.  Think of it as a paypal account. I'm in the early phases of this and I'm just trying to learn what I need to know.  I already have a strong background in software development but I've never done anything like this before.  I imagine there are some escrow services that I can utilize?  Where can I get information to get me started on making this happen?


## Answer 33671

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-12-13
- score: 2

Definitely a talk to allawyer to start with. THis may require licensing as financial institution of SOME sort, even if not a bank. They will gladly tell you the more detailed requirements, if any apply.

Then a grasp of basic accounting.


## Answer 33669

- posted by: [Matt](https://stackexchange.com/users/-1/14496-matt) on 2011-12-13
- score: 1

<p>Are you operating as an actual financial institution like PayPal or, say, Ally Bank? It sounds like you just want users to be able to add or withdraw credit to/from their account for purchases.</p>

<p><a href="http://www.namecheap.com" rel="nofollow">NameCheap</a> does something like this: you choose how much you want credited to your account, and it performs a checkout via Paypal, for example, for that amount. So NameCheap has been paid and then I think they just update their database to record the transaction. Same with withdrawals.</p>

<p>I like this method. Keep a balance in a central business account dedicated to this, where you'll accept payments and debits from/to your customers. Keep an accurate, well-maintained, secured, and backed-up database recording each transaction. This way you can know how much each user has in their account currently.</p>

<p>I don't know any legal implications, but this is how <em>I</em> would do it, anyway.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
