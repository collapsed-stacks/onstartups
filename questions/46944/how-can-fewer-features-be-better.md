## How can fewer features be better?

- posted by: [Ken](https://stackexchange.com/users/-1/23746-ken) on 2013-01-27
- tagged: `software`, `getting-started`, `books`
- score: 7

Just today I started to get interested in this field and I've started with [Getting Real][1]. I kept seeing answers here that recommend it and it also seems trustworthy.

However, one thing I don't get is this:

> We'll cover the concept of less throughout this book, but for
> starters, less means:
>
> - **Less features**
> - **Less options/preferences**
> - Less people and less corporate structure
> - Less meetings and abstractions
> - Less promises

I understand most of these, but "less features"? why?

Later in the book they mention *[Writeboard][2]*. I Googled it to see what we're talking about, but to be honest I was kind of disappointed. I assumed it was something like an online OneNote or something..  
It's just a place to put text in online.

It **is** useful IMO, don't get me wrong, but if it had more features wouldn't it shine much brighter? Maybe if you could also draw and not only type text, maybe you could drag & drop images, or attach files, and so much more.

**Why shouldn't my application thrive with features to make the user experience as best as I can make it?**

*By the way, that doesn't have to mean that my software would be even a tiny bit more complex or intimidating.*

Also, why less options/preferences? people want to be able to customize their programs. Think of a world where you can barely do that.. isn't it just awful by comparison?


  [1]: http://gettingreal.37signals.com/
  [2]: http://123.writeboard.com/new


## Answer 46945

- posted by: [frenchie](https://stackexchange.com/users/-1/15155-frenchie) on 2013-01-27
- score: 12

There's a quote that goes something like *"perfection isn't reached when there's nothing left to add but instead when there's nothing left to remove"*. Search engines used to look like the Yahoo homepage and then Google removed every feature they could and I think they were just left with the search bar. But less features doesn't mean less capabilities; it's just that you want the features to be revealed as the users get more involved with the product, not upfront. The opposite example would be MS Word: you need to take a class for 6 months before you can use it to write a letter. 

Getting Real talks about startups and STARTING a business: you start with a simple product that's focused on few features and then you add them as the business evolves. Facebook started with just status updates. **You start simple, and then you add.**


## Answer 46968

- posted by: [Boris](https://stackexchange.com/users/-1/11773-boris) on 2013-01-28
- score: 4

'Getting Real' is good book, heavy on substance, but heavy on hype and over-simplification too.

People love to quote famous writers and throw stuff like 'fewer is better', 'small is beautiful'.

More is Actually Better
=======================
As you have probably noticed, quite often, more is more. What a surprise. That is why Microsoft Office, while considered bloated by many, is still the most profitable software in the world.

You Can't Do More
=================
You should forget the literal interpretation of the 'less is more'. Be smart and think about it. The real problem is people **significantly underestimate** how much effort it takes to implement a given feature. It takes even longer to do it well. And it takes, again, much much longer, to implement it in a **notably good** way. (Think 'Paper' for iOS)

Do As I Do, Not As I Say
========================
If you look at 37 Signals' own products, you will notice that they add stuff over time. They have almost never removed features. It is logical, and makes sense, but is inconsistent with the advice they give.

Focus
=====
So, even if more is more, you can't do it all. You can't even do much. What you can realistically hope for, is to correctly identify the core functionality of you app/idea, and to put all your efforts into it. 

In the end, if you succeed in making it good and satisfying beyond people's expectations, it might just be enough for success.



## Answer 46955

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2013-01-28
- score: 2

Features add complexity. Complexity makes usability more difficult and increases development and maintenance time.

Best is to find the sweet spot, with just the right balance between features and complexity.


## Answer 46963

- posted by: [scunliffe](https://stackexchange.com/users/-1/1103-scunliffe) on 2013-01-28
- score: 2

Less features is better.  One of the biggest problems in software is that developers love to make stuff. (*it's in our nature, and yup I'm guilty too*)

 > Product Guy 1: Can you make this blue?...
 >
 > Product Guy 2: Nah. Wait how about purple?...

 > Developer: How about we just make it configurable!
 > I'll need to add a new table to the schema, store the current value in the session, build a configuration page with a color wheel widget that lets you choose the color...

It takes a lot of restraint for the developer (and product management) to say no - ***we don't need this***. Or as they often say in Agile Development **YAGNI** (Ya Ain't Gonna Need It).

Both groups of people should be focused on what features the end user actually needs.  Do they need to be able to export this data? No? then don't waste time building the export wizard.

When indecisive about a feature... I like to ask myself... "Are we going to lose customers if we don't add this feature?" - If the answer is no or likely not then you need to ask yourself if it is worth adding.


## Answer 47027

- posted by: [Hans Fremuth](https://stackexchange.com/users/-1/17050-hans-fremuth) on 2013-01-30
- score: 1

<p>I am missing an important issue so far: <strong>product-market fit</strong>. Unless you are building a product for yourself, YOU ARE NOT THE CUSTOMER. You may think you know its needs well, but you WILL be wrong on many parts. Starting with less means less wrong assumptions (and therefore less waste of your efforts).</p>

<p><img src="http://i.stack.imgur.com/BV1Pk.jpg" alt="Focus on product-market fit"></p>

<p>Entrepreneurs are passionate and inevitably opinionated (this is a good thing). It's a good strategy to start with less, get surprised by user feedback, learn from it and <em>then</em> home in on additional features that hit the mark better.</p>



## Answer 47048

- posted by: [Brunno Silva](https://stackexchange.com/users/-1/9710-brunno-silva) on 2013-01-31
- score: 1

“Simplicity is the ultimate sophistication.”
― Leonardo da Vinci

All features in your app add value to it... and cost for you to maintain them.

Every feature means more code, more bugs, more user training, more specs, more designs, more docs, more performance issues, but not always means more value for the user. Indeed, 20% of your features shall represent 80% of your app's value.

**"Less features"** is just another way to say **"Stick with the 20% that matters and forget the 80% of headache!"**



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
