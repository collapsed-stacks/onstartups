## Facebook Connect versus Facebook app?

- posted by: [Dan](https://stackexchange.com/users/-1/1600-dan) on 2009-11-20
- tagged: `facebook`
- score: 4

Is it more useful to have a Facebook canvas app than simply having Facebook connect on your own site?  Why?

As far as I can see, either one let's you get approximately the same thing into a Facebook user's stream, which is the only visible part to me.



## Answer 3910

- posted by: [danpickett](https://stackexchange.com/users/-1/13-danpickett) on 2009-11-20
- score: 3

Having developed both, I can say that developing a Facebook connect application gives you more control. If you don't need to show information on people's profiles (boxes) and you really just want to publish feed items - FB Connect is a simple solution. You can do other cool things like see what friends you have on FB are using your application, etc. It's a great way to see the effectiveness of FB marketing on your application as well. The number of FB Connected users is generally a good indicator of conversion from Facebook related materials.

Going with a canvas app does increase project risk, in my opinion. The platform is fairly young, and FB often changes things without prejudice. FB Connect is still subject to this risk, but I think it's less significant, and they generally seem to be a bit more caring when it comes to making changes on that side of things.

Oh, and use the JavaScript api instead of their FBML if you can help it - the markup it generates isn't standards compliant and can mess rendering up a bit.






## Answer 3923

- posted by: [Joe A](https://stackexchange.com/users/-1/60-joe-a) on 2009-11-21
- score: 1

<p>I pondered this question myself at the beginning of the project I'm working on, and chose to go with Facebook Connect for my main site, but also develop a canvas app as a "lite" version. The reason were:</p>

<ol>
<li><p>I was able to maintain autonomy with my site as far as UI and flow while still benefitting from using Facebook's powerful platform features. I can drive traffic to my fully featured Connect site using a smaller canvas version that exposes 1 or 2 features.</p></li>
<li><p>I would eventually like to consume competiting authentication providers, APIs, etc and not tie myself to Facebook. In 3 years time there could be a mass exodus of FB like we are seeing with MySpace now.</p></li>
<li><p>Facebook itself is <a href="http://news.cnet.com/8301-19882%5F3-10323364-250.html?tag=newsLatestHeadlinesArea.0" rel="nofollow">promoting Connect over canvas applications</a>. Furthermore, by going Connect I can further insulate myself from risk that another FB platform change can break my app.</p></li>
</ol>



## Answer 3900

- posted by: [CoderDennis](https://stackexchange.com/users/-1/517-coderdennis) on 2009-11-20
- score: 0

I think it's about how you want visitors to enter your site/app.

Are the visitors already on your site? Use Connect.

Are the visitors coming from Facebook? Use a canvas app.

You could build both interfaces and share the business logic between them.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
