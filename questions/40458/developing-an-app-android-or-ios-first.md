## Developing an app, android or ios first?

- posted by: [mugetsu](https://stackexchange.com/users/-1/14786-mugetsu) on 2012-07-10
- tagged: `apps`, `android`, `apple`
- score: 8

These days most apps support both ios and android. But which one would be the best to get done first? What are the pros and cons of either way? We want to launch a closed beta and get as many users as possible on one of the os.


## Answer 40459

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2012-07-11
- score: 9

The answer is, it depends on your market. 

 - Where are they? In the US or Australia then your more likely to try iOS, China your more likely to go Andoid or Microsoft.
 - Who are they? Designers, then its likely iOS, Business people, more likely Microsoft, general consumer, then possibly Android.
 - How are you going to get paid? from them buying the App, maybe better off with iOS. In app purchases or advertising, then doesn't matter much. Trial ware, Windows has this built into the core. 
 - Are you the first and only? if its a brand new idea then go with an established market place like iOS as its the "showcase" one and people are willing to pay. Android is wild west and traction for paid apps can be harder. If there are competitors already more established then look at the new emerging windows market and maybe become the big fish in the currently small pond before it grows.

For my clients I usually suggest they write it as a website for the first version, unless there are technical limitations or the sales model is app purchase from the store. 

This is because:

- Most apps (except games) don't need to run on the native devices to achieve their goals. If your app doesn't need the phone specific inputs then keep it netural.
- Having it as HTML means they can make changes to the concept very quickly, responding to a market in the early days is a critical success factor.
- Its typically quicker to get the same thing running on several devices quickly.
- Can use google analystics to understand who is actually using their application, and with which devices. Understanding who they are and what they want means you can make more informed choices around the next features to implement.

Once it is established you can then look at native versions because you know who wants it and what they are using. Also you can use some of the bridging technologies to like Linked In have for their iPhone app.




## Answer 40468

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-07-11
- score: 3

Another point - is the app free or paid?  Apple takes a 30% cut of the pay, so that may influence your decision.  Also to consider - can your application be done as an HTML5 app - bypassing all the store / platform specific issues altogether?




## Answer 40579

- posted by: [Darren Cook](https://stackexchange.com/users/-1/14258-darren-cook) on 2012-07-14
- score: 1

<p>This is a hard question, like going to a restaurant and being told you can order food or order drinks, but not both.  So my suggestion is to make an HTML app, then use something like <a href="http://en.wikipedia.org/wiki/PhoneGap" rel="nofollow">PhoneGap</a> to compile it into both a iphone native app and an Android native app (as well as Windows, Blackberry, etc.)</p>

<p>Then if performance becomes an issue, you can optimize into a native app later. (You're talking about a closed beta, so the design will change a lot from that feedback; you don't want to optimize too early.)</p>



## Answer 45157

- posted by: [Anastasiya](https://stackexchange.com/users/-1/21909-anastasiya) on 2012-12-19
- score: 0

The quick answer is that the ROI is usually much higher on iOS apps. Startups/app developers tend to focus initially on one platform to build on. However, to develop a good app with nice looking interface, iOS provides much more, making life easier for developers.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
