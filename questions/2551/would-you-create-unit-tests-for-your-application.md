## Would you create unit tests for your application?

- posted by: [jpartogi](https://stackexchange.com/users/-1/911-jpartogi) on 2009-10-27
- tagged: `development`, `testing`
- score: 3

I don't know about you, while I agree that unit testing can reduce defects and therefore can maximize ROI in the long run, but it just takes an amount of time. Knowing that you're a startup where time matters and it costs you every dollar, would you write a unit test?

What are the pro and cons writing a unit test based on your personal experience besides the reasons that I talked about? Do you even care about writing unit test in your startup?

**EDIT**:

I'm asking here because I'm asking from business point of view, not technical point of view. If I ask at SO, the response that I get will be of course mostly from technical point of view.


## Answer 2582

- posted by: [RonGa](https://stackexchange.com/users/-1/218-ronga) on 2009-10-27
- score: 4

QA is crucial for more then just ROI.  If your product doesn't work, your customers will not buy it.  If it causes them hard (delete their info, waste their time or anything else) they will actively tell people not to use your product, or worst.

The last thing you want is to be associated with a product that didn't meet quality standards.  Unit testing, stress testing and other tests are crucial.


## Answer 2552

- posted by: [Paul McMillan](https://stackexchange.com/users/-1/1126-paul-mcmillan) on 2009-10-27
- score: 3

Ask this on stackoverflow.

That said, yes, we unit test. Not because it catches all bugs, or because it prevents us from introducing regressions, but because it speeds up testing here and now. Whenever we're running a test on new code, we find that we need to test it, tweak it, and then re-test it. Writing that as a unit test very rapidly saves time over re-doing the same set of steps repeatedly after each change.


## Answer 2553

- posted by: [DThrasher](https://stackexchange.com/users/-1/326-dthrasher) on 2009-10-27
- score: 2

I'm a complete believer in unit testing. It took me a while to get the hang of it, but once I got past the learning curve, it saved me far more time than it cost.

The main benefits for me were:

 1. It helped us improve the design of the code by forcing us to decouple components. This came in handy later when we needed to swap out certain modules or cut features prior to launch.
 2. It gives us confidence that we're not breaking existing functionality as we roll out new features and fixes.
 3. It gave us a great platform to test individual features or components without having to worry about the interactions with the rest of the system.

The major drawback, apart from the initial learning curve, is that it takes experience to know what parts of the system *can* and *should* be unit tested. For example, a web API should be thoroughly tested, but most user interfaces change too rapidly to make the effort worthwhile.


## Answer 2554

- posted by: [Gabriel Hurley](https://stackexchange.com/users/-1/1005-gabriel-hurley) on 2009-10-27
- score: 2

Absolutely!

(*not only will it prove to you things work now, but when you make changes in the future, it'll prove that things **still** work*)

(*I've written many apps, both with and without unit tests*)


## Answer 2586

- posted by: [Winfield](https://stackexchange.com/users/-1/1020-winfield) on 2009-10-27
- score: 2

Automated testing is essential for a software startup.  You are wasting time and money if you forego rigorous unit and functional testing.

 1. Writing Unit Tests helps you write software more quickly.  It will allow you to catch bugs earlier, prove functionality, and document usage. 

 2. Software Startups usually cannot afford QA or have minimal QA staffing.  The only way to maintain quality without massive manual efforts is automated unit and functional tests.

 3. Startups involve constant change.  Without adequate test coverage you will be UNABLE to commit a major refactoring/change or be significantly slowed at the very least.

In the first two years of our startup I have seen all three of these theoretical arguments validated.  We have maintained high quality through 30+ software releases without ever hiring QA.  We have fundamentally refactored core financial systems in a single development iterations and gotten it right, due to automated test coverage.  

I can not argue strongly enough in favor of unit/functional testing from day 0.


## Answer 2555

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-27
- score: 1

It depends on your end goal. If you want to get it out quickly, before the competition, then whatever doesn't help you with that hurts you.

If you want to design for maintenance now then unit test.

If you are in the very early stages and your design is changing a great deal, then unit testing can be a pain, as you will constantly be changing tests just because you are madly making interface changes.

But, ultimately, by the time you have it out of beta you should be unit testing, as you are now going into a maintenance phase, and this will help ensure that your code is in better shape.

I am in the early stages, haven't even fully settled on a language yet, so no unit testing. :)


## Answer 2564

- posted by: [Chris](https://stackexchange.com/users/-1/923-chris) on 2009-10-27
- score: 0

Unit testing helps demonstrate that your application is doing what you intend. Wouldn't you, and/or your team of coders, like that peace of mind before giving the app to the world? Personal experience tells me that if you don't unit testing from the get-go your application will eventually reach a point where you think you need it. And unit testing as an afterthought is more difficult than doing it as part of your development process from the start. Sure, it's time consuming, but at least you'll know your app works and that its design is solid (another benefit: writing tests makes you think about your design/APIs). Hopefully the up-front cost of unit testing will save you time later when your startup has to worry more about the business end of things. 


## Answer 2571

- posted by: [danpickett](https://stackexchange.com/users/-1/13-danpickett) on 2009-10-27
- score: 0

I'd recommend incorporating Test Driven Development (TDD) into your practices. I think it's well suited for a startup environment. You don't have time to backtrack and handle regressions. You need something automated to help protect you against it.

What's more and what I haven't seen mentioned here, is TDD can actually benefit your architecture greatly. If you're focusing on smaller problems and incrementally advancing your business logic, your code will be more clear and concise. Otherwise, I've found over engineering happens.

I'm a big believer in the promises of Agile Development methodologies, and Test Driven Development is a cornerstone practice. It's a great way to get started in incremental development, and really helps you release early and often.


## Answer 2576

- posted by: [CoderDennis](https://stackexchange.com/users/-1/517-coderdennis) on 2009-10-27
- score: 0

This might be an insignificant grammatical point, but no, I would not write a unit test for my app.

I would write unit tests to test individual units of code as part of the development process.

The tests for the whole app are integration tests and/or QA tests. There is a significant difference even though they are all called "tests."



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
