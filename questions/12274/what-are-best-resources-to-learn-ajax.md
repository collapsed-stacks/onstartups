## What are best resources to learn AJAX?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-06-22
- tagged: `web`
- score: 0

What are best resources to learn AJAX in detail?


## Answer 12278

- posted by: [Mike Lee](https://stackexchange.com/users/-1/3589-mike-lee) on 2010-06-22
- score: 1

<p>I agree with Ricardo, StackOverflow might be a better place for this question.</p>

<p>AJAX stands for <a href="http://en.wikipedia.org/wiki/Ajax_%28programming%29" rel="nofollow">Asynchronous JavaScript and XML</a> and is generally written in <a href="http://en.wikipedia.org/wiki/JavaScript" rel="nofollow">JavaScript</a>. It primarily utilizes the XMLHttpRequest object within the DOM. To learn how to use this object and build AJAX functionality, however, you'll first need to learn JavaScript.</p>

<p>O'Reilly's books are a fantastic resource. Here are some books that will help, in order of most basic to most advanced:</p>

<ol>
<li><a href="http://oreilly.com/catalog/9780596521875/" rel="nofollow">Learning JavaScript</a></li>
<li><a href="http://oreilly.com/catalog/9780596101992/" rel="nofollow">JavaScript: The Definitive Guide</a></li>
<li><a href="http://oreilly.com/catalog/9780596517748/" rel="nofollow">JavaScript: The Good Parts</a></li>
<li><a href="http://oreilly.com/catalog/9780596528386/" rel="nofollow">AJAX: The Definitive Guide</a></li>
</ol>

<p>If you prefer to learn from videos, Douglas Crockford has a bunch that are hosted on the <a href="http://developer.yahoo.com/yui/theater/" rel="nofollow">YUI Theater site</a>. Just look for all of his videos (unfortunately, there's no way to filter the videos to display just his).</p>

<p>The definitive blog on all topics AJAX is <a href="http://ajaxian.com/" rel="nofollow">Ajaxian</a>, where you can find many examples of cool uses of AJAX.</p>

<p>There are lots of <a href="http://www.google.com/search?q=xmlhttprequest+cross+platform" rel="nofollow">cross-browser &amp; cross-platform issues</a> with the XMLHttpRequest object, however. Therefore, many developers use cross-platform JavaScript libraries to easily get around this. Some popular libraries are:</p>

<ul>
<li><a href="http://jquery.com/" rel="nofollow">jQuery</a></li>
<li><a href="http://script.aculo.us/" rel="nofollow">Script.aculo.us</a></li>
<li><a href="http://developer.yahoo.com/yui/" rel="nofollow">YUI</a></li>
<li>And there are many, many more</li>
</ul>

<p>To tie this back to startups &amp; business, you can look at AJAX with this kind of business benefit:</p>

<p>AJAX allows you to create websites that act like desktop applications on a web browser. When you click on a button, you don't need to wait for the entire page to reload. Just a small piece of it can change. Gmail and Google Maps are perhaps the best examples of good uses of AJAX. This means perceived &amp; actual improved download times, improved usability, and improved functionality. This leads to greater user enjoyment, lower user frustration, and thus, hopefully, greater user retention.</p>

<p>Hope this helps.</p>



## Answer 12276

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-06-22
- score: 0

First of all... I think you should post this question in a different site... http://stackoverflow.com perhaps? However, since I am already here and I have a fair answer to your question here it goes. 

Look at the following sites for resources, guides and examples on how to use AJAX:

http://jquery.com/

http://tekpub.com/production/jquery This site charges $25 for the webcast but it is well worth the money. I've used this before and was very happy with the quality and the content.

http://www.w3schools.com/ajax/default.asp

Good luck!


## Answer 12328

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-06-23
- score: 0

<p>IMHO, The best way to learn is hands on.  </p>

<p>There is a great little web "series", creating a web app from scratch which steps you through the... umm.. steps necessary to build an application.  Ajax is part of it.</p>

<p>Here's the <a href="http://css-tricks.com/examples/WebAppFromScratch/" rel="nofollow">link</a>.</p>

<p>Ajax, like other technologies, is best understood in the context of a actual application - many times people just tack on the functionality for a "gee whiz" eye candy.  A good example of the benefits of ajax in a ecommerce environment is a one page checkout process.  (<a href="http://demo.onestepcheckout.com/products/19-widescreen-flat-panel-lcd-monitor.html" rel="nofollow">demo site</a> - add an item to the cart and press checkout) As you change the options, you get immediate feedback on any price / delivery changes.  Makes the checkout process a non-threatening process.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
