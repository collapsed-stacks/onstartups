## Charging for a Web App

- posted by: [the angry burger](https://stackexchange.com/users/-1/15531-the-angry-burger) on 2012-01-10
- tagged: `webapp`, `charging`
- score: 1

This may be an in-appropriate question but we are looking at changing the way we charge our customers because the current system is complicated. The problem is that its hard to simplify it without risking losing revenue. Let me explain

Currently we charge customers for access to the web site. For example if the customer wants 10  users we charge them £5 each a month so

10 * £5 = £50 a month.

But we also have a "Foo" module that you can buy on a per user basis. So the customer may also want 3 of their users to have access to Foo as well at £4 per user

(10 * £5) + (3 * £4) = £62 a month

However this is a real pain as we have to manage which users have access to Foo. Don't allow them to give access to more than 3 users, all managed through roles, and it becomes complicated for them to setup access. Plus its not always the clearest to sell.

What we would like to do is charge them for a site wide licence so all users would have access to the Foo module. So in the above case we could charge them £12 a month for everybody to have access to the "Foo" module and we'd still be taking the same revenue.

However we'd be losing out in the long run as if they had wanted 5 people to have access to Foo in the current method we would make

(10 * £5) + (5 * £5) = £75

but the new method would still be £62

So I think really what I'm asking is does anybody know of a good way we could change our licencing that would simplify it without losing revenue. This is only an example. In reality we have a lot more modules and possibly (hopefully) a lot more users.

Or is our current method acceptable?


## Answer 34665

- posted by: [Brian Karas](https://stackexchange.com/users/-1/8465-brian-karas) on 2012-01-10
- score: 1

You need data on your subscribers to make an informed decision.

Let's say the average customer has 10 users, 4 of which also buy up to the Foo module.

Ideally, you'd set the price of the foo module to be equivalent to 5 or 6 users.  In some cases you'll make money, in some cases you'll lose money, but the average case should be on the positive side.

It's kind of a value pricing experiment.  People don't like making decisions like this.  They also don't like spending needless money.  Your goal is to set a price where it does not become a considered purchase to them.

Also, this partly depends on what the Foo module is and what your application is.  EG: if your app is a Sales-forcey kind of thing, and Foo module is something that provides global roll-up reports, well then only my sales VPs really get any value/use from that.  I might not want Foo to be a site-license because I'll feel like I'm paying money for something that only 12% of my users need.  But, if Foo is a cool charting widget, well then I could see how all of my users MIGHT be able to use that at some point, so I'll feel comfortable paying for it site-wide.


## Answer 34666

- posted by: [dnbrv](https://stackexchange.com/users/-1/15284-dnbrv) on 2012-01-10
- score: 1

First of all, you did your math the wrong way. In the second calculation, you take your price for module "Foo" as £5/mo. while it's £4/mo. in the first one. Thus, your total for 5 seats of module "Foo" in addition to 10 seats of the software is going to be £70.

Second, charging a flat access rate in addition to a subscription fee isn't a smart decision when you're trying to maximize revenue while reducing overhead on administrating the license. You need to bundle and charge more per license. If the subscription is £10/mo. and module "Foo" is £4/mo. then sell the "full-package" at £12.50-13/mo. This way you will increase per seat revenue while giving a sense of extra value.

However, in order to do this, you need to know how much your customers value modules (i.e. which ones they're more willing to buy in bundles). Some modules may be valuable only to a small number of your customer's users so they won't see the value in bundles.

If you want to charge a flat fee per customer then follow Brian's advice of finding out the average number of seats using that module and charging just above it.


## Answer 34673

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-01-10
- score: 0

In the long run what you really need is an accounting and billing system that permits this sort of flexible billing without too much effort.

Since you don't currently have such a system, you need an interim solution so you can have some time to improve your billing system.

When you have a new customer who wants to sign up why not offer them a special promotion as follows:

> Sign up for one year and we will let all your users have access to the
> FOO module for the first year for half price! That's right - here's
> how it works: Say you need 10 users but only 5 require access to the
> FOO module; well signup for our 10 user package, pay us for 5 uses of
> FOO and everyone else can use FOO for free during the first year! Why
> are we doing this? We believe that they will love FOO so much that
> everyone will want to continue using it after the first year is over.


Extend the offer to your current customers as well and you will have a year to fix your billing system.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
