## What are the most important features to include when building Content Management System?

- posted by: [pennyfiller13](https://stackexchange.com/users/-1/2438-pennyfiller13) on 2010-02-03
- tagged: `development`
- score: 1

I'm building a new social platform.  I understand that is very important to include a Content Management System as part of the development.  Can you describe specific features you would develop within CMS function for the purposes of running a social platform website.  How will CMS prove to be efficient?


## Answer 7530

- posted by: [Frederick Cook](https://stackexchange.com/users/-1/2344-frederick-cook) on 2010-02-03
- score: 1

In general, you can either design your own, or use an out-of-the-box CMS such as Drupal.  If you design your own, I would say you would need to either bring on a technical co-founder with database experience or spend a bunch of time with someone like that learning how to lay out the database architecture.

In general though, if you design your own, you will probably need (Edited):

 - Model - interaction between relational database and user interface
 - View - user interface
 - Controller - relational database, and associated stored procedures to access it

If you want more detail, you may try posting this over at http://stackoverflow.com/ since it is a more technical question.


## Answer 7633

- posted by: [Abdu](https://stackexchange.com/users/-1/2029-abdu) on 2010-02-04
- score: 1

Building a social platform AND a CMS is huge. First find out if you can just use a read made social software and a ready cms. Check out DotnetNuke + Active Social. I mention these two because I know ASP.NET. I am sure PHP and other platforms have similar combinations. But building them from scratch is too much work.


## Answer 7638

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-02-05
- score: 1

<p>Really more of a Stackoverflow conversation, but here is a good resource to review when building CMS systems.</p>

<p>From <a href="http://www.packtpub.com/PHP-5-CMS-Framework-Development/book" rel="nofollow">PHP 5 CMS Framework Development</a> </p>

<p>Required features</p>

<ul>
<li>user management</li>
<li>access control</li>
<li>security</li>
<li>extensibility</li>
</ul>

<p>Desirable features</p>

<ul>
<li>performance</li>
<li>database abstraction</li>
<li>menuing</li>
<li>internationalization/localization</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
