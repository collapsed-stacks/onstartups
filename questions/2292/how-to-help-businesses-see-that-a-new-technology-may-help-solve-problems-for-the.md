## How to help businesses see that a new technology may help solve problems for them

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-23
- tagged: `technology`
- score: 2

In my town there appears to be no business using a technology called functional programming. Microsoft is including a new language for this in their next version of Visual Studio.

I am thinking about doing a demo where developers can write applications to try to crash my server using a new FP framework, and also an IIS webserver, so they can see that the IIS one will crash much sooner than the FP one.

My thought is that the developers will then mention to their bosses about this, and if they can hold off on buying new hardware to scale their webservers by just moving to a new framework, it may be justifiable.

My hope is to not convert these websites but to start training developers in this new way of programming.

Does my plan sound like a good approach, to show companies that this new technology may be beneficial?

**Update:** I was trying not to get into the details too much as I thought that may be beyond the scope of this site, but the framework is: [http://liftweb.net/][1]


  [1]: http://liftweb.net/


## Answer 2325

- posted by: [Claus Schwarm](https://stackexchange.com/users/-1/294-claus-schwarm) on 2009-10-24
- score: 2

<p>You idea is quite interesting -- sort of "Show don't tell!" --, but I'd say it won't work. I'm sorry.Hardware is cheap, today. Custom software is not!</p>

<p>Nobody's going to rewrite existing software to save a few thousand dollars on hardware. Thus, the only potential clients are those who start a new project. Unfortunately, they are also unlikely to be interested. This is due to the special <a href="http://www.welton.it/articles/programming%5Flanguage%5Feconomics.html" rel="nofollow">economics of software</a>, in general: The <em>switching costs</em> are high and there are large <em>network effects</em>. The same basically applies to frameworks, too.</p>

<p>Someone considering a new language/framework for a new web site wants answers for some very basic questions:</p>

<ul>
<li><p>Is there <strong>sufficient demand</strong> for the language/framework? This is because a language/framework used by many others is less likely to vanish into obscurity.</p></li>
<li><p>Is there <strong>sufficient supply of programmers</strong> fluent in the language/framework? Without experienced programmers, the existing ones are a scarce resource (and thus expensive). One would need to train others in the language/framework or may be required to rewrite from scratch, someday.</p></li>
<li><p>Is there <strong>sufficient supply of Add-Ons</strong> under an appropriate Open Source license (BSD, MIT, Apache)? Without such add-ons (Forum, Wiki, Issue Tracker, eCommerce, Blogs, etc.), everything needs to be written from scratch.</p></li>
</ul>

<p>To sell a language/framework, in general, you have to prove that these problems are already solved. On top of that, you have to show that is also provides additional benefits -- higher productivity, for example, or less maintenance. Typically, one does so by providing references to case studies, testimonials, words-of-mouth, a large ecosystem, etc.</p>

<p>So, <strong>to answer your headline question</strong>: To show businesses that a new technology helps them solve problems, you point to other businesses who already solved their problems with the new technology.</p>

<p>How do you find the first one?</p>

<p>Simply, in theory: You'd need to establish a beachhead by writing a <a href="http://en.wikipedia.org/wiki/Killer%5Fapplication" rel="nofollow">killer application</a>. Then, you may be able to sell training or support on top.</p>

<p>Hope that helps.</p>



## Answer 2296

- posted by: [RonGa](https://stackexchange.com/users/-1/218-ronga) on 2009-10-23
- score: 1

What is your goal?  Do you want to simply spread the word or do you stand to profit from it somehow?

In order to give you advice, I need to know what your goals are...


## Answer 2949

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2009-11-02
- score: 0

It sounds like you are just trying to have an excuse to use functional programming.  There is no reason for businesses to move to an IMPLEMENTATION of an implementation language just because it is the hot new thing.  

Be careful of silver bullets and snake oil.  Your business targets will be skeptical - and you should be too.  If you start jumping up and down, touting the latest programming fad pretty soon you will be labeled as a kook or a functional programming zealot.  What you really want to be is someone who solves problems.  Learn new things, sure, but don't get caught up in, or, worse yet, promote the hype of things that have little, if any end-user value or meaning.


## Answer 2950

- posted by: [Chaoz](https://stackexchange.com/users/-1/1203-chaoz) on 2009-11-02
- score: 0

Functional programming just isn't used because it is hard to write big applications with it when you're working in teams. Object oriented programming solves this problem a lot better.

There's a particular reason why it's not commonly used. You should use the right tools for the right job, and functional programming is not part of that in my opinion. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
