## URL Logo Question

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-30
- tagged: `website`, `logo`
- score: 2

How do you add a logo so it appears in the URL address box in a browser? For example; Dharmesh has the Hubspot logo appear at www.hubspot.com in the URL address box. Thanks. -Kevin 


## Answer 2820

- posted by: [Del Putnam](https://stackexchange.com/users/-1/671-del-putnam) on 2009-10-30
- score: 9

<p>The quick answer is to just put this in the <code>&lt;head</code>> section of your page:</p>

<pre><code>&lt;link rel="icon" type="image/png" href="icon.png"&gt;
</code></pre>

<p>You can find more specifics here: <a href="http://www.w3.org/2005/10/howto-favicon" rel="nofollow">http://www.w3.org/2005/10/howto-favicon</a></p>

<p>Let me know how it works.  Have fun!</p>



## Answer 2853

- posted by: [Chaoz](https://stackexchange.com/users/-1/1203-chaoz) on 2009-10-30
- score: 3

<p>It's called a <a href="http://en.wikipedia.org/wiki/Favicon" rel="nofollow">favicon</a>, and you should use an ico file for it if you want it to work in all the browsers. </p>

<p>Using anything other than icon files will result in the favicon not working in Internet Explorer!</p>



## Answer 10651

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-27
- score: 0

Yes it's called a favicon.  There are various websites that can help you make one if you already have a logo.  E.g. http://tools.dynamicdrive.com/favicon/

Recommend you have a transparent background on the source file and your favicon.  Onstartups has a white, non-transparent background on their favicon which is not as nice as it could be.  See twitter for a good example of a favicon with a transparent background.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
