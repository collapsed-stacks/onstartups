## Strengths and Weakness of Split or A/B testing

- posted by: [blunders](https://stackexchange.com/users/-1/4764-blunders) on 2012-01-14
- tagged: `ab-testing`
- score: 2

Listening to a trendy popular book which appears to be pushing A/B split testing pretty hard without covering the weaknesses or barriers to get returns from it.

Are the any good resource for understanding the strengths and weakness of split or A/B testing?

(Mainly recall the sample size required to get valid results AND that the out come only produces one decision, not a chain of decisions; meaning using A/B testing for every choice is just not a good idea based on the volume required and related cost.)


## Answer 34811

- posted by: [Matt](https://stackexchange.com/users/-1/8784-matt) on 2012-01-14
- score: 4

<p>The real problem with split testing is the great power it gives you to focus on the tiny details.  You'd better be sure you're in the right forest first though before you start thinking of trees and individual leaves on those trees.  Because you do get actual, measurable improvement it can reinforce and encourage you focussing on the <strong>wrong problem</strong>.  Just because it is <em>measurable</em> does not make it <em>meaningful</em>.</p>

<p>Which of several AdWords ads convert best - simple and clear-cut, right?  What if your ad writer is not as good as you think - you could perhaps have bumped click-through by far more by hiring someone entirely different.  Are you going to split test ad copy writers?</p>

<p>Similarly when multivariate testing on your site, you need to be sure that your options are meaningful in terms of copy, design, usability etc.  If the design doesn't convert well in the first place, what's the point messing about with colour or layout option a, b and c?</p>

<p>Sample size and distribution:  You really need to be running the test for over a week - Monday traffic is not often the same as Sunday.  If you have a seasonal business March might not obey the same rules as August.  You also need to be getting enough hits to each variation to be statistically worthwhile - for a new site that could be near impossible.</p>

<ul>
<li>Does the small variation in conversion mean anything at all in the context of the hits you have?</li>
<li>Would the same test three months later give entirely different results due to having a seasonal profile and your visitors are now peak season as opposed to off-season three months back?</li>
</ul>

<p>...and what if you a/b test the old site with the new?  Is it meaningful - is it the inevitable resistance to change, or uncertainty with finding things in the new design that's causing the differential, or is it actual and real problems with the new with respect to the old?  At what point can you be sure?  <em>Really</em>?</p>

<p>Are you <em>actually</em> going to scrap your $xx,xxx site redesign if the split test says so, or are you going to fiddle with the details whilst basically remaining committed to the junk that is the "improved" design?</p>

<p>Ok, there's been plenty of instances of terrible redesigns out on the web, but let me give you just two.  (I've no idea if either of these split tested at all)</p>

<p><a href="http://lifehacker.com" rel="nofollow">http://lifehacker.com</a>: Months after the redesign I still hate their new active layout.  It's still harder to find things than it ever used to be, it's still inconsistent, and it still returns search results in the tiny right-hand column which is not the one with the scroll bar.  Result?  I visit <em>only</em> when I get handed a link that interests via someone else.  No amount of split or multivariate testing is going to resolve core, broken usability.</p>

<p><a href="http://trustedreviews.com" rel="nofollow">http://trustedreviews.com</a>: I visited very regularly, as aside from trusting the content the design was <em>fast</em> and <em>light</em>, displaying a summary that enabled you to rapidly scan for new updates.  Redesign based on WordPress.  Result?  (Ignoring the sea of orange) Horribly slow comparative load times, no longer possible to take in what used to be on the homepage without multiple clicks and slow page loads.  Some useful things the old site did simply can't be done any more.  Many other minor usability issues.  They can A/B the life out of it now and a good chunk of their old user base will never notice as they're now on different sites.  I've not visited for months.</p>

<p>Split test those <em>meaningfully</em>.</p>

<p>Don't get me wrong, Google Website Optimizer is a great tool, but it's one of the very last to be used.  The last layer of polish, used when something needs <em>polishing</em>.</p>

<p>Google split test a lot - and they never get their new layouts and designs wrong, do they? <a href="http://stopdesign.com/archive/2009/03/20/goodbye-google.html" rel="nofollow">Obligatory link to the Google 41 shades of blue testing story</a>.  The rollover pulldown menu Google now have in place of the discrete black bar with all links seems like a big leap backwards to me usability wise, but I've no doubt the A/B testing makes me "wrong".</p>

<p><a href="http://www.codinghorror.com/blog/2010/07/groundhog-day-or-the-problem-with-ab-testing.html" rel="nofollow">Here, have Jeff Atwood's take on it</a>.</p>



## Answer 34817

- posted by: [WooHoo](https://stackexchange.com/users/-1/14202-woohoo) on 2012-01-14
- score: 4

From my personal experience it's important to know why you are doing an a/b test.  So in the past we have asked testers to go through the signup process and list the barriers to signing up. 

So if a barrier was say too much information on a page, we would reduce the information and a/b test.  

So my suggestion is don't do a/b testing on hunches or what you think may work more effectively, take the time to learn what potential customers think. 

This may sound obvious but always test the actual conversion rate, so if you change a landing page, and ten percent more people click through that doesn't mean you will get ten percent more conversions.  We have had a case where we a/b tested two landing pages, much more people clicked through on the new landing page.  But actual conversions dropped by eight percent on the new landing page.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
