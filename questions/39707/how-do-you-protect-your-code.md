## How do you protect your code?

- posted by: [hiro](https://stackexchange.com/users/-1/18273-hiro) on 2012-06-05
- tagged: `code`
- score: 2

For a startup, the product is the most important asset, but it seems that in many/most startups (I know), the <b>complete code base</b> is shared among every member of the team. Even complete database access is shared, too.

I know that accessing the complete code base may make the process easier and faster, but it's very dangerous and unprofessional because, in a startup, employees come and go so often. And you are the one who fire them.  

I assume that most startup doesn't want to get involved in any kinds of lawsuits, which take unnecessary time and money. Thus, protection beforehand is much better.

How could you deal with this situation? What's your method of protecting your code base?


## Answer 39716

- posted by: [futureal](https://stackexchange.com/users/-1/18012-futureal) on 2012-06-06
- score: 3

<p>The main differences between development at a startup and at any other enterprise are that at a startup, you are more likely to have fewer developers, rapid releases, scattered code and deployments, and overall, more chaos.</p>

<p>However, in a modern software company -- startup or otherwise -- it is unrealistic to expect that your employees won't have access to your codebase. Even if you attempt to partition the code based on access rights to repositories, your developers are likely to intermix and re-deploy your code as it suits their productivity.</p>

<p>There are some basic best practices you should follow, some of which it sounds like you already are:</p>

<ul>
<li><p>Store your code in an enterprise-ready source management tool, and make sure each person who has access rights has their own account. If possible, use a solution that can log check-outs in addition to check-ins. As stated, this will not really prevent people from copying your code around, but it is a good first line of defense.</p></li>
<li><p>Restrict access to your source repository to your VPN if you have one, or if not, see if you can configure it in such a way that nobody in the outside world can "see" your server. Again, this does not guarantee anything, but minimizes the risk of unauthorized accesses to your repository, and discourages employees from doing things like checking out code at home.</p></li>
<li><p>Minimize the number of deployments to necessary systems. Too often, a startup moves rapidly enough that pieces of code get strewn all over servers in development environments, temporary servers, and so on. Often times developers will be deploying things themselves to test configurations, and nobody ever cleans things up. Just because it is a startup doesn't mean you shouldn't strive to have a clean set of environments with a minimal number of code deployments. Make sure that when developers deploy code, they are doing it only to systems that you own or maintain.</p></li>
<li><p>Restrict access to non-production environments to your VPN if you are able. Restrict access to product environments to as few people as possible. Restrict access to actual production data to the fewest number of people possible. None of these will necessarily protect your code, but in many cases, the only thing worse than giving up your code is giving up your (customer) data, for privacy and other reasons.</p></li>
</ul>

<p><strong>Now, with all of that said, always assume that your code has and will leave the building. Whether innocently or maliciously, once you have employees, your precious software will be out in the wild somewhere. If you are lucky, nothing will ever come of it, but if you are unlucky, somebody may either (a) use it to develop a competing product, or (b) attempt to claim copyright.</strong></p>

<p>Although there is a cost involved, if you see true value in the proprietary nature of the software you are developing or planning to develop, you need to retain legal services and make sure that at a bare minimum:</p>

<ul>
<li><p>Every in-house developer has signed an employment agreement that specifies the work they do for you as <a href="http://en.wikipedia.org/wiki/Work_for_hire" rel="nofollow">work for hire</a>. This is not always straightforward but best practices do exist and they hold up pretty well in court.</p></li>
<li><p>Every external developer or development firm has signed a contract prior to any work being completed that clearly specifies the design requirements, and clearly identifies your company as the owner of any resulting software. There can be a lot of gray areas in third party work, especially when requirements are loosely given, and copyright of the resulting software can often be claimed by the third party after the fact.</p></li>
<li><p>Every developer, internal or external, has signed some form of a no-compete agreement in your area. Generally speaking, these are not very enforceable in court. However, just by having it, it will often discourage developers from attempting to do things like steal and repurpose code or ideas, and it certainly won't hurt you.</p></li>
<li><p>Finally, that copyright notices, licenses, and so forth are all correctly inserted into your code and checked in to your repository, and logged, so that you have a pristine legal record of the creation and ownership of your software. If you do need to challenge somebody on the ownership of <em>your</em> code down the line, you will want a timestamped record of your claim of ownership. </p></li>
</ul>

<p>Although there are best practices for some of these, the law around software is <em>constantly</em> evolving, and many gray areas do exist. There is no substitute for real legal counsel on these matters, and if you are serious about protecting proprietary software inventions, you need to have somebody audit everything and make sure you are on track.</p>

<p>These issues are ones that every software company faces, regardless of size. My final advice is, don't get bogged down worrying about all of these details, but do spend as much time as you feel is necessary given your investment in the software. If, as you say, the entire value of your company is in the software product, then you stand to lose a lot if somebody attacks the code. Were it me in that situation, I would immediately seek legal counsel and look for next steps in securing your investment in your product.</p>



## Answer 39709

- posted by: [webbie](https://stackexchange.com/users/-1/16413-webbie) on 2012-06-05
- score: 1

Does your code need to be protected - is it the "secret sauce" of your product? Unless your code is your competitive advantage, I wouldn't worry about others walking away with some knowledge of it, unless you deal with ecommerce and customer data, especially personally identifiable information (PII is email, name, dob, etc).

Basics: All programmers should have their own accounts for your code repo, no sharing. If you have sensitive data, have separate accounts to manage that data with only your most senior developers using those accounts. Have people running DB reports use read-only accounts, ideally with limited access to tables they run reports on.


## Answer 39717

- posted by: [nathan](https://stackexchange.com/users/-1/17082-nathan) on 2012-06-06
- score: 1

Everyone so far has given great advice, but protecting the code isn't as important as protecting the client list is. if I had Microsoft's Windows 8 code, it really wouldn't mean much as I don't have the resources to monetize it.  

Source code isnt the product unless you are literally selling source code. Everything is the product, from the app to the customer support, the public face, the problem that it solves for the customer, etc, etc, etc.

ex: having Stack Exchange's source code means nothing because you don't have Stack Exchange's customers. That isn't to say this isn't necessarily a bad problem to solve, just that there are more pressing and urgent matters.


## Answer 39711

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2012-06-06
- score: 0

Webbie has good practical advice.  I'd add "Keep journals of access to the code."  That way, if a version of it shows up in the wild, you may be able to track it back to when it was pulled from the repository.  Some repositories will also add a watermark.   Also:

*  Get a good non-disclosure agreement in place
*  Make sure you own the code, either as a work made for hire or an outright copyright assignment.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
