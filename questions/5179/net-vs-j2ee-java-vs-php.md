## .NET vs J2EE/JAVA vs PHP

- posted by: [sthomps](https://stackexchange.com/users/-1/1962-sthomps) on 2009-12-16
- tagged: `software`
- score: 4

We are currently building a new social networking platform, and I was wondering everyone's opinion was on what base to build it on. I know this is an age-old debate between .NET and PHP, just wondering what people believe is the best to build.  (speed, scalability)

Thanks in advance


## Answer 5185

- posted by: [skillguru](https://stackexchange.com/users/-1/742-skillguru) on 2009-12-16
- score: 3

<p>If you are a programmer, I would suggest go with a language you are comfortable with. I am a programmer and stared with my product. Some people suggested to go with Ruby on rails, others said php etc etc
The idea is to develop your product at earliest , launch it , validate your business idea and then move forward. If your product succeeds then you can can always come back and fine tune it.
The advantage with language like Java, .NET and php is that you can find lot of programmers. Some more advice can be found here</p>

<p><a href="http://www.geekevaluation.com/blog/2009/04/18/tools-for-a-startup-part-1/" rel="nofollow">Tools for startup</a></p>

<p>I used java, Spring hibernate with php</p>



## Answer 5182

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-12-16
- score: 1

What requirements do you have?  What external libraries or functionality do you want to use?

Which OS are you running on, WinXP?

What are you familiar with, how strong are you in these three languages?

Personally I would look at going to Scala, using LIFT, as it runs on the JVM, but, if you don't have anything done yet, then you may want to start with PHP, so you can get something done quickly, and at least have an alpha version up, so you can show potential investors.

Once you know what features you want then you can redo it in a cleaner fashion in .NET or Java, depending on your answers to the questions above.

By going to .NET, if you worry about speed or scalability in parts then you could write those parts in F# and get some improvement, for example, but Scala will compile both CLR and java bytecodes so it can work on either platform, so scalability is less of a concern, if you can design in multi-paradigmic systems (I think that may be a new word, may need to be spelled 'paradimic').

If PHP meets your needs and you can scale it well, then you can continue to use it as your front-end and just look at making changes to the backend.

My point is that all three are used in large websites, so any of them will work well, the correct answer will be based on your answers above. 

 For example, if you need Comet, so you can have socket connections that stay open for a long time, then PHP will have a problem, then you are using .NET MVC if .NET can do it at all, otherwise you are looking at some other language.


## Answer 5191

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2009-12-16
- score: 1

See here: 

http://answers.onstartups.com/questions/831/how-to-pick-a-platform-for-a-startup-web-2-0-app

All those answers will help you.


## Answer 5200

- posted by: [espinet](https://stackexchange.com/users/-1/1892-espinet) on 2009-12-17
- score: 1

For a quick rapid prototype to get proof of concept, as a software engineering student I'd recommend Ruby on Rails. It so much time consuming work for you saving you hours and hours doing stuff you need to do else where. Rails also has a lot of "Gems" which add extra functionality to your software with very little effort. Something like Facebook's auto-complete in their search bar. 

Once your application takes off, your profitable, and Ruby is no longer fast enough then you could translate some of subsystems to a much faster language. You can leave those decisions for later.

Summary:<br />
Build your application quickly and easily in Ruby on Rails<br />
See if theirs a market or if you have a quality product people want to use.<br />
Get a large userbase and become profitable.<br />
Move subsystems to a faster language if required.<br />

Matt

P.S. This is exactly what Twitter has done.


## Answer 5212

- posted by: [Raymond Giorgi](https://stackexchange.com/users/-1/1960-raymond-giorgi) on 2009-12-17
- score: 1

I can't answer on .NET vs J2EE, since the differences between the two are pretty marginal and asking which is better is usually the same as asking, "What's your preference"?

However, it's been my experience that PHP is not great at scaling in terms of programming, and, as the old adage goes, hardware is cheaper than your engineer's time.

A couple years ago, I worked on maintaining an existing PHP inventory application, and even the slightest change often times meant spending hours combing through a combination of code and HTML trying to find an ending curly brace. Of course, I had to edit the deployed application remotely using emacs, but that's another story entirely.

For small applications, though, J2EE and .NET can really be overkill. In Java, a lot of time needs to be spent configuring and tuning Hibernate, struts-config, etc, so simple CRUD applications are usually done best in PHP.

One very important thing to keep in mind, though, is that both .NET and Java are also meant to be used to implement desktop applications, which is great because you have access to third party packages, system info, etc. from within your web application.


## Answer 5220

- posted by: [skillguru](https://stackexchange.com/users/-1/742-skillguru) on 2009-12-17
- score: 1

<p>I am a j2EE programmer and prefer Java+Spring+Hibernate on tomcat server. I was not a big fan of php but every since I started used wordpress and its plugins , I have become a big fan. If you look at  my site <a href="http://www.skill-guru.com" rel="nofollow">Skill-guru</a></p>

<p>, it is a combination java and php.
I did most of part in java and integrated wordpress for blogging and then integrated a third party forum , jforum.
I managed to pull wordpress posts into java application by connecting two databases.</p>

<p>The best of part of php is that is search engine friendly. </p>

<p>So I am having best of both worlds. Our blog consists of lots of articles and information of how we are doing all this stuff.</p>

<p>But remember do not try to code everything. Jot down requirements and then try to integrate existing applications and componenets</p>



## Answer 5246

- posted by: [Jagath Narayan - Ordoro](https://stackexchange.com/users/-1/1975-jagath-narayan-ordoro) on 2009-12-18
- score: 1

Don't look at just the technical pros and cons of the language, also look at the programmer culture associated with that language. 

In my experience, the J2EE folks are very "enterprise-ey". Very process oriented / methodical. Where as the Python / Ruby folks are more dynamic, flexible, improvisational kind. I guess it has to do with the nature of the languages and the availability of toolkits.

Neither style is right or wrong, be aware that there are different styles and consider the one you are comfortable with.


## Answer 5221

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-17
- score: 0

I would not use one of them. I have PHP experience, a little bit of Java and I started few projects with Ruby.

PHP is easy to use but is quite traditional and limited. Symfony is the only decent franework, Zend Framework is too low level, thus not productive. 

J2EE is the most reliable especially for financial application, and Spring + Hibernate is a bullet proof solution. It is very unproductive and tiring because you have to fight against the compiler instead to using a more BDD process.

.NET is a direct contender of Java, a bit more modern, but is Microsoft, so if you do not want to throw away your money I would not use it. There is the option to use C# on Mono, but I would use Java on Linux instead a not so popular and not 100% compatible alternative.

I would use Ruby or Groovy. Groovy runs on top of Java, Spring and Hibernate (a quite layered solution !!!). Ruby's environment is quite similar to PHP, is an advanced language and has Rails, at the moment the most productive and feature complete solution for web development. With one book, 'Agile Web Developemnt with Rails', you can use a state of the art solution, which is quick, good quality and is very used for Web 2.0 startups. Grails is similar to Rails but is developed with Groovy.

I choosed Ruby + Rails. 


## Answer 5258

- posted by: [Dan](https://stackexchange.com/users/-1/1600-dan) on 2009-12-18
- score: 0

Although I don't know your requirements (as another poster pointed out), I would at least consider Google App Engine, the Python edition, that's probably Django, maybe Pylons.

The biggest advantage is zero sysadmin. No configuring boxes, deploy by clicking a button.  It also scales, but that's a rarer problem.

The biggest downside is that it is preview release and has limitations. However, that may not be a big downside if what you are trying to do is rapidly find market fit.


## Answer 5456

- posted by: [Abdu](https://stackexchange.com/users/-1/2029-abdu) on 2009-12-23
- score: 0

I don't think PHP is scalable enough. The choice of language doesn't matter much. Use whatever you are comfortable with. If you are going to hire local programmers, look at their rates. I think Java/J2EE is the most expensive and it might be hard to find good Java developers.

Also you might want to start with an open source project instead of starting from scratch so whatever language/technology that project is using, that would be your criteria.


## Answer 6200

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2010-01-08
- score: 0

This is more of a religious issue rather than a business one.  Go with what your developers are most comfortable with.


## Answer 6203

- posted by: [Scott Drake](https://stackexchange.com/users/-1/2199-scott-drake) on 2010-01-08
- score: 0

Find talented developers and let them tell you what they would like to use. Talented = experienced building apps with challenges similar to yours that were successfully completed and launched, and preferably lived with for a few years. Make sure that it's easy to find other talented developers in whatever languages/technology stack they recommend because they likely won't be around in a year. In my local market, there's a ton more .Net developers than J2EE. In other markets J2EE is more common. Almost any language/platform can be used to build a successful app if the right talent is working on it. So focus on finding the right talent from the largest available pool in your market, not on the technology.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
