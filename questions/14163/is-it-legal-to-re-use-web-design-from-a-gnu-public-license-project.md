## Is it legal to re-use web design from a GNU public license project?

- posted by: [UnStartup](https://stackexchange.com/users/-1/2189-unstartup) on 2010-09-21
- tagged: `legal`, `website`
- score: 2

I found a web design layout that I like, and it is from a GNU GENERAL PUBLIC LICENSE open source project.

Will I run into any legal issues here?

I know I should talk to a lawyer, but just curious as to others feedback on this.


## Answer 14165

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-09-21
- score: 1

<p>Disclaimer: I'm not a lawyer, and this is not qualified legal advice. Use at your own risk.</p>

<p>Your first step is to figure out which license the <em>website itself</em> is under. It may be different from the software; or there may be no explicit license for the website (HTML, CSS, JS etc) itself.</p>

<p><strong>If</strong> the website is licensed under the GPL version <strong>2</strong>, then you can freely use the design, HTML, CSS and Javascript on your own site. <strong>But</strong> you must:</p>

<ul>
<li>Make a version of your (modified) website codebase available for download free of charge.</li>
<li>Display the GPL version 2 license on your site, so that people can see that the site is licensed under the GPL 2.</li>
<li>You <strong>must not</strong> run website code and your own application code in the same memory space (i.e. on the same PHP application server). If you do, your own application must also be GPL 2 licensed.</li>
</ul>

<p>Nota bene: The above is valid if <em>static or dynamic linking</em> is the <a href="http://en.wikipedia.org/wiki/GNU_General_Public_License#Linking_and_derived_works" rel="nofollow">criteria for determining whether your own code is <strong>a derived work</strong> or not. Opinions differ.</a></p>

<p>If the codebase is licensed under the GPL version <strong>3</strong>, the terms are stricter and your own code will be more likely to also fall under the GPL version 3. See this nice <a href="http://www.groklaw.net/articlebasic.php?story=20060118155841115" rel="nofollow">overview of the GPL version 2 and 3</a>.</p>

<p><strong>My personal advice: Either stay away from GPL licensed software, or pay the original author for a copy of the work under another, closed-source license.</strong> The original author can always license the work to you under another license, and in fact many will do so for a modest payment. Using GPL code for commercial uses is tricky; it's IMHO easier to either keep away from GPL code or obtain it under a <a href="http://en.wikipedia.org/wiki/BSD_and_GPL_licensing#Copyleft" rel="nofollow">non-copyleft</a> license.</p>



## Answer 14164

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-09-21
- score: 0

Website design and copy is copyrighted, which is separate from the licensing stuff of the software in question.

So no, you cannot steal it.

However if you ask they might very well say "Sure, take it!"  So I'd ask!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
