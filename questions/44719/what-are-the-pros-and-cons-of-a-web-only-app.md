## What are the pros and cons of a web-only app?

- posted by: [Richard](https://stackexchange.com/users/-1/17832-richard) on 2012-12-03
- tagged: `development`, `apps`, `rss`
- score: 3

I've developed a web-based RSS reader and it seems the next logical step would be to create apps for the various mobile platforms (iOS, Android, etc.). But I have no idea where to begin and I would have no way of testing my apps. (I don't own any mobile phone/tablet and I don't want to buy an array of devices just to test one app.) I've heard there are ways to create a mobile app once and then port it to various devices, but that route seems to require some usability tradeoffs.

I'm thinking it would be it would just make more sense to build a mobile-friendly version of my rss reader that has a sleek "app" feel to it. But if it's that easy, why do so many sites even bother with the time and expense of creating a native app?

I literally haven't spent more than five minutes using a smartphone in my lifetime. (No, I'm not a luddite, I just have no need for a mobile device. Also I am Canadian, and the telcos here charge exorbitant rates I'd rather not pay.)


## Answer 44734

- posted by: [Billy Chan](https://stackexchange.com/users/-1/21618-billy-chan) on 2012-12-04
- score: 3

*Disclaimer: I'm experienced at web but shallow on mobile apps*

After reading the question body, I think the question title would better be: Mobile site VS Native App - cost and benefit

*I use "site" here to refer to your web app that lives on server but not client device.*

There are two ways to build a HTML5 mobile site:

1. Responsive Design
    + Basic: Use CSS/JS to make the site fitting mobile screen
    + Work: You need to shrink some functions/displays in server side by detecting mobile, because mobile device can't handle too much elements on screen.
    + Use case: Good for simple and regular site such as blog, not good for sophisticated web app like yours.

2. Mobile version
    + Basic: Use JavaScript frameworks such as Sencha and jQuery Mobile to build another site in mobile. Detect mobile and redirect them to mobile version.
    + Work: Full rebuilding. You can hardly utilize any of your previous work on client side, especially JavaScript.
    + Pros: Full mobile compatible. Easy to use on mobile. 
    + Cons: Lower performance comparing with native app. Similar workload.

There is also hybrid method like PhoneGap. Basically it is to package your mobile version and release a mobile app. The performance is still lower than native app.

Native apps excel on performance and user experience, that's not something mobile version sites can compare with. Even Facebook admitted that they made a mistake on sticking with HTML5 instead of going native: http://highscalability.com/blog/2012/9/15/4-reasons-facebook-dumped-html5-and-went-native.html

My suggestions:

+ Continue to optimize your web app for web. **Make sure your API is good enough for future native app usage**
+ Make responsive design for tablets, add some support if possible, such as touch, under current JS framework.
+ Go native when you have resource.


## Answer 44723

- posted by: [Ulflander](https://stackexchange.com/users/-1/21874-ulflander) on 2012-12-03
- score: 2

Here is (a very little) list:

Pros:

- Use advanced features available only using native apis 
- Better integration on the device
- Usable offline (with cached RSS feeds for example)
- Better performances


Cons:

- Far more expensive
- Far more work
- User experience to reproduce carefully in order to be coherent between all apps, but user experience have to be coherent with the device OS too in order for people to quickly understand the UI
- Have to be approved by app stores policies
- Have to be downloaded and installed




## Answer 44722

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-12-03
- score: 0

<blockquote>
  <p>Why do so many bother to do a native app?</p>
</blockquote>

<p>Because they require access to hardware specific features unavailable to the HTML5 Crowd.  Used to be that you could not create a native feeling app in HTML5- its not easy to do, but there are some good examples that with certain applications it is possible. <strong>Example</strong>: a good writeup on the development of the <a href="http://justinvincent.com/page/2043/anatomy-of-a-native-feeling-html5-ios-app" rel="nofollow">splitsville IOS html5 app</a>. </p>



## Answer 44724

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2012-12-03
- score: 0

To add to the list of pros of having a native app: More exposure. Some people discover new apps solely by browsing featured app lists on their mobile devices.


## Answer 45109

- posted by: [Anastasiya](https://stackexchange.com/users/-1/21909-anastasiya) on 2012-12-18
- score: 0

Some more pros of having a native app: it gets full support from application stores and marketplaces. Users can easily find and download the apps they need. Also native apps have to get an approval, the user can be assured of complete safety and security of the app. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
