## How did Magento create an commercial Enterprise version when magento is open source?

- posted by: [Blankman](https://stackexchange.com/users/-1/4860-blankman) on 2010-10-18
- tagged: `software`, `open-source`, `license`
- score: 3

It's interesting how an open source product has a commercial version, nice business strategy to get market penetration!

How did Magento create an commercial Enterprise version when magento is open source?

Don't they have to release the commercial versions source code for free then?


## Answer 15261

- posted by: [Dan Dyer](https://stackexchange.com/users/-1/4221-dan-dyer) on 2010-10-18
- score: 5

<p>The open source version of Magneto is licensed under the <a href="http://www.opensource.org/licenses/osl-3.0.php">Open Software Licence</a>.  I'm not familiar with the OSL but it is a "<a href="http://en.wikipedia.org/wiki/Copyleft">copyleft</a>" licence similar to the <a href="http://www.gnu.org/licenses/gpl.html">GPL</a> (or, <a href="http://en.wikipedia.org/wiki/Open_Software_License#Comparison_with_the_LGPL.2FGPL">according to Wikipedia</a>, more like the <a href="http://www.gnu.org/licenses/lgpl.html">LGPL</a>).</p>

<p>The basic premise behind copyleft licences is that source code should be provided to anybody who receives the software.  However, just because Magneto is released under the OSL, doesn't mean it can't also be released under some other non-open licence.  You or I could not take the open source version and create a closed source fork because we are bound by the terms of the OSL, but the original copyright holders can.  They are free to provide the software to one group under the terms of licence A and to another group under the terms of licence B.  This "dual licensing" is quite common for open source projects.</p>



## Answer 15508

- posted by: [Lena Schimmel](https://stackexchange.com/users/-1/4970-lena-schimmel) on 2010-10-24
- score: 1

<p>There are many software products which use this way of dual licensing. As long as the company wrote all the source code by themselves, they can license it in as many ways as they like. </p>

<p>Things get more complicated when <em>strangers</em> contribute new code to the open source version. This submission is usually exclusively licensed under the open source / copyleft license, so the company is not allowed to use it within their closed source premium version. To use it anyway, they have to either</p>

<ul>
<li>rewrite the new functionality from scratch</li>
<li>pay (or otherwise convince) the contributor to license his code for closed-source usage</li>
<li>recruit the contributor to work for them, improving the closed source version</li>
<li>make the premium version open source / free software (but this is hardly possible while still forcing customers to pay for it)</li>
</ul>

<p>I think the first three options are quite common. I recently read a really good book about it but I forgot the title, and as far as I remember there is no English version of that book available (only German).</p>

<p>EDIT: See this question and it's answers, they pretty much tackle the same problem: <a href="http://answers.onstartups.com/questions/12772/make-my-failed-web-application-open-source" title="Make my failed Web application open source?">Make my failed Web application open source?</a></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
