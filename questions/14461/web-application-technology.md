## Web Application Technology

- posted by: [Jeff](https://stackexchange.com/users/-1/4460-jeff) on 2010-09-26
- tagged: `ecommerce`, `webdev`, `webapp`
- score: 0

My startup idea involves a web application that has the following requirements:

1. will need to charge my customers securely using someone else's service
2. must scale easily   
3. must be cheap to deploy
4. must be reasonably responsive (much of it will be client side javascript, but there is some server interaction)
5. will need a database on the back end (not a huge database, but it will need to scale with the customer base) 

Who should handle billing/payments? (Paypal?)

What technology do you all recomment using to write the appilcation? (I'm leaning towards: MySQL/PHP/Javascript)

Where should I deploy the app? (Amazon cloud?)



## Answer 14467

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-09-26
- score: 12

<p>Jeff, I don't mean to be ill mannered, but you're clearly not a technology guy. "Cheap" and "scale easily" don't go together in the same sentence.</p>

<p>There is no way to answer your question. <strong>You're not providing a level of detail even nearly close enough to make a solid architecture choice.</strong> And even if you did, the most important factor are the people involved, certainly not the programming language. The most important single factor in picking a programming language and web framework should be your peoples proficiency and level of experience with the platform.</p>

<p>My suggestion to you would be to think of every tech person you've ever worked with. Can you think of someone who is a very good programmer, gets things done, is honest to a fault, and compatible with your personality? You need a <a href="http://answers.onstartups.com/questions/tagged/co-founder">tech co-founder</a>.</p>



## Answer 14464

- posted by: [blparker](https://stackexchange.com/users/-1/4449-blparker) on 2010-09-26
- score: 2

 1. I don't see a reason why PayPal wouldn't be sufficient. It's secure and capable of handling all the traffic you could send it.
 2. If the application is well written, most frameworks should be able to scale pretty well.
 3. I would suggest using an open source technology then.

As far as the rest, I would recommend using:

 - PHP/MySQL/jQuery (takes a lot of the bare metal JS out of the equation)
 - Ruby on Rails/MySQL/jQuery

Either of these work really well, are easy to use, and have been shown to scale well for large sites with large amounts of traffic.

As far as deployment, that basically boils down to a preference. If you are going with a hosted option (GoDaddy, Hostmoster, etc), you can usually get a plan with unlimited bandwidth and disk storage for under $5 a month. Not a bad deal. With these plans, you would have the ability to host your application and database. As for the cloud approach, I'm not to certain about that...some cloud services are going to NoSQL route, so you would need libraries to handle your data management for whatever technology you pick.

At this stage, don't get too hung up on details. Go with what you're comfortable with. **Be crappy at first, release often, and iterate.**


## Answer 37965

- posted by: [Emma McCreary](https://stackexchange.com/users/-1/15481-emma-mccreary) on 2012-04-08
- score: 0

I don't recommend PayPal. The way they do subscriptions is awful. Go with Chargify or build your own system that interacts with one of the gateways that lets you have a credit card "vault" to store people's cards. That way you can charge them when you need to, and not have to worry about creating and deleting subscriptions when they upgrade. It's the most flexible solution.

You didn't mention a web framework. Choosing a good one is essential to build apps quickly that are scalable. I recommend Yii, but there are others that are good - go to StackOverflow for these kinds of questions. 

But I agree with the other posters, you need a tech partner. If your business's core product is technical, you need a technical person on board. There will be hundreds of technical decisions to be made.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
