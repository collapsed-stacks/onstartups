## Sales Commission website with Geolocation?

- posted by: [A T](https://stackexchange.com/users/-1/15651-a-t) on 2012-02-09
- tagged: `website`, `sales`, `recommendations`, `proposal`
- score: 1

I'm looking for a Customer Relationship Management solution with an easy to use interface.

The simplest way to describe what I'm looking for is through a [very rough!] mockup:

![SalesCom site][1]

The idea is that the customer will sign-up on a separate site, and give a reference, which will then directly pay the salesman commission. I don't want multiple salesman to revisit the one place, as that leads to bad reputation.

Also, if I have multiple salespeople in one city, I don't want them to go to the same place on the same day, so salespeople need to choose what to add to their queue for the day (or week or month). 

So I was thinking a neat CRM geolocation site with queues would be best (with associated PhoneGap built mobile apps).

If there aren't any available, I'd be happy to open-source the whole project, and write it in Django or .NET.

**Are there any websites around which offer these above—streamlined—features?**

  [1]: http://i.stack.imgur.com/kgDCZ.png


## Answer 36155

- posted by: [Tim](https://stackexchange.com/users/-1/14914-tim) on 2012-02-14
- score: 1

We have had success with SugarCRM: http://www.sugarcrm.com/crm/ it's PHP based and open source so it's customizable. Since there are about a million CRM products out there and none of them will be exactly what you want out of the box I suggest you download this app and have it customized. If you didn't have the staff in house to customize it I would suggest getting a freelancer to customize this to your specs. That way you get exactly what you want at a very reasonable price since it shouldn't take too many hours to complete this kind of task. 

Good luck, 
Tim - VA


## Answer 36321

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2012-02-18
- score: 1

<p>AT - if you are looking for an open source solution that is easy to modify and make into your own creation I would suggest you look at <a href="http://www.fatfreecrm.com" rel="nofollow">Fat Free CRM</a></p>

<p>It's based or Ruby on Rails and follows all of the RoR conventions so it is pretty easy to jump in there and make adjustments and improvements. It would be ridiculously simple to add the <a href="https://github.com/alexreisner/geocoder" rel="nofollow">geocoder gem</a> - <a href="http://railscasts.com/episodes/273-geocoder" rel="nofollow">example of using it</a>.</p>

<p>I have been developing for quite some time and have done both Django and Rails, Ruby and Rails is my go to framework right now for web applications. Custom coding your solution in either would be pretty simple, using something like FatFreeCRM may get you to where you want to be a little faster. I'm definitely a Rails advocate.</p>



## Answer 36272

- posted by: [bwasson](https://stackexchange.com/users/-1/12611-bwasson) on 2012-02-16
- score: 0

The features you're looking for are included in just about every CRM application under the sun (And some ERP solutions as well). I have experience with SugarCRM and Salesforce.com Both are great, and are well worth the expense, though my company currently uses SugarCRM for cost considerations. 
Salesforce.com and SugarCRM are both highly extensible, so if you have the budget you could hire an expert to do the geolocation things, though honestly it's not really needed if you ask me. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
