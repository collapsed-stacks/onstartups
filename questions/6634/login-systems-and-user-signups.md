## Login Systems and User signups

- posted by: [Eric](https://stackexchange.com/users/-1/1832-eric) on 2010-01-16
- tagged: `user-interface`
- score: 2

Our web app deal with social networks and different login systems fit with the app. MY question is which login frontend do you prefer.

a. a username / password text field form with submit button
b. a sign in with twitter OAuth button only
c. a facebook connect button only
d. combination of a + b
e. combination of a+b+c

I really feel that a segment of users are comfortable with A that they do not try a web app when its not there. and i feel that some LIKE to create a separate account to try before linking their Twitter/facebook account. anyone have any insights on login frontends/system's effect on user signups?


## Answer 6637

- posted by: [Denis Hennessy](https://stackexchange.com/users/-1/311-denis-hennessy) on 2010-01-16
- score: 2

I think the Facebook Connect and Twitter OAuth are fine where there's a **natural** link between your application and those networks. However, I think the regular username/password logins are important for people who either don't have a Facebook/Twitter account or don't want to link those accounts to your app until they've used it for a while.

If your app doesn't have a natural link to social networks, then I think it's probably a waste of time adding an additional authentication mechanism.


## Answer 6641

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-01-16
- score: 2

I'm not on Twitter or Facebook, so b) and c) alone are dealbreakers for me.

**For "regular" users:** I'd say logon via email and password; email (as user id) and password and nothing else. My reasons are:

 - Many users are not on social networks, so a 'classic' logon method is required.
 - The email & password dialog is well known and has good usability. More complex logon methods are less well tested and understood. The model of having your logon credentials stored and managed on another site is not intuitive.

**For "techy" users:** I'm a bit in doubt, but I guess it's valuable to provide a choice between **username/password *or* OpenID**. OpenID is becoming common among tech-savvy users, and can simplify credentials management for the users.


## Answer 6645

- posted by: [Benjamin Wootton](https://stackexchange.com/users/-1/2094-benjamin-wootton) on 2010-01-16
- score: 1

I'm as techy as they come, but even I'm a bit put off by these login schemes such as OAuth.  

Consider offering it an option, but it would be waaay down my list of priorities as it would directly appeal to so few people.
 


## Answer 6659

- posted by: [Jesse](https://stackexchange.com/users/-1/2244-jesse) on 2010-01-17
- score: 0

I love the RPX interface.  rpxnow.com - you should check it out.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
