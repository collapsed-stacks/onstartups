## Is it a good idea to create a new app on WordPress?

- posted by: [Sirwan Qutbi](https://stackexchange.com/users/-1/7815-sirwan-qutbi) on 2011-02-17
- tagged: `ideas`, `wordpress`, `apps`
- score: 2

Is it a good idea to use WordPress as the base for a startup app? Would a VC invest in an app if it was built on WordPress, regardless of the idea? The app, for example, is a photosharing site using the user's system on WordPress to share and post photos to each other.

Good idea, or use something 'faster' like django?



## Answer 20339

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-02-17
- score: 2

What is wrong with using Wordpress? How is it any different than using Codeigniter or Kohana which are both PHP frameworks? A VC isn't going to say, "Your site isn't running on code that was 100% created by you and your team, we don't want to invest."

If you want to get into specifics, by your logic a VC could refuse to fund your application because you are using Apache as your web server and not a web server that you've created yourself.

The technology does however play a crucial part I believe, but not what technologies you have used, but rather how well thought out your design and development process is and how you've implemented them. 

Wordpress if optimised correctly can be used for anything, it's pretty much a CMS framework in my opinion in that it can be extended and hacked easily unlike a lot of other CMS's.

Stick with Wordpress if it is what you know. Wordpress has the simple admin and content creation features baked in going for it. Remember that anything can be optimised regardless of language or software of choice.


## Answer 20363

- posted by: [Andy Cook](https://stackexchange.com/users/-1/6493-andy-cook) on 2011-02-17
- score: 2

<p>Technologies don't matter to investors. You could write you entire app in BASIC if you wanted and they wouldn't care. The reason why you don't want to write your app in BASIC is because it will take you forever to finish anything and gain any traction.</p>

<p>Use whatever technology you can to get a product out the door as fast as possible and test whether people even want it or not. If you have a deep understand of how Wordpress works and can make it do what you want, why not use it? I've programmed 4 projects on Wordpress so far and have run into relatively few problems.</p>

<p>Downsides to building on Wordpress</p>

<ul>
<li><strong>No guaranteed plugin support</strong> You're going to spend a bulk of your time finding plugins and testing them, only to find they don't fit into your application. You also don't want to modify a plugins source code because if you update it by accident, you'll lose your work. And you never know when a plugin will be deprecated by a new Wordpress Core update.</li>
<li><strong>Can't modify the core</strong> - Never modify the Wordpress core. You're going to have to write your own plugins or PHP files to make Wordpress do what you want</li>
<li><strong>No built in Ajax/Javascript support</strong> - I'm not sure about CodeIgnitor, CakePHP and other PHP frameworks, but Wordpress does not have native support for AJAX methods. You can query the Wordpress database extremely easily, but you can't make it do much on the front end.</li>
</ul>

<p>Upsides to building on Wordpress</p>

<ul>
<li><strong>Rapid development environment</strong> - You could get a minimum viable product up in a weekend just to see if anyone wants to even use your idea.</li>
<li><strong>Great documentation</strong> - Wordpress has some of the best documentation I've seen</li>
<li><strong>Great community</strong> - There are thousands of plugins and entire communities that rally around Wordpress like <a href="http://wordpress.stackexchange.com/">Wordpress.StackExchange</a></li>
</ul>

<p>In my opinion, Wordpress is an amazing platform to build the first iteration of your product on and get something out the door. You're going to rebuild your entire site anyways, so you might as well waste no time learning and getting your Minimum Viable Product done.</p>

<p>You need to think seriously about your customer acquisition strategy. That's going to be your biggest challenge. And here are some samples of sites I've hacked on Wordpress. They all took me less than a weekend:</p>

<ul>
<li><a href="http://www.quochilla.com" rel="nofollow">Quochilla</a> - A website for startup quotes</li>
<li><a href="http://www.mybookhound.com" rel="nofollow">MyBookHound</a> - Share your books with friends and track where they go</li>
<li><a href="http://www.sponsorastartup.com" rel="nofollow">SponsoraStartup</a> - Try to get people with money to pay for your startup event tickets</li>
</ul>

<p>Message me if you have anymore questions or want to chat more! I love that topic of this thread.</p>



## Answer 20365

- posted by: [Scott](https://stackexchange.com/users/-1/6594-scott) on 2011-02-17
- score: 1

I've built various projects (if not profitable ones) on top of Drupal which is an Open Source CMS.  It has been fabulous for having tons of prebuilt fucntionality. 

The downside? 

If you go through a major upgrade, your add ons and tools could very well be broke and require new programming.  With a major upgrade from 6 to 7, I have to decide what's more important, getting drupal 6 modules ported over to drupal 7 or keep working on my project.

Since I am bootstrapping my projects with after hours time, I have been "forced" to stick with the drupal 6 environment with  the knowledge that I have a major pain point coming along down the road.

The upside? I wouldn't probably have anything up and running if I had to start from scratch.  A man only has so much time and resources.


## Answer 20337

- posted by: [bhanu prasad](https://stackexchange.com/users/-1/7050-bhanu-prasad) on 2011-02-17
- score: 0

VC's don care about technologies and also VC's don invest money on the product and they invest money on the team. If product is of 100% worth then only they value product for 30% and remaining 70% they concentrate on the team.


## Answer 20338

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2011-02-17
- score: 0

It is a good idea to build a product/feature in the WordPress platform. I am not sure if VCs would be interested in a startup that is dependent heavily (a feature) in a platform such as WordPress. However, if your product is popular, your startup could become an acquisition target for Automattic which is the company behind WordPress.

Just build it and find out by yourself. Concentrate in a product that customers are interested on, do not worry too much about VCs right now.


## Answer 20340

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2011-02-17
- score: 0

Would a VC invest in your App?
Yes - if you can get a huge user base (and maybe implement a monetization strategy).
No - if you can't get user traction.

Basically whether you use Wordpress does not independently determine VC investment. You could very well bank on other CMSes (Drupal, Joomla, etc.) if a user database and photosharing module are all you need.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
