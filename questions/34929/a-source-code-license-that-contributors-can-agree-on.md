## A source code license that contributors can agree on

- posted by: [Leo](https://stackexchange.com/users/-1/15540-leo) on 2012-01-18
- tagged: `legal`, `software`, `software-licensing`
- score: 2

This question is related to [a previous one I've asked]( http://answers.onstartups.com/questions/34848/looking-for-most-permissive-license-for-human-readable-source-code), but this aspect felt broad enough to deserve its own space.

I have a web site where others contribute code and I am in need of an open source license that accomplishes 2 goals:

1. Conveys to viewers of the site that all source code they see is free for any use.
2. Informs contributors (whose code is going to be used by viewers) that by submitting code they agree that (A) the code they post will be free to use, that (B) they cannot break any rules by posting it, and that (C) the site itself cannot be held liable for code posted in violation of (A) & (B)

Let's say goal 1 is accomplished by something like the [Creative Commons BY license 3.0](http://creativecommons.org/licenses/by/3.0/). However, in reading through the license, I am not sure it accomplishes goal 2. 

 - Is this an effective license given the two goals above? 
 - If not, what additional licenses are appropriate here?


## Answer 34975

- posted by: [Andrew Bradford](https://stackexchange.com/users/-1/15710-andrew-bradford) on 2012-01-19
- score: 2

<p>To accomplish goal 1, that code is available for any use for free, you can use any number of open source / free licenses such as the BSD or MIT license.  Usually these are called "academic" licenses since most are named for academic institutions.  Generally they allow anyone to do just about anything with the code, so long as attribution is provided when required.  Source does not usually have to be provided along with binaries.</p>

<p>To accomplish goal 2, you should really look into contributor license agreements or contributor copyright assignments.  The Apache Foundation has a nice <a href="http://www.apache.org/licenses/icla.txt" rel="nofollow">contributor agreement</a>.  The FSF has a nice contributor <a href="http://git.savannah.gnu.org/cgit/gnulib.git/tree/doc/Copyright/assign.changes.manual" rel="nofollow">copyright assignment</a>.  You could also look into the Apache license, which has clauses giving rights to the project for any contributed code and having all contributors, by contributing, state that they are able to do so.</p>

<p>I'm not a lawyer.  I suggest you read Intellectual Property and Open Source by Van Lindberg and talk with a real lawyer to make sure you're doing things correctly, even if you utilize a system used by another successful project.</p>

<p>Sorry that I'm not able to provide more links, my account does not have enough reputation to post more than 2 links.  You should be able to Google for the Apache, BSD, and MIT licenses and find the Van Lindberg book easily at many libraries or at various book stores.</p>



## Answer 34949

- posted by: [Dana Shultz](https://stackexchange.com/users/-1/1841-dana-shultz) on 2012-01-18
- score: 1

<p>Even for goal 1, the Attribution license to which you linked is not ideal, in that, as the name suggests, it requires attribution.</p>

<p>I believe that the Creative Commons CC0 <a href="http://creativecommons.org/publicdomain/zero/1.0/" rel="nofollow">Public Domain Dedication</a> (which was mentioned in two of the answers to your other Q) can come close to achieving both of your objectives. As concerns copyright, all rights are waived, so users can do whatever they want.</p>

<p>CC0 is limited in that it does not address other rights (such as patents and trademarks), but those are likely to be minor considerations in your situation.</p>

<p>In summary, I believe that you need, fundamentally, a waiver of rights rather than a license.</p>

<p>(As concerns not "break[ing] any rules" in posting content, countless websites have this type of provision that you can use as a starting point.)</p>

<p>Disclaimer: This information does not constitute legal advice and does not establish an attorney-client relationship.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
