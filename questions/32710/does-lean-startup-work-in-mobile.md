## Does Lean startup work in Mobile?

- posted by: [RonGa](https://stackexchange.com/users/-1/218-ronga) on 2011-11-17
- tagged: `strategy`, `lean`, `mobile-apps`
- score: 6

I started reading into the lean start-up method, and it makes a lot of sense that this is the way to start a company.  The thing is, can this method work with a mobile app, where it can take a while for apps to get approved?  Its not like a website that you can update 50 times a day and do split testing by running different versions on different servers...

What do you guys think?  Has anyone tried it here?  Did it work?


## Answer 33023

- posted by: [roman](https://stackexchange.com/users/-1/14667-roman) on 2011-11-26
- score: 7

My answer is "Yes" as well. This is really a problem with Apple where you've got only 100 beta testers.

Don't forget that Lean Startup is not just about testing several versions of the product - but is a kind of ideology which you could apply in your startup.

Your first step should be an MVP (minimum viable product) which should get you some testers. You don't have to test on 100 people to know what works and what doesn't. Installing great analytics should give you great insight into what your users are doing.

The idea of a web based solution is not bad. Though the speed is not as native, the feel can be almost identical. The little differences shouldn't matter too much if your product is awesome. If it's really great - you will see it immediately.

Using the HTML5 approach will allow you testing with unlimited number of users with the feel of a native app.

Many startups use A/B testing with just mockups without a real product - you could try that one as well. Just to get the initial feedback.

Lean startup doesn't state that you should have the PERFECT product to test it. Just an MVP version of it. Web solution is good enough.

BTW, Lean startup is also a state of mind - just keep it lean with all your expenses and efforts ;)


## Answer 32820

- posted by: [Sum](https://stackexchange.com/users/-1/14557-sum) on 2011-11-21
- score: 4

<p><strong>YES, It can</strong></p>

<p>The principles of the Lean Startup can most definitely be applied. You can launch a MVP quickly and iterate from there. (Sure it might take a week or two extra to go live, but that's part of the game) </p>

<p>When you run a beta, it truly is a beta. Users will have to give you their UUID's and you'll have to install software but software like <a href="https://testflightapp.com/" rel="nofollow">TestFlight</a> makes this a lot easier to do. </p>

<p>You can iterate 50 times a day, with your own development devices and see which ones you like. </p>

<p>It's harder to apply, but it will work. (And remember, you don't need to follow the principles like its a holy text. You just need to embrace the concepts behind them) </p>



## Answer 33162

- posted by: [aoporto](https://stackexchange.com/users/-1/11579-aoporto) on 2011-11-30
- score: 3

Eric Ries does a great job in his book of showing through case studies how the Lean Startup approach has worked in various industries and established companies.  The key is to stick to the fundamentals: MVP, smaller batches, testable hypotheses, etc. Considering that many lean methods come from manufacturing (e.g. Toyota), this is definitely not just for the web.  The web certainly makes it easier to test and deploy, which is why it is so powerful a technology, while the App approval process makes this more challenging. I'm going through the same hurdles with my App development, but I will follow the fundamentals plus the excellent advice already given here to use lean within the constraints of a curated app store model. Feel free to contact me in the future if you want to compare notes on what has worked. 


## Answer 38194

- posted by: [Andrej Kostresevic](https://stackexchange.com/users/-1/17504-andrej-kostresevic) on 2012-04-14
- score: 1

It definitely does, although there are some challenges that are not present with web products.

- approval times for iPhone
- users have to agree to upgrade to the new version
- versioning between server-side and client-side features

That said, do not forget that the issues described above affect the speed of iteration in what is not necessarily the first stage of a lean startup. They do not affect your ability to talk to your potential customers and conduct problem interviews or solution interviews. They do not affect your ability to research the market, examine the volumes of google searches or conduct smoke tests using ad words and/or simple landing pages. They do not prevent you from conducting a concierge MVP, where you offer a manual service to a small number of people to prove your value hypothesis.

Lean is a mindset - "how can i test my assumptions with the least amount of effort possible." Sometimes the answer involves writing apps or adding features to your existing apps. A lot of the times it does not.

For the cases where your MVP is best conducted by developing an actual app, there are things you can do to work around the issues presented by the mobile platforms. 

Others already mentioned distributing your app to a small number of testers without going through the app store. For Android, this is a non-issue - you can email your app to as many people as you wish without submitting to the Market (I'll never get used to saying Play).

A/B testing is not easy on mobile, but it is possible. Switching features out in response to data sent to server is another way to experiment without versioning your app. 

And finally, the mother of all approaches: using hybrid HTML5 and native apps which offer you the best of both worlds: the ability to be in the app stores and leverage native functionality when needed, as well as the ability to introduce new functionality, A/B test or switch your features on the fly, by just changing your server-side code.



## Answer 41312

- posted by: [Emirikol](https://stackexchange.com/users/-1/19227-emirikol) on 2012-08-13
- score: 1

with a Native app development - **only using data driven split testing**.  
with wrapped html - yes.  

the Lean Startup's main claim is that the startup's product is **validated** learning, all the additional tools - an MVP, interviews and the 5 whys are additions to the core methodology of conducting experiments. thinking lean yet *proving* nothing does not give you the vaunted advantage of not developing features that users don't want.  
Certainly you can do a non-mobile solution at he beginning such as a a concierge MVP but that does not answer your question. After you passed that point and created an application you still need to learn.

**Option I - using beta testers**  
the limit of 100 testers makes this option irrelevent.

there are few things as dangerous as false knowledge - thinking that you've proved something when you still don't know the answer.   
to gain knowledge using the scientific method you need a controlled experiment with a representative sample giving you a statistically significant result. 
based on http://www.surveysystem.com/sscalc.htm (my knowledge in statistics is rusty)
with 100 testers you can get a 95% certainty that your results have any meaning for a total amount of users of 135 or less. got more than that? then your tests are practically meaningless.

**Option II - plain normal update cycle**  
here what you have is a long iteration cycle, instead of deploying 50 times a day you're deploying once every few months. that's how long you have to wait before you get the results of experiments. and worse, since you want to know what is the specific effect of each change - that's one feature per 1+ month.  
only one change each month for your developers to develop.  
only one lesson learned each month.  
if there is any truth in the lean startup's premise then you are guranteed to be pulverized by faster iterating competition.

**Option III - data driven split testing**  
in this method, you code many split tests in one version, the application decides which functionality to execute according to data from the server. the server is responsible for assigning your users to one experiment each and making sure a control group exists.  
though your iteration is long you can conduct many experiments in paralell this way, which is actually what a web based solution does anyway since most experiments should track long-term consequences and not just immediate results.




## Answer 44517

- posted by: [Dirk de Kok](https://stackexchange.com/users/-1/21778-dirk-de-kok) on 2012-11-26
- score: 1

I agree, lean startup is a state of mind of constantly coming up with hypotheses, experiments, validation and learning. Some thoughts on lean startup for mobile:

 - Your launch is a really important moment for your app success. Make sure you have a pretty   decent app at least, and not a minimal rough MVP.
 - Mockup testing helps with getting feedback, HTML basic app is even better.
 - There are A/B testing tools for native mobile like SwitchBoard and Clutch.io nowadays.

More can be found in my blogpost [here](http://blog.mobtest.com/2012/11/applying-lean-startup-to-mobile).



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
