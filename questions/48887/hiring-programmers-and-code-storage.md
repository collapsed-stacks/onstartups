## Hiring Programmers and Code Storage

- posted by: [clifgray](https://stackexchange.com/users/-1/21414-clifgray) on 2013-05-02
- tagged: `crm`, `code`
- score: 3

I have two freelancers working for me right now and I am using Freelancer.com where you simply send code back and forth by zipping it and using their proprietary messaging system which is clunky. 

I would rather use another solution where you can have code related to specific clients and store it permanently online.  Like a CRM bred with a good repository. Do you know of any products like this?


## Answer 48889

- posted by: [James Wood](https://stackexchange.com/users/-1/26080-james-wood) on 2013-05-02
- score: 3

How about TFS Online? http://tfs.visualstudio.com/

Free for less than 5 users (and for a short time free for even more than 5 users).


## Answer 48891

- posted by: [MDMoore313](https://stackexchange.com/users/-1/23558-mdmoore313) on 2013-05-02
- score: 3

A company I used to work for had us use [redmine](http://www.redmine.org/). We never uploaded code through it, however it does integrate with SVN which we did use. If you have them on separate projects you can create separate repo's and limit access to each one.


## Answer 48895

- posted by: [Jeanne Pindar](https://stackexchange.com/users/-1/26083-jeanne-pindar) on 2013-05-02
- score: 3

<p>We host our repository at <a href="https://www.assembla.com/home" rel="nofollow">Assembla</a>,  which also provides ticketing, forums, email notifications etc. </p>



## Answer 48898

- posted by: [NtscCobalt](https://stackexchange.com/users/-1/26085-ntsccobalt) on 2013-05-02
- score: 3

<p><a href="https://bitbucket.org/" rel="nofollow">BitBucket</a> gets my recommendation. Unlimited Free private GIT or Mercurial repos as long as 5 or less users are allowed access to any given repo. If you are hiring programmers from the Open Source world GIT is probably the Source Control you'll want to use though BitBucket does not provide free Bug-Tracking tools.</p>



## Answer 48929

- posted by: [MarkWalls](https://stackexchange.com/users/-1/26098-markwalls) on 2013-05-03
- score: 3

Either TFS online or Bitbucket are good options. Both of them are free to use. I use TFS because it is the best of breed among the free project management options that link to code directly, and because I'm a .NET developer it is the most integrated with my platform.

Alot of it depends on the code base you are programming in though. I prefer to use TFS for .NET projects because then I can have my project management and code base together, and in .NET the programmers can link specific task items to code changes checked in to the central repository.

TFS online now has Git repository capabilities, along with their more centralized proprietary change tracking technology, so it is pretty open.

Bitbucket is Git/Mercurial based, but it is free and open. I haven't enjoyed tracking project completion through them though. It isn't really part of their UX.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
