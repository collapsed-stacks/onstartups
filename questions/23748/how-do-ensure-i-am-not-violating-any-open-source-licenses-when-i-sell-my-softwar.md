## How do ensure I am not violating any Open Source licenses when I sell my software?

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-04-21
- tagged: `open-source`
- score: 2

I few months back I was talking to friend who works in M&A for a big software company and he was telling me that a large deal just got killed because they realized that part of the code was built out of Open Source pieces that didn't have the licenses required to be sold the way they were. This raised a very big concern that I feel a lot of entrepreneurs don't realize: We need to be extremely careful about the type of licenses Open Source code are distributed under. Some don't allow you to just take it, put it in your code and sell.

It becomes even worth when you use frameworks, that have plugins taken from other Open Sources projects, etc etc.. 

So my question is: How to be sure you are compliant..

What if I code everything using Symfony, or Codeigniter of RoR, stuff like that. What about Javascripts libraries, jQuery, and others? Is there a way, a tool, some kind of solution to this problem? 

I'm not looking for answers about the specific example I gave but generally a general framework (or tool) to make sure that I'm not spending month building a business to realize when it's time to sell it for big bucks that most of it is illegal!

Thank you.


## Answer 23749

- posted by: [ron M.](https://stackexchange.com/users/-1/2122-ron-m) on 2011-04-21
- score: 5

NO magic here. Just the basic good old technique: Make a list of all your software 3rd party dependencies and track down their licenses. Read, understand fully and make sure you're in compliance.


## Answer 23757

- posted by: [Bob Murphy](https://stackexchange.com/users/-1/5778-bob-murphy) on 2011-04-21
- score: 4

Look at the license **before** you start using a software component. If you have any doubts, find another component or write your own.

I've built a lot of software in C or C++ that links with various open-source components, and here's what I do:

 - GPL compilers and so on are okay as standalone executables, but no GPL code gets compiled or linked into proprietary software.
 - LGPL code is only cool for use in proprietary software if it's built into a separate dynamically-linked library. I typically use LGPL libraries that ship with the operating system (e.g. Mac OS X or Ubuntu).
 - Anything that's static-linked needs to have a non-infective license. Examples include the BSD, MIT, zlib, and Boost licenses.

There are probably similar rules of thumb for the languages and technologies you're using. If you're in doubt about a particular component, ask on a relevant mailing list or IRC channel.



## Answer 23750

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-04-21
- score: 0

This sounds a bit silly considering all major software companies especially Apple and Microsoft often use a lot of open source third party software components and technologies in their own OS's.

A good open source licence will let you do whatever you want with the software as long as you properly attribute the open source developer(s). If you have an iPhone, go to settings and then about, you'll notice a lot of attribution for third party open source components in Apple's iOS for example.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
