## I want an effective solution to prevent piracy and manage licensing of my java desktop application

- posted by: [user893664](https://stackexchange.com/users/-1/12839-user893664) on 2011-08-19
- tagged: `licensing`, `software-licensing`
- score: 3

I am developing software that will be useful during search engine optimisation of a website. This software is a desktop java application.

I have heard that (specifically) Java applications can easily be hacked into.

Are there good solutions that prevent piracy and allow me to sell licenses of my software?



## Answer 29055

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-08-19
- score: 12

<p>I'm founder of the company that makes <a href="http://wyday.com/limelm/">LimeLM</a>, a licensing and online activation product. We have examples showing <a href="http://wyday.com/limelm/help/using-turboactivate-with-java/">how to use LimeLM &amp; TurboActivate with Java</a>. Also, if you want to prevent your compiled jar from being decompiled we recommend using <a href="http://proguard.sourceforge.net/">ProGuard</a> in tandem with LimeLM. ProGuard is a free and open source obfuscator for Java.</p>

<p>If you have any questions we'll be glad to give you a hand.</p>

<p>Tell me if this helps.</p>

<h2>What's the use of copy protection?</h2>

<p>This point was raised in another answer, so I'll address it here. Every copy protection can be cracked. This is an indisputable fact. So that raises the question: what's the point of copy protection if it can be cracked?</p>

<p>Here's the answer: <strong>casual piracy</strong>.</p>

<p>Customers using the same product key over and over again (aka casual piracy) can cost you real money. It's rarely malicious -- these customers aren't wringing their hands while giving their best evil villain laugh. It's much more banal. It's usually the department in a company that buys the licenses is different than the department in the company that actually handles the licenses.</p>

<p>This is why you <em>need</em> strong hardware locked licensing. It will tell your customers when they've used their allotted licenses so they can purchase more. Then they can purchase more licenses and be merrily on their way.</p>

<p>The Business Software Alliance does a yearly study on casual piracy -- check out their studies if you need further proof.</p>

<h2>But what about crackers?</h2>

<p>If it exists on a computer it can be cracked. You can't stop crackers. All you can do is increase your revenue by dealing with casual piracy.</p>



## Answer 29057

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-08-19
- score: 2

> I want to know of a good solution that prevents piracy and allows me
> to sell licenses of my software.


There is no good copy protection.

Look at all the high cost games, all spending huge amounts on copy protection and every approach is cracked fast. Game over.

Go for something cheap (computer name, SID vs. license file) to keep casual copying away and otherwise forget it. People want to copy it? It will be copied and your copy protection will be laughed at, regardless how much you spend.

They can not even keep Blue Rays copy protected. Or AAA games that spend significant amounts of money on copy protection schemes.


## Answer 29091

- posted by: [Xaqron](https://stackexchange.com/users/-1/11178-xaqron) on 2011-08-20
- score: 1

The best solution is protecting your product by `design`. If possible you should not ship the most important part with the software. This part is usually some of your application `business rules` and some other times it's some kind of `data`.

In your case, a good Idea is shipping `user interface` as desktop application and make it dependent to some sort of updates.

Example 1: Antiviruses need to be updated with the last virus signatures (`data` is critical here, and the engine is shipped with product)

Example 2: You have a diet program which gets some information from user (sex, age, height, weight...) and offer a weight loss program. Hide the `business rule` (diet program) by connecting to a web service over the internet.

Remember, due to different internet speed of users you should limit this connectivity and don't use it for real-time sensitive works (like painting on a canvas).

So, you need to think if it is possible to do some change in design instead of looking for theft-proof software locks/obfuscators.


## Answer 32425

- posted by: [Dominic](https://stackexchange.com/users/-1/14333-dominic) on 2011-11-09
- score: 1

(Disclosure - I work for Agilis Software, who provide Java license management tools).

First of all, there are well-tested and sophisticated commercial license management solutions out there. Since your application is in Java you probably want to make sure the licensing tool is multiplatform Java too, so you don't introduce platform dependencies. This is also a good sign that the vendor actually understands the special issues raised with protecting Java apps (and not just wrapping some C code and calling it a Java library).

When it comes to security there are actually two independent issues to consider: 
- Protecting your intellectual property (IP), and
- Ensuring the license check is not circumvented.

Techniques that meet the latter goal include checking a digital signature of the license-checking library at run time (to ensure it hasn't been spoofed or tampered with), exception based flow of control and flow-control obfuscation. Encryption is the usual approach for the first goal, and there are several tools on the market that do this.

Hope this helps,

Dominic



## Answer 34912

- posted by: [aaron](https://stackexchange.com/users/-1/15680-aaron) on 2012-01-18
- score: 0

It looks like the TrueLicense project has been revitalized. it's new webpage is http://truelicense.java.net/. I've implemented TrueLicense in a new Swing application I've built. I had to adapt the suggested usage a bit so that I can create license *strings* that users can copy and paste instead of license files.

At least studying this library and reading the documentation will help you understand better how a licensing solution would work.


## Answer 34927

- posted by: [Krzysztof Kowalczyk](https://stackexchange.com/users/-1/3945-krzysztof-kowalczyk) on 2012-01-18
- score: 0

What you want is to maximize your profits.

You need to be aware that implementing any anti-piracy measures degrades the user experience for people who pay you money i.e. generate your profits.

When talking about piracy people usually consider only one aspect: revenue potentially lost to piracy.

You need to consider potential revenue lost because a user was unable to properly unlock your software even after paying you or potential revenue lost due to negative word of mouth (e.g. a paying customer frustrated with your anti-piracy scheme wrote a negative review of your software) or revenue lost because you were spending your time implementing anti-piracy measures when you could have been improving your software.

I'm not saying you shouldn't add anti-piracy measures. I am saying that you should weight all sides of the equation (as opposed to blindly assuming that anti-piracy measure are good for your profits) and if you do implement anti-piracy measures, make sure that they have minimal impact on your paying customers.

As NetTecture said, there is no "effective" solution to piracy. Apple is unable to prevent people from finding a way to jailbreak every version of iOS and you can bet they spend significant resources on that.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
