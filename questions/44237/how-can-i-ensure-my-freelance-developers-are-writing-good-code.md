## How can I ensure my freelance developers are writing good code?

- posted by: [JDH](https://stackexchange.com/users/-1/13136-jdh) on 2012-11-15
- tagged: `webdev`
- score: 1

I'm the one that posted the question, "Do I need a CMS?" Thank you for all the answers, they were very helpful. I decided on going with a framework, codeigniter to be exact, due to its reported ease of use (ultimately I want to learn it, and I only know a tiny bit of php right now). 

Im very active on odesk and know how to hire well, but my concern is now that I am no longer doing this "cheap and dirty" I need to make sure that the code delivered not only works, but is clean, semantic, well structured, etc. 

With my limited knowledge, it will be impossible to know if what I'm getting is quality code or not.

So I have a few questions:

Who can I hire to review the code submitted to me by the freelancer, and what would be a fair hourly rate? 

Does the fact that they are working with a framework essentially force them to write quality code? Or will there still need to be quality control measures as outlined above, or others?

I appreciate any help, I want to make sure i know what I'm doing before moving forward, so thank you for your suggestions and feedback. 

EDIT: Thanks for all the answers. It sounds like a "test plan" is going to be important in this. For anyone interested, here's a great article I found that explains what this is. 

  [Test plan][1]


  [1]: http://www.testing-web-sites.co.uk/2010/05/29/how-to-write-a-test-plan/


## Answer 44282

- posted by: [frisbee](https://stackexchange.com/users/-1/21648-frisbee) on 2012-11-16
- score: 2

I agree with the poster who states that "good quality code" should come 2nd to "working code", but any strategy for sane software development does the following:

Step 1. Provide a SPECIFICATION that states exactly what you want the code to do. Please note that *this is not as simple as it sounds*- you need to list absolutely EVERYTHING that you expect to be able to do with the software. Note that general goals are not good enough here. 
     
As an example, take an online shop. The goal "Sell a tshirt" is useless. Your spec needs something closer to "Upload thumbnail picures, set prices, interface with Paypal, store user's email, put sale icons on top of pictures." This will help your initial developer create exactly what you want with no surprises.  Note that many companies pay someone to do this step for them as well as the next step.

Step 2. You should then pay your independent developer to develop an even longer list of UNIT TESTS from your SPECIFICATION that test multiple cases of each feature. This list is typically called a TEST PLAN. Bonus points (i.e. more value to you) if your independent reviewer can provide you a test suite/piece of software that you can re-run when updates to your site get performed.  

Good luck! (The caps lock words are google search words that may help you find more books on this expansive topic.)


## Answer 44242

- posted by: [Billy Chan](https://stackexchange.com/users/-1/21618-billy-chan) on 2012-11-15
- score: 1

I think the first priority in deliverables should be working software rather than coding quality.

Ensuring working software is not easy. Beyond your manually checking the functionality, the best way is Test Driven Development.

So, if you are going to build something seriously, you need to ask the freelancer to write tests, both unit tests and integration tests.

I believe any developer who can write tests will not produce cheap codes, but not all developers could write tests or be comfortable at it. 

You can check the testing code by yourself or ask a fellow coder to check it. It should take only a few hours since you probably don't need further checking once you know this freelancer could write acceptable tests. I guess the rate for a decent PHP coder who checking it may be $50-$70 per hour.

However, if you are going to build a very simple app you may not need such an overkill.

A side note about the framework. CodeIgniter is light and don't have good support on testing built-in. Yii is better and support test driven development more naturally, and Yii has nicer code base than CodeIgniter in my opinion.




## Answer 44245

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2012-11-15
- score: 1

You're searching for an easy way to do what software engineering professionals have spent decades trying to solve.

Here are a few things you can do:

1.  Follow a good development process with appropriate reviews along the way.  What reviews?  Review any design documentation, functional specifications, architecture document, interface specifications, etc....  You should have somebody else looking at the code being produced by every developer.  (If they're pair programming, then you may already have this.)

2.  Come up with a testing strategy -- you ought to have regression testing, to make sure that your coders don't break anything along the way.  You also need to systematically test new functionality.  And, you need somebody to consider the security of the software.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
