## Changing Licensing model for a Software Framework to more permissive

- posted by: [romaninsh](https://stackexchange.com/users/-1/13659-romaninsh) on 2011-10-23
- tagged: `software`, `open-source`, `licensing`, `webdev`
- score: 2

I'm author of the "[Agile Toolkit][1]" Framework. Currently it's available under dual license 

 - Affero GPL - any use, personal or commercial
 - Permissive license for $130/domain
 - Permissive license for unlimited domains $460/year

([link for licensing terms][2])

Since I have released it, many users have expressed desire to make personal projects and AGPL license seem to be an obstacle. I don't want to adopt MIT/BSD as it would pretty much any chance for me the get any revenue.

Suggest what license combination to use to keep framework open source and free for personal use, but still require to purchase a license for commercial use.

Also - I know I might need to seek advice from a legal advisor on this, but this is a very low-profit project so I can't afford to spend much. 

  [1]: http://agiletoolkit.org/
  [2]: http://agiletoolkit.org/commercial/store


## Answer 31800

- posted by: [Kekito](https://stackexchange.com/users/-1/5898-kekito) on 2011-10-23
- score: 2

I think you have the best combination of licenses already.  Apache/MIT/BSD clearly don't work.  Any other GPL license would allow commercial use since I presume people running a website would not be distributing the modified code.  The Affero license is the only GPL license that applies even when the code is not distributed.

I don't see why people using your code for personal products are complaining about the Affero license.  I would stick with your current course.


## Answer 31794

- posted by: [Alain Raynaud](https://stackexchange.com/users/-1/502-alain-raynaud) on 2011-10-23
- score: 0

How many users is many? You can grant licenses on an individual basis. That might be good enough for you, while providing a very strong legal protection. Just add a link to your site saying, if you need a license for private, limited use, email restrictedlicense@myproject.com.


## Answer 34073

- posted by: [Krzysztof Kowalczyk](https://stackexchange.com/users/-1/3945-krzysztof-kowalczyk) on 2011-12-23
- score: 0

You're in a tight spot - there is no existing open source license that has the properties you seem to want.

I can see why GPL turns people off - since your code is PHP, GPL license would force people to publish all their PHP backend code as GPL and I can understand why it makes people uncomfortable (as well as requiring more work for them to comply) even if it's for personal project.

On the other hand, as you pointed out, you can't just use MIT or BSD license as it provides no reason for anyone to pay you.

You need a custom license, one that doesn't require people using it for personal projects to publish all of their code but also has enough restrictions so that people using it for business purposes will pay you.

The only idea I have is a license that says: use for personal projects is free (and, unlike GPL, there's no need to open-source your code) but use for commercial projects requires paying you.

I've seen such scheme used by some desktop software. Would it work? I don't know. Clearly, it's a honor-based system as the definition of what is a commercial project is fuzzy and your ability to find out who breaks the rule and enforce the license limited (although the same can be said about GPL license as well).




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
