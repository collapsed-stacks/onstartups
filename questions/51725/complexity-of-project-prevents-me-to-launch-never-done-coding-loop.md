## complexity of project prevents me to launch "never done coding loop"

- posted by: [Rubytastic](https://stackexchange.com/users/-1/16595-rubytastic) on 2013-11-14
- tagged: `launch`, `release`
- score: 1

<p>*</p>

<blockquote>
  <p>I feel like im heading to a never done coding and never going to
  release my webapplication for several reasons. For the last year I
  have been using this project to learn a new programming language (
  ruby on rails ) then I implemented many fancy features to keep the
  code clean like splitted route /config/routes/*.</p>
</blockquote>

<p>*</p>

<p>I feel im constantly at the "almost done" fase, although using a project management tool to keep track of al known issues, bugs, improvements and have a time slot start_at to end_at I can keep track of the project somewhat over different versions. Currently Im at version 2.0 where there is most of the stuff done.</p>

<p>I have not written a full testcase (specs ) yet for my project and feel i will skip on this for now to first validate if the application will be used as thought. 
but have started writing them at least. The problem now it seems that code is breaking for no reason sometimes even though the code is very well organized, modulized, cleanedup and refactored ( except the views which i planned to use presenters but for now leave as is due to prevent further delays)</p>

<p>launching this project feels very personal and i feel lots of frustrations not heading my goal sooner. I recently refactored most of the code because It was technically not solid enough ( realtime game element) which makes it a much more hassle than some regular site.</p>

<p>How to best tackle this?
I for now decided:</p>

<ul>
<li>Put all issues not urgent or important in backlog</li>
<li>Not fixing any more bugs as of this point, if it just works its OK for now</li>
<li>Heading towards production environment be running and solid</li>
<li>Only checking the user registration onces more but after this no modifcations to it anymore</li>
<li>Plan to invite some friends to the site this weekend</li>
<li>Not spending all my hours anymore on this project but just minimize the hours and try to do more work in these and just finalize </li>
<li>skip features like mobile views and mobile versions for now</li>
</ul>

<p>Even with above in mind i still feel i never going to be able to release/launch since everytime there keeps getting issues. I recently switched form unicorn to puma and added some monitoring tools for the several background services like redis and sidekiq.
Yes i have done a lottt of work but still "What you see" on the frontend of the application its not visible that so much logic is inside the application.</p>

<pre><code>+----------------------+-------+-------+---------+---------+-----+-------+
| Name                 | Lines |   LOC | Classes | Methods | M/C | LOC/M |
+----------------------+-------+-------+---------+---------+-----+-------+
| Controllers          |  3396 |  2617 |      37 |     272 |   7 |     7 |
| Helpers              |   623 |   434 |       0 |      71 |   0 |     4 |
| Models               |  1522 |   653 |      33 |      82 |   2 |     5 |
| Mailers              |   324 |   261 |       7 |      41 |   5 |     4 |
| Javascripts          | 19961 | 14613 |       0 |    1351 |   0 |     8 |
| Libraries            |   726 |   543 |       7 |      26 |   3 |    18 |
| _pending specs       |    27 |    17 |       0 |       0 |   0 |     0 |
| Controller specs     |    45 |    38 |       0 |       0 |   0 |     0 |
| Model specs          |   142 |    26 |       0 |       0 |   0 |     0 |
| Request specs        |    74 |    60 |       0 |       0 |   0 |     0 |
| Routing specs        |   299 |   212 |       0 |       0 |   0 |     0 |
| View specs           |    80 |    66 |       0 |       0 |   0 |     0 |
+----------------------+-------+-------+---------+---------+-----+-------+
| Total                | 27219 | 19540 |      84 |    1843 |  21 |     8 |
+----------------------+-------+-------+---------+---------+-----+-------+
  Code LOC: 19121     Test LOC: 419     Code to Test Ratio: 1:0.0
</code></pre>

<p>YES i need more specs </p>



## Answer 51861

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2013-11-24
- score: 0

<p>Release NOW.</p>

<p>Releasing a product is scary, making the code better is comforting - but at some point you have to get over your fear and get the damn thing out the door.</p>

<p>You can fix bugs later, you can add features later, you can write tests later, you can refactor later, you can even make major design changes later. as long as users are able to start using the product (even if it's difficult or need manual work by you) you can release the product.</p>

<p>"If you are not embarrassed by the first version of your product, you've launched too late." - Reid Hoffman.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
