## What are the Pro's and Con's of using log in with Facebook or log in with Google?

- posted by: [Don Tarinelli](https://stackexchange.com/users/-1/13278-don-tarinelli) on 2011-09-12
- tagged: `google`, `facebook`, `social`
- score: 10

I have seen more and more websites allowing you to log in with your facebook or google account.  I am in the process of building a new website and I am wondering what the pro's and con's of doing this is because I am trying to decide if i want to implement this in my own site.  


## Answer 29973

- posted by: [Atul Goyal](https://stackexchange.com/users/-1/11816-atul-goyal) on 2011-09-12
- score: 6

Pros of using Google/FB login (btw OpenId is also there which essentially is a similar thing):

 1. The biggest advantage for a user is that he **does not need to create and remember one more password**!!
 2. for you one advantage is that you don't need to worry about **security of user's passwords** (yes, it matters) 
 3. you're making users happy by making their **registration and login process simpler** as they already have FB/Google account. Complex registration method are very _successful_ in frustrating potential users away.


Cons:

 1. Ok, even if you use Google/FB login, you must keep in mind that **not all users want to use their credentials of some other *trusted* site (Google, FB) on your website**. Whether you call it lack of knowledge or privacy concerns, you have to consider all types of users. 
 2. Also, some people are concerned about Google/FB/OpenId **tracking users' browsing habits**. (well if you're using their 'login' they know which all websites you use which could be a privacy concern)

I'd suggest that whatever login/registration method you decide, it should be based on your target users. Take a look at Stackexchange registration (which I guess you must have seen), it provides so many options to make the registration process (almost) frictionless.

--
edit:

Benefits of using OpenId (as mentioned on their [website](http://openid.net/get-an-openid/individuals/) ). Actually, these also apply to other alternate login methods like Google/FB 

>  - Accelerate Sign Up Process at Your Favorite Websites
>  - Reduce Frustration Associated with Maintaining Multiple Usernames
> and Passwords
>  - Gain Greater Control Over Your Online Identity
>  - Minimize Password Security Risks








## Answer 30001

- posted by: [Rob Gordon](https://stackexchange.com/users/-1/8967-rob-gordon) on 2011-09-13
- score: 1

There are two other possibilities;

1. Letting people log on with both Google and Facebook, and other services as well - Twitter, Linkedin even Yahoo and others.  The easiest way to do this would probably be through an integration with Janrain Engine https://rpxnow.com/

The downside - if you got to be successful with lots of members, it could get pricey since they have a per-user fee.  Check their rate schedules. 

2. Don't do it at all.  I tried this on some of my sites, and I found it to be a trip into the weeds.  If your registration system really works, why not just keep control yourself?  No one knows were this market is headed, and unless you think it will dramatically increase your registrations, there might be some advantage of of keeping control of your member registration data yourself.  Then there will never be a question as to who "owns" your members. 


## Answer 30013

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-09-13
- score: 1

<p>The main reason sites offer log-in through third party services is that <strong>it reduces sign-up friction</strong>. Private sign-ups can be simple and easy, or they can be a royal pain. And often you only know that <em>after</em> you hit 'register.'</p>

<p>So that's a great reason for supporting one or more social sign-ups. But there are alternatives. Plus, if you <em>do</em> go for a third party identity system for initial signup there's an important choice.</p>

<p><a href="http://Posterous.com" rel="nofollow">Posterous.com</a> has its own private identity space. But they also make it super easy to sign up. Either fill in (just!) email, user name and password on the home page, or without signing up first you can email post@posterous.com and you're off and running with your first blog post. And some sites started out majoring on mobile sign-up, using that other common identity, your cellphone number. Third party logins aren't the only low-friction mechanism.</p>

<p>So think about the use cases your new site is serving, and ask, "What are the lowest friction ways someone could get up and running?"</p>

<p>If you do decide to use (any or all of) Facebook, Twitter, Google or an OpenID to get people onto the site, you still have to choose whether that is (a) one available choice, the other being a private sign-up, (b) the <em>only</em> method to get and stay registered, (c) an on-ramp from which you will then work to convert users to a private identity.</p>

<p>Each of those choices has its supporters. The best call is going to depend on the nature of the service you intend to offer and the users you will serve. Think it through, and <strong>make the best call you can based on what you know now</strong>. (And you can always change your mind when you have the experience to make that judgement better. It can be moderately annoying to users, but if you handle change well it can build your reputation!</p>



## Answer 37020

- posted by: [Tien Do](https://stackexchange.com/users/-1/9267-tien-do) on 2012-03-10
- score: 0

Pros:
1. Your users don't have to register and remember a new account.
2. They can log in to your website in a familiar way.
3. You save time from coding yourself a trivial user management functions.

Cons:
1. Someone worries about privacy but I don't think it makes much sense since a website can only access minimum data of a user such as first name, last name, email which must be submitted to every website they want to use.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
