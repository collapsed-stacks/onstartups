## It's ok to launch a software product when Beta testing is not fully finished?

- posted by: [Nestor Sanchez A](https://stackexchange.com/users/-1/1476-nestor-sanchez-a) on 2012-04-15
- tagged: `software`, `launch`, `beta`
- score: 3

I'm having trouble finishing the Beta testing period of my software product.
In particular it hangs/crashes in some laptops with low to moderate memory and speed capabilities.

This problem is hard to reproduce and solve, so it could take me weeks or even months working on this. But I want to launch my product and start charging for it ASAP (to users who does not suffer this issue, of course).

Considering that this problem can affect, lets say, 25% of my users/customers base,
and that the product starts in Trial mode for 30 days free of charge...

Should I solve the problem first and ensure a reasonable reliability to all of my users?
or should I start launching the product and charging now for those able to do it?

Thanks for your opinions and suggestions!


## Answer 38200

- posted by: [TimJRobinson](https://stackexchange.com/users/-1/4907-timjrobinson) on 2012-04-15
- score: 5

If by launch you simply mean make it available to the general public then yes that should be ok. 

But I definitely would not try and do a big launch with press / blogger attention etc while the product is in it's current state. Only attempt widespread adoption when it's working well enough that 95%+ of users that want to use your app will be able to use it. 

It seems cool because "75% of the people will like it and who cares about the other 25%". In reality those 25% will talk a lot more about the bugginess than anyone else and you'll have a lot of users seeing comments about how the product is "not ready", "in a buggy state" and not even attempt to use the product because of that (and these comments are going to stick around for months or even years holding you back even when the product is 100% bug free). 


## Answer 38201

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2012-04-15
- score: 3

Find out what laptop configurations cause the problem (even if you can't fix it yet).  Then just set your system requirements to exclude those.  Perhaps you can even run a detection on application load that checks if they meet the requirements and just show a message if they dont.

This way you don't have unreliable software for 25% that signup and you still get to launch now.


## Answer 38211

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-04-15
- score: 1

Why do you want to end the beta test, wthout solving the problems found in the beta test?

If the answer is, you want to make money- then consider this. Many people buy software without a 30 day trial. Suppose your product is widely successful and 1,000 people want to buy it before the end of the trial. Or 1,000 people buy it right after the 30 day trial ends.

By your own admission, 250 of those users will not be able to run the software. And yes- many people will assume that the "bug" is a trial limitation and still buy it anyway.

So what will you do with 250 people who paid money for your software, but can't run it??? They will either do a chargeback, or demand a refund. Either way, your credit card processor is going to cancel your account. So much for making money.

Finally, you need to check with a lawyer about your software's warranty terms. There are inherent warranties associated with selling products to consumers in the US, and selling a product that doesn't work on 25% of all computers, without an explicit warning, could get you into big trouble.



## Answer 38242

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2012-04-16
- score: 1

It's in the nature of software that you can't in the general case guarantee that it will function as intended. So Ts & Cs are very important. And bug fixing never ends.

Your issue is confined to systems with

> low to moderate memory and speed capabilities

So you have a choice whether you want to highlight to prospective users and purchasers that your product requires certain system characteristics - and if these are simply described your software could even check whether the system it is being installed on meets those requirements.

In my view, you need to learn all you can from existing users, ask their opinion, and make sure that there's a clear way for users who can't get the software working to see what's going on and to get a refund if it doesn't work for them. A 7/14/28/30 day free trial is also a very familiar approach in the market that works fine.

Then launch, and offer the best service you can to all users, so those who can't use the software still have a reason to recommend you.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
