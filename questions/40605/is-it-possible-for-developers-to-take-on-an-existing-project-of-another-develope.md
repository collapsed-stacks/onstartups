## Is it possible for developers to take on an existing project of another developer(s) or programmer(s)?

- posted by: [Wanda Pebbs](https://stackexchange.com/users/-1/18806-wanda-pebbs) on 2012-07-16
- tagged: `webapp`, `webservices`, `webdev`, `developers`
- score: 2

Wondering if it's possible to hire a new set of developers to take on an existing project not completed by previous developers? Some complained it may be difficult to understand the codes developed by the incumbents and as sort, would prefer to start afresh.

Opinions are welcomed.


## Answer 40607

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-07-16
- score: 7

<p>Yes, it is possible. If it is difficult depends on the work others have done. IF it is code and follows the <a href="http://rads.stackoverflow.com/amzn/click/0132350882">"Clean Code" principles</a> aswell as using standard frameworks then it should  easy to take over the code.</p>

<p>If the previous programmers did not respect general coding conventions or use exotic frameworks, it might become difficult. </p>

<p>Personally I would never do a "fresh start" before investigating the codebase. Some programmers prefer "fresh starts" only because they are used to other frameworks or different styles (or languages). </p>

<p>If have worked on development projects for years (I mean, one project going on for years). The project team changed much since I joined. I was not the first one on the project and not the last one. Still it was possible to take over the project.</p>

<p>After all when a codebase grows it becomes more difficult and difficult to get into. But the risk to develop it newly is not to underestimate. Nobody can guarantee you it becomes actually better.</p>

<p>therefore I would look at the old code:</p>

<ul>
<li>did the previous developers use standard frameworks (for example Zend Framework, jQuery, Wicket etc)</li>
<li>did the previous developers use tools to verify standard quality (code style tools like Checkstyle, or other tools like Findbugs)</li>
<li>did the previous devs create Unittests (phpunit, Junit etc) and how much do the test cover the code (40% is not acceptable, >85% is very good)</li>
<li>is the code documented (Java/PHPDoc, additional documents</li>
</ul>

<p>Then look at the new devs.</p>

<ul>
<li>have they experience with the same tools, languages etc?</li>
<li>do they follow clean code standards?</li>
<li>are they willing to write docs?</li>
</ul>

<p>Ask them, why exactly they want a fresh start. There is a learning curve when adapting old software, but this cannot be the exact reaons. It must be something like circular dependencies, multithreading issues, exotic and not maintainable frameworks etc.</p>

<p>Only if I knew this I would decide if it is better to start over again. Remember, it is your money and they need to tell you why you should pay for the same work twice.</p>



## Answer 40609

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2012-07-16
- score: 5

I've worked on projects where there was an existing codebase - and sometimes I had to start over from scratch, but usually not. If possible, I prefer to use the existing codebase unless there is a really good reason not to.

A competent programmer, or team of programmers, should be able to inherit code and build on it. This should be the preferred approach, as it reduces the number of errors re-introduced (after all, the existing codebase had some testing done on it) and avoids completely redoing the work of others.

That being said, on occasion, the existing code will be of such poor quality (whether this is because it is poorly written, poorly documented, or written in some esoteric framework or language) that a redo will be required. 

If the new team is suggesting a redo - be sure to get other opinions to ensure that this is not a form of laziness on the part of the new developers to avoid learning the existing code.


## Answer 40606

- posted by: [user999629](https://stackexchange.com/users/-1/18807-user999629) on 2012-07-16
- score: 1

Yes is posible.

The learning curve for them can be large or small depending on the previous team.

If a programmer already saw the codebase and said it is best to start fresh, keep that in mind, and ask others the same.


I would recommend to start fresh if the project allows, and use a open source framework to keep consistency over the project.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
