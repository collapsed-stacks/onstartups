## Social Network Idea

- posted by: [Daniel](https://stackexchange.com/users/-1/10538-daniel) on 2011-06-04
- tagged: `social-network`, `facebook`
- score: 3

I have an idea of a social network site. I think that technically I can make this idea as a facebook application, but commercially speaking, what are the disadvantages and the advantages of doing it as a facebook application instead of making my own site?


## Answer 25914

- posted by: [Mike](https://stackexchange.com/users/-1/10720-mike) on 2011-06-04
- score: 1

<p>I guess I'll give an answer, hopefully at the very least I'll give you a list of things to think about.</p>

<p>The trouble with this question is that there is very little information to go on, so I can only give general suggestions.</p>

<p>The biggest question to think about is what your goals are and what your users will want/expect. If you expect that most of your potential users are going to be on Facebook and would enjoy using it on through Facebook, than making a Facebook application rather than an external website which interacts with Facebook could be the way to go. On the other hand, if you expect that either your user-base is going to somehow include or attract a significant amount of non-Facebook users, then creating your own separate website which simply allows Facebook authentication (and possible integration) may be better.</p>

<p>You specifically ask about this in terms of commerce. Unfortunately I do not have as much knowledge in this subject, but the little that I do know is this: Facebook now has its own system of currency in the form of "Facebook Credits". I am not sure what the restrictions on this are, but if you are able to integrate with this system (no matter which method you choose), then it could allow you to quickly and easily start making money. I do not know how popular the Facebook Credit system is currently. On the other hand, there is also always Paypal which could be just easy to setup (note: I have not used Paypal, so I do not actually know what is involved).</p>

<p>The reason I, personally, chose to make a website rather than Facebook application is because I am expecting my users to integrate with multiple social systems such as Twitter, Digg, and others. I also wanted to allow my users to login with OpenID along with the other popular <a href="http://oauth.net/" rel="nofollow">OAuth</a> (system Facebook uses) services.</p>



## Answer 27129

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-07-05
- score: 0

I don't think it is a mutually exclusive choice anymore.

You can design it so the layout of the site will suit the Facebook restrictions and then put your own frame around it or if you design the site with that in mind you can seperate out the functions from the views and have 2 versions one for facebook and one for the rest of the world. 

**Commecially speaking** ...

Facebook gives you a huge market, that if your app is cool could allow you have a huge uptake. It has a lot of stuff built in that you can take advantage of in terms of the platform and social graph etc. Basically you don't have to reinvent the wheel or go through the pain of collecting all those people yourself.

Doing it on your own means that you are in control of it all. Decisions made by facebook about security, marketplace, positioning / marketing visablity changes, random rules that may or may not impact you are not your problem. If you end up with a lot of users on your own then you are more likely to be seen as a safer buyout target due to the list above, though if your doing well on facebook people would target you as a buyout option anyway.

**Summary**.

As I said up the top ... its not mutually exclusive ... I would start designing your own API which you can use on your own site, on facebook, in an iPhone/Win7Mobile/Andoid app and to bind you into other sites. Get this right and it will be somewhere between a 10% and 20% additional effort to spin up a new platform. Do your research about what is on offer from the FB API and use it as a guideline for what to build into your app. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
