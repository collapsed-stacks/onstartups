## Does my CMS choice limit the scalability or types of services I can integrate?

- posted by: [LongWinter](https://stackexchange.com/users/-1/8540-longwinter) on 2011-03-28
- tagged: `webservices`, `mobile`, `community`
- score: 4

My start up business will be a social service that also hooks to a mobile application. I want my users to be able to interact with my service over their phones or on their PCs. Naturally I'm thinking the service will be a huge hit with 1000s of users at a time at some point.

I'm very familiar with Joomla but I'm not a programmer. I was thinking of building out most of the site in Joomla and then having the core elements of my service developed to work within Joomla. 

Does a CMS built on a LAMP stack have any limitation on what kind of features/services can be integrated (or well integrated) and can they scale well if the service does become popular?




## Answer 22464

- posted by: [Joseph Barisonzi](https://stackexchange.com/users/-1/8791-joseph-barisonzi) on 2011-03-28
- score: 4

***Yes***. There are different issues with different CMS's for scalling and integration of different features.
***No***. It is simply a factor of time/money. With the right time and money you will be able to hire a programmer that will be able to integrate what you need. 

The web is littered with a plethora of custom made proprietary CMS platforms which have significant challenged in scaling, bridging and incorporating the features and services that you need. In fact in the early '00s it seemed that every web development firm tried to differentiate with a proprietary CMS. 

But, if you know Joomla- then you are looking in the open source world and you know that while there are platforms that work better, or are more or less easy to work with the bridging of php and mySQL can be done. 

Our team uses Joomla almost extensively and after 10 years has yet to find a scalability, feature or service that we have not been able to integrate with our site. The open source nature of Joomla, iframes,  APIs, developer community, and broad-based adoption allow us to meet all of our customers continually changing and growing needs. 

I think the biggest issue on a CMS is what language world you are going into .net/.asp or .php/msSQL. To me that is the critical question which determines scalability and what type of features will be easier to integrate. 




## Answer 22447

- posted by: [pdenya](https://stackexchange.com/users/-1/9005-pdenya) on 2011-03-28
- score: 2

Depending on the features and services you may end up working against the CMS a little bit but in general you won't be limited by your CMS choice as long as your willing to hire a programmer.

LAMP stacks are cheaply scalable.  You can scale cheaply with Amazon's platform but it can be a little bit intimidating.  There are also platform as a service offerings like Rackspace or PHPFog that make scaling effortless but slightly more expensive. 


## Answer 22488

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2011-03-29
- score: 2

<p>In my opinion if you want a CMS that is extensible and is based on PHP so you can use it on a cheap LAMP stack, you can't go past <a href="http://drupal.org/" rel="nofollow">Drupal</a>. It's a beast in terms of what can be done with it's powerful theming and plugin system.</p>

<p>Provided you use a CMS that is extensible, has a good database structure (proper indexes, optimised, etc), easy to theme and most of all only loads things when you need them (stay away from Wordpress in this aspect as it loads everything all at once).</p>

<p>Having said all of that, Joomla! is a pretty good CMS and in my experience I've never had a scalability or problem implementing new functionality. Another good heavy weight is <a href="http://expressionengine.com/" rel="nofollow">ExpressionEngine</a>, although not free, it's pretty powerful and cheap for what you get, not to mention it is built on the Codeigniter PHP framework.</p>

<p>I woudln't be worried about the CMS, but moreso what hosting provider you choose. If you're going to be offering a service that will have 1000's of users online at once, then you'll find that hosting will be the bottleneck.</p>

<p>Amazon has nice scalable hosting, although it can work out to be just as pricey as a standard dedicated server, the bonus is that it is infinitely scalable to accommodate any load or traffic.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
