## MySQL and PostgreSQL licence issue

- posted by: [Josh Morrison](https://stackexchange.com/users/-1/12044-josh-morrison) on 2011-07-18
- tagged: `open-source`, `license`
- score: -1

Our company wants to use [MySQL][2] for one software product, and our product is not open-source. Is it legal to use it freely?

If not, how about [PostgreSQL][1]? Is this okay for our purpose?

  [1]: http://en.wikipedia.org/wiki/PostgreSQL
  [2]: http://en.wikipedia.org/wiki/MySQL




## Answer 27636

- posted by: [Andreas Arnold](https://stackexchange.com/users/-1/5361-andreas-arnold) on 2011-07-18
- score: 3

<p>Do you want to distribute the product? If yes, do you want to bundle MySQL? Then the GPL isn't too clear about that point. Is it now statically linking or not? I guess no one really knows the answer to that.</p>

<p>If, however, you don't bundle it with your product and the user has to download it themselves, you should be fine, even with the <a href="http://en.wikipedia.org/wiki/GNU_General_Public_License" rel="nofollow">GPL</a>, since you are not distributing a GPL product.</p>

<p>If your product is a web application, so you aren't distributing any code at all, then you are fine. There is actually a special version of the GPL, <a href="http://en.wikipedia.org/wiki/Affero_General_Public_License" rel="nofollow">Affero GPL</a> (AGPL), which closes that loophole. With the AGPL you have to distribute any modification made to a AGPL product, even if you aren't technically distributing your product.</p>

<p>If you want to be totally safe, use PostgreSQL, since PostgreSQL is licensed under the <a href="http://www.opensource.org/licenses/postgresql" rel="nofollow" title="PostgreSQL License">PostgreSQL License</a> (which is a <a href="http://en.wikipedia.org/wiki/BSD_licenses" rel="nofollow">BSD</a>/<a href="http://en.wikipedia.org/wiki/MIT_License" rel="nofollow">MIT</a> style license), and you should be fine.</p>

<p>But to be really safe, ask a lawyer and let him decide.</p>



## Answer 27631

- posted by: [Filippo Diotalevi](https://stackexchange.com/users/-1/4482-filippo-diotalevi) on 2011-07-18
- score: 2

At this point, I think it's difficult to provide you with a "sure answer".

It used to be common understanding that you cannot distribute a product containing GPL software without GPL-licensing the product itself.

In recent years, I have seen so many interpretations and counter-interpretations (what's distribution? is there a difference between statically-dynamically linked libraries?) that I cannot honestly give a general answer anymore. Many of these discussion are also summarised at http://en.wikipedia.org/wiki/GNU_General_Public_License

Ideology aside, it is my opinion that the GPL license is one of the worst licenses ever written. It's verbose, ambiguos, with a ridiculous "ideological" preamble.
The central concept of distribution is never defined in the license, leaving the reader with many question (is distribution when a contractor create the software for his customer? Is it distribution when ACME Germany gives the software to ACME Italy? Is it distribution when the Bank IT Dept install a software in all Bank's branches?)

All in all, I think the only safe option to use GPL software (and MySql) is to use it for in house projects. That's, by the way, the common use case of MySql. If you want to package it and sell it to customers as part of a bigger project, you'll easily get into trouble.

Note that all this discussion does not apply to PostgreSQL. PostgreSQL is licensed under a BSD/MIT-type license, and therefore can be used, modified and distributed without any license issue.







## Answer 27640

- posted by: [Marcin](https://stackexchange.com/users/-1/8798-marcin) on 2011-07-18
- score: 1

If you can't answer this yourself by understanding the licences, you need a lawyer.

Did you even try to read the licences in question?


## Answer 27646

- posted by: [Jack Rodenhi](https://stackexchange.com/users/-1/1839-jack-rodenhi) on 2011-07-18
- score: 0

If these answers are not satisfying, you might take a look at the Firebird Database.  Its license is explained in the Firebird Wikipedia entry:

> The Firebird database engine and its modules are released under an
> open-source license, the Initial Developer's Public License (IDPL), a
> variant of the Mozilla Public License (MPL). It does not force the
> developer to open the products using Firebird or even
> custom-derivatives made from its source code; but if the developer
> chooses to do so, then some terms and conditions should be honored.
> The IDPL gives the developer the freedom of making propietary, closed
> source applications that use Firebird or are based on it

So far as capabilities go, the database is transaction driven, includes Views, Stored Procedures and Triggers, is very SQL 92 compliant, can be run in a client server mode or embedded and is apparently handling some databases in the wild with sizes of 50 to 100 GB.  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
