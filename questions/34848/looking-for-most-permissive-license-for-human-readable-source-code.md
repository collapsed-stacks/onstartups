## Looking for most permissive license for human readable source code

- posted by: [Leo](https://stackexchange.com/users/-1/15540-leo) on 2012-01-16
- tagged: `legal`, `software`, `software-licensing`
- score: 1

Having a web site that may contain source code posted by users, I am in need of a completely obligation free license, and a statement by which users agree code posted by them is allowed to be addressed under such license.

This is the most permissive I have found:
http://creativecommons.org/licenses/by/3.0/

I am looking for one that is free of any conditions, not even attribution.

Can anyone direct me to such a license?

**EDIT:**  The website will contain content contributed by others. My main concern is letting users agree the work they post is free for any use and that they are allowed to post it in such a way (e.g. they are not posting commercially protected code). Does the CC license above state that? Does this protect me from any kind of lawsuit?


## Answer 34680

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-01-11
- score: 2

Instead of trying for a license how about stating that only code in the public domain may be posted? 

Further as part of the signup process have each user agree that they will not post any code that is not in the public domain and that they have full permission to upload whatever code that they do.


## Answer 34862

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2012-01-16
- score: 2

<p>The <a href="http://creativecommons.org/about/cc0" rel="nofollow">CC0 copyright waiver</a> which @Eric Jain linked to is a good choice (be sure to read their FAQ). It's a more 'modern' solution, so it mentions issues like patents. However, the <a href="http://www.opensource.org/licenses/MIT" rel="nofollow">MIT license</a> (@Ask Bjørn Hansen) or <a href="http://www.opensource.org/licenses/BSD-2-Clause" rel="nofollow">2-clause BSD license</a> (@pdjota) are more common, and more well understood by your target audience.</p>

<p>Just using an open-source license will probably <em>not</em> grant you <a href="http://en.wikipedia.org/wiki/Digital_Millennium_Copyright_Act#Title_II%3a_Online_Copyright_Infringement_Liability_Limitation_Act" rel="nofollow">'safe harbor' status under the Digital_Millennium_Copyright_Act</a>. I'm no lawyer, but I would think you will at least need a well made "Terms of Use" document, and a working infringement notification &amp; takedown process.</p>

<p>I'd suggest you start by reading the questions <a href="http://answers.onstartups.com/questions/tagged/terms-and-conditions">tagged terms-and-conditions</a>, and have a look at the <a href="http://answers.onstartups.com/users/1841/dana-shultz">relevant answers from Dana Shultz</a>. And after that, please go see a qualified lawyer specialized in this area of law.</p>



## Answer 34849

- posted by: [mynameisausten](https://stackexchange.com/users/-1/15647-mynameisausten) on 2012-01-16
- score: 1

I think what you are trying to do is a double-negative of sorts; the entire reasoning behind licensing is to give credit where it is deserved. However, if you force the user to sign an agreement (something along the lines of : 'i hereby relinquish all rights to this code') then you wouldn't need a creative commons license. The downside of this is that you would be required to keep all of that data in case of a lawsuit.

So my final suggestion is to just keep the CC license that you have found and, to put it bluntly, just not care if other users don't link back to your page.


## Answer 34851

- posted by: [ejain](https://stackexchange.com/users/-1/15437-ejain) on 2012-01-16
- score: 1

<p><a href="http://creativecommons.org/choose/zero/" rel="nofollow">CC0</a></p>



## Answer 34683

- posted by: [SoftwareCarpenter](https://stackexchange.com/users/-1/15547-softwarecarpenter) on 2012-01-11
- score: 0

<p>I would suggest checking out several different types of collaboration community software sites. Open Source and distribution can be defined differently for what your business model entails. Open source is different then <a href="http://en.wikipedia.org/wiki/Comparison_of_free_software_licenses" rel="nofollow">free software</a>. To ensure you meet either definitions then I would make sure your site meets the licence requirements. Hosting sites like <a href="http://www.codeplex.com" rel="nofollow">Codeplex (Microsoft)</a>, Launchpad.com, and SourceForge.net would be good to check out sense they deal with these issues.</p>



## Answer 34850

- posted by: [pdjota](https://stackexchange.com/users/-1/1355-pdjota) on 2012-01-16
- score: 0

by far the less restrictive licence is Public Domain but it is not so popular.
Commons is not a bad choice for reusing source, remember for instance that all questions and answers in this site are under commons 3.

Nevertheless, I would recommend you to take a look at:
http://www.opensource.org/licenses/category

And IMHO, even if BSD and MIT licence require you to include or reference the disclaimer.

http://www.opensource.org/licenses/MIT

Or ever simpler

http://www.opensource.org/licenses/BSD-3-Clause

These are widely used and accepted licences by different communities of developers and allow you to any type of commercial, non-commercial what-so-ever use.

Hope it helps,


## Answer 34860

- posted by: [Ask Bjørn Hansen](https://stackexchange.com/users/-1/4358-ask-bj-rn-hansen) on 2012-01-16
- score: 0

The MIT license is nice. That being said, maybe what you need is a copyright assignment.  You don't say what your site does.  More details will make it easier to give you a good answer.

Edit: It definitely sounds like what you need is appropriate terms and conditions and/or some sort of contributor agreement.  You are concerned about getting them to state/agree that they are allowed to give you the code, and that they agree to the code being used as your site uses it.  The agreement should explicitly allows your site to re-post what they posted and under what terms (can you re-license it?  Can they remove the content again, what happens then?  etc).  Maybe see what stackoverflow does?  If you want to be more formal about it, then the Apache Software Foundation has a contributor agreement along the lines of what you talk about.

As a side note I didn't think the CC licenses were particularly appropriate for source code.



## Answer 34889

- posted by: [Dmitry Leskov](https://stackexchange.com/users/-1/2093-dmitry-leskov) on 2012-01-17
- score: 0

Check out the <a href="http://unlicense.org/">Unlicense</a>.


## Answer 34898

- posted by: [Coren](https://stackexchange.com/users/-1/15667-coren) on 2012-01-17
- score: 0

<p>The <a href="http://sam.zoy.org/wtfpl/" rel="nofollow">WTFPL license</a> of <a href="http://en.wikipedia.org/wiki/Sam_Hocevar" rel="nofollow">Sam Hocevar</a> is well known in the open source community as probably the most permissive license. But its name can worry your users...</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
