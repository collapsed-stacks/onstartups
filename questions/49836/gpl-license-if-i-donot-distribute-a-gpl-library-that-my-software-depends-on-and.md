## GPL License: If I donot distribute a GPL library that my software depends on and have the user download externally, do I have to use GPL

- posted by: [Somesh Mukherjee](https://stackexchange.com/users/-1/16623-somesh-mukherjee) on 2013-07-10
- tagged: `software-licensing`
- score: 3

I am stuck between a few choices for my turnkey Project management system: a library that uses GPL and an inferior library that is under MIT license. 

I am wondering if I don't distribute the library with my software and require the user to download it externally, do I still have to release under GPL? 

And on those lines, if I add a downloader that the user can run to satisfy dependencies(download the library), is it a violation of GPL. 

I am making proprietary software and would really like to earn money for it. 

I am not looking for exact legal advice, but I am sure this is a common use case. 



## Answer 49843

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2013-07-10
- score: 2

<p>Please see my answer to this question which you might find helpful too:</p>

<p><a href="http://answers.onstartups.com/questions/49759/ownership-issue-of-open-source-project-when-moving-to-vc-funding/49768#49768">Ownership Issue of Open Source project when moving to VC funding</a></p>

<p>In your case if you modify the GPL lib you have to put these changes under GPL too. 
See: <a href="http://www.gnu.org/licenses/gpl-faq.html#TheGPLSaysModifiedVersions" rel="nofollow">http://www.gnu.org/licenses/gpl-faq.html#TheGPLSaysModifiedVersions</a></p>

<p>Still you can charge money for it:
<a href="http://www.gnu.org/licenses/gpl-faq.html#DoesTheGPLAllowMoney" rel="nofollow">http://www.gnu.org/licenses/gpl-faq.html#DoesTheGPLAllowMoney</a></p>

<p>If you just prelink your software, it does not count as modification:
<a href="http://www.gnu.org/licenses/gpl-faq.html#Prelinking" rel="nofollow">http://www.gnu.org/licenses/gpl-faq.html#Prelinking</a></p>

<p>I don't know what exactly you are doing. But the "download it yourself" pattern might not help you but it is an indicator that you might be safe. Please read through the linked FAQ above and consult your local lawyer on this matter. There cannot be a general advise without knowing how your software exactly relates to the GPL'ed one.</p>

<p>The website GPL Violations also maintains a nice little <a href="http://gpl-violations.org/faq/vendor-faq.html" rel="nofollow">FAQ</a> on this topic.</p>

<p>That all said it should basically be easy for you too include the GPL'ed source code in your distribution along with your proprietary binaries (assuming you software doesn't need to be GPL'ed).</p>



## Answer 49849

- posted by: [David](https://stackexchange.com/users/-1/5460-david) on 2013-07-11
- score: 2

If you ask users to download the library separately and you include no other GPL components, then no, you would not have to distribute your the rest of your code under the GPL. Using the method calls of the API doesn't bind you to the license, only use of the actual code.

That said, you do still need to distribute your software under a license that is compatible with the GPL. Otherwise, when the user puts everything together and uses it they will be in breach of the GPL on that component.

This has been tried a number of times historically and virtually always kills the project, users won't jump through hoops like this.

Edit: One thing to add is with the GPL there are the legals and there are the ethics. The intention of the GPL is perfectly obviously and the author of that library is stating their intention by using it. My personal view is that trying to work around the intention using a legal loophole is unethical. I would never buy such software, I wouldn't allow such a tactic to be used in my own company and I wouldn't deal with another company that does such a thing. You might buy in some extra functionality in the short term, but the ethics of the decision might also come back and bite you. 


## Answer 49895

- posted by: [Krzysztof Kowalczyk](https://stackexchange.com/users/-1/3945-krzysztof-kowalczyk) on 2013-07-16
- score: 2

**This would be illegal!**

**Both previous answers are wrong** (I only scream because it's important).

The fact that you ask your users to download the GPL library your program **needs** to work is irrelevant. I understand why people are tempted to creatively work around GPL license, but it's still illegal.

If your code depends on non-trivial piece of GPL code, even if it is packaged as a library and you ask users to manually download it, your app is still a derivative of that GPL code and therefore you're bound to GPL license.

In fact, LGPL license exists precisely to address this case: an LGPL'ed library can be used by non-LGPL code. If you use library under LGPL, you only have to open-source the changes (if any) to that LGPL library. If you use GPL library, you have to open-source everything.

Think of it this way: it's trivial to convert any piece of GPL code into a library and build your proprietary code on top of that. This trivial trick would nullify the GPL. People are not doing that not because you're the first one to come up with this clever work around but because it's not a work around.

What you want to do would be as illegal as if you distributed the GPLed library yourself.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
