## How do you use web data with heuristics to group customers

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-11-04
- tagged: `marketing`, `internet`, `statistics`
- score: 0

I've read a few blogs on identifying a customer type from how they get onto your page.  I'm not familar with these techniques but the implications I find intriguing and would like to incorporate onto my websites.  So would love to hear of tools and techniques.

Thank you


## Answer 16044

- posted by: [Samik](https://stackexchange.com/users/-1/3353-samik) on 2010-11-04
- score: 1

<p>Using <a href="http://www.google.com/analytics/" rel="nofollow">Google Analytics</a> you can go a lot of distance in this. How do you use it is based on your experience with the tool. I am listing pretty basic ones here:</p>

<ul>
<li>Use the network property in the user section of it to get what was the speed, connection type.</li>
<li>Use the map overlay to know where are they coming from</li>
<li>User browser capabilities can point which browser is used by your users etc.</li>
<li>New vs returning visitor is also indicative enough.</li>
</ul>

<p>Hope this helps.</p>

<p>Cheers,</p>

<p>Samik</p>



## Answer 16083

- posted by: [Alan Ma](https://stackexchange.com/users/-1/5217-alan-ma) on 2010-11-05
- score: 1

AFAIK, creating different campaign and using different landing pages/content for these campaign is probably one of the best way to achieve what you described. GA does help, but you can always write some scripts to analyze your own dataset. You can even take GA data into Excel and slice/dice it. HTH.


## Answer 16106

- posted by: [Janis Peisenieks](https://stackexchange.com/users/-1/5241-janis-peisenieks) on 2010-11-05
- score: 1

I would approach it this way. 

 - Create/Download a script that creates a database of sites, that users come to you from.
 - Group them up. You could try Googling them, Alexa, etc. , but what you need to look for is the type of website is it. What type of customers does it provide you with, and what can you do once you know what kind of customers come from there. Can you sell a particular product to them, are they more prone to buy one thing, and less on another and so forth.
 - Create/download a script that searches your database, matches the type and acts on the commands. This script would check, if it knows what to do with a a user from a particular website, and if clear, what does the site need to do/display to make that sales.

There are more to it, and you could possibly use some API's to do some automation for you.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
