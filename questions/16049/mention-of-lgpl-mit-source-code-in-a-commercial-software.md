## Mention of LGPL/MIT source code in a commercial software

- posted by: [Tom](https://stackexchange.com/users/-1/5227-tom) on 2010-11-04
- tagged: `software`, `license`
- score: 1

My commercial software is using some code source licensed under LGPL or MIT.
How and where should I mention this?
Is it mandatory?


## Answer 16050

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-11-04
- score: 2

Follow the license of use.   


## Answer 16060

- posted by: [HedgeMage](https://stackexchange.com/users/-1/5198-hedgemage) on 2010-11-04
- score: 1

I don't know the terms of the MIT license by heart, so you'll have to read it.

With regard to the LGPL: is the LGPL work you are using (hereafter referred to as "foo") a library or something else?  Is the work based on foo (hereafter referred to as "bar") a derivative of foo, a work that uses foo, or are you unsure (in which case provide more info on bar)?

Generally, if foo is a library, and bar uses foo as an external dependency rather than compiling whole chunks of foo into bar, bar is a work that uses foo, and you have no particular responsibilities under the LGPL.

If you foo is a library, and bar is a modification or derivative of foo, or foo (or significant portions of foo) are compiled into bar to make it count as a derivative, the LGPL applies and you must provide the proper notices, access to the source code, etc.  In this case you may at your option relicense bar under the GPL instead of the LGPL if doing so makes more sense to you.

There are a bunch of other cases, but those are the two most common.

IANAL*, but I run an open-source based development shop, so I deal with this stuff daily.

--Susan


*I Am Not A Lawyer: in other words, don't take my word for it, that's what lawyers are for.


## Answer 16061

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-11-04
- score: 1

<p>EDIT</p>

<p>Based on  your <a href="http://sourcegrid.codeplex.com/license" rel="nofollow">link to the project</a> it is the <a href="http://www.linfo.org/mitlicense.html" rel="nofollow">MIT license</a>, not LGPL.  <a href="http://en.wikipedia.org/wiki/MIT_License" rel="nofollow">Here is a wiki page on the MIT license</a>.</p>

<p>So I think you need to have this notice in your software somewhere:</p>

<blockquote>
  <p>Copyright (c) 2009 Davide Icardi</p>
  
  <p>Permission is hereby granted, free of
  charge, to any person obtaining a copy
  of this software and associated
  documentation files (the "Software"),
  to deal in the Software without
  restriction, including without
  limitation the rights to use, copy,
  modify, merge, publish, distribute,
  sublicense, and/or sell copies of the
  Software, and to permit persons to
  whom the Software is furnished to do
  so, subject to the following
  conditions:</p>
  
  <p>The above copyright notice and this
  permission notice shall be included in
  all copies or substantial portions of
  the Software.</p>
  
  <p>THE SOFTWARE IS PROVIDED "AS IS",
  WITHOUT WARRANTY OF ANY KIND, EXPRESS
  OR IMPLIED, INCLUDING BUT NOT LIMITED
  TO THE WARRANTIES OF MERCHANTABILITY,
  FITNESS FOR A PARTICULAR PURPOSE AND
  NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
  FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF
  CONTRACT, TORT OR OTHERWISE, ARISING
  FROM, OUT OF OR IN CONNECTION WITH THE
  SOFTWARE OR THE USE OR OTHER DEALINGS
  IN THE SOFTWARE.</p>
</blockquote>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
