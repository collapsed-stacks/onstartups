## Which to show first: login or register screen or both?

- posted by: [Genadinik](https://stackexchange.com/users/-1/8929-genadinik) on 2011-12-26
- tagged: `website`, `registration`
- score: 1

I have a site for which I am working to improve user onboarding.

What happens now is that when a user does some action that requires him to be logged in, I make a jQuery popup come up telling him to log in. And if he is not registered, there is a link to registration.

But sometimes I see sites that do it in reverse order and shoe the "register" screen first.

I guess if you want people to register, the register screen makes more sense, but then it would annoy people who are already registered. No?

What is the best practice for doing this sort of thing? Does it make sense to show both, the register and login form on the same popup?



## Answer 34145

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2011-12-26
- score: 1

<p>I think the best idea is to include both, similar to the way a bulletin board or forum does it. Do this in a header or sidebar that is obvious but out of the way. And show the content of the main screen to indicate to the user what they are missing by not registering.</p>

<p>A good example are <a href="http://wordpress.org/support/" rel="nofollow">the WordPress.org forums</a>.</p>



## Answer 34150

- posted by: [Karan K](https://stackexchange.com/users/-1/15160-karan-k) on 2011-12-26
- score: 1

It depends whether you're trying to be a site that gets loads of users, or a site that wants to please your users. 

For example Gmail, they have loads of users, they want their users to come back and use their services again, so the login is first, if you want to use Gmail services, you can register easily with the link.

Facebook, completely focused on growth, but they have 700000000+ users to please, so they have both.

A site that tries to get you to register by the simplest means possible is usually trying to trick you in to joining. I tend to stray away from sites that have a register form inline, and a login link externally, they usually turn out to be spam sites that send me daily emails to buy rubbish. 

I suggest you have a login/register button, on click, open a popup with login, and have a register link, on click of register, fold out a minimal register form with 3 fields, then post that data to a longer form. Thereby levelling out both aspects, and keeping user-annoyance to a minimum.

Good luck :)


## Answer 34174

- posted by: [Abhijeet Kulkarni](https://stackexchange.com/users/-1/14856-abhijeet-kulkarni) on 2011-12-27
- score: 0

Have both Login and Register on same pop up windows so that if user haven't register they come to know where they have to register many times they have to search where to go for registration so it will be good to register and login same pop up.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
