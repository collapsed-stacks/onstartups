## Advice for conducting a pilot

- posted by: [DThrasher](https://stackexchange.com/users/-1/326-dthrasher) on 2009-10-21
- tagged: `software`
- score: 1

I have a chance to conduct an on-site pilot of my desktop software. How should I prepare for the pilot? What factors should I consider? What are the best practices for conducting a pilot?



## Answer 2110

- posted by: [Rob Allen](https://stackexchange.com/users/-1/604-rob-allen) on 2009-10-21
- score: 2

<p>In your pilot, are you testing for usability or just looking for system bugs? If you including usability, there is a lot to consider. More formal information is available in <a href="http://en.wikipedia.org/wiki/Software%5Ftesting" rel="nofollow">this</a> Wikipedia, but here are a few points off the top of my head: </p>

<ol>
<li>How many testers will you have? If this is the first of many test sessions you do not want more than 5 - 10 people according to <a href="http://en.wikipedia.org/wiki/Jakob%5FNielsen%5F%28usability%5Fconsultant%29" rel="nofollow">Jacob Neilsen</a>.</li>
<li>What tasks are you looking to test? Make sure you have a script/task list for testers to follow which closely mirrors what the end-users will be doing on a daily basis, otherwise you will not get useful feedback. </li>
<li>How are you going to monitor the software usage? There are <a href="http://danalytics.blogspot.com/2007/07/usability-testing-techsmith-morae.html" rel="nofollow">many</a> <a href="http://silverbackapp.com/" rel="nofollow">usability</a> testing software packages for tracking keystrokes, clicks, etc. which also pair with a screen mounted web cam that syncs the video feed with the key/click log. This is great for usability testing. If you want to have people just walk around and ask questions, you will need to train them first. There are also companies/consultants which specialize in this sort of thing, a Google search should bring up a few in your area. </li>
<li>Consider the physical environment your testers will be in? It should be comfortable and relatively free of distractions. </li>
<li>Who from your team will be present at the test? </li>
<li>What level of guidance over and above the task list will you provide? </li>
<li>When bugs are encountered, how will you be logging them? </li>
</ol>

<p>Despite the URL pointing to a US Government site, <a href="http://www.usability.gov/refine/learnusa.html" rel="nofollow">this page</a> also has relevant usability testing background information.</p>



## Answer 2115

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2009-10-21
- score: 2

Rob makes some excellent points. Pilots can be tricky. The best advise I ever got on conducting pilots (or any kind of comparison experiment) was to do a Design of Experiment (DOE).

DOE is pretty formal and uses statistics to compare different treatments. For your pilot (experiment), you probably don't need all the fancy math. What you do need is to answer these questions:

 1. Define the present state. This goes a long way in figuring out what you might effect.
 2. Define the desired state, with your solution. This has to be quantifiable. Things like: Saving X amount of minutes, reducing defects or whatever. Get agreement on what success is.
 3. Define metrics to measure.
 4. Baseline the present state and confirm the measured metrics.
 5. Apply the treatment and measure them metrics.
 6. Analyze the results
 7. Repeat as necessary with different treatments or measurements.

This is clearly a shorter list than the whole method but is a good snapshot of how to go about proving that your solution adds value. There may be debate over what are "hard" savings as opposed to "soft" savings. Get those discussions done up front and drive toward the definition of success that everyone agrees with.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
