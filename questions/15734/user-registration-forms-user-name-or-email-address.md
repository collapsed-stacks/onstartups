## User Registration forms - user name or email address?

- posted by: [JDelage](https://stackexchange.com/users/-1/2505-jdelage) on 2010-10-28
- tagged: `website`, `user-interface`, `registration`
- score: 11

I would like as simple as possible a registration and login process.  Should I use a username or an email address as the key identifier during the login?  (Presumably the user db might also a user name AND an email address (and a unique ID number, first and last name, etc) - my question is just for the login and registration.

Thanks,

JDelage

PS:  For those interested in this question, it was asked on the webmaster QA site, but the angle here is different (see http://webmasters.stackexchange.com/questions/3096/user-registration-forms-do-we-need-a-user-name).


## Answer 15741

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2010-10-28
- score: 13

I prefer using an email address because I always forget my login name. Even better, use OpenID. That's much better than either methods since now, the user only has to remember one login.


## Answer 15746

- posted by: [Martin](https://stackexchange.com/users/-1/4248-martin) on 2010-10-28
- score: 8

Whatever you do, please make it very easy to know WHICH one to use.  Please don't:

    Username: _________________

when you really mean email.  I can't stand that!


## Answer 15751

- posted by: [Ricardo](https://stackexchange.com/users/-1/42-ricardo) on 2010-10-28
- score: 4

I prefer username, don't make me type my full email address please! In the registration process you should ask for the email address to make sure your users can reset their password/username if needed. I usually have the same username for many different sites but different email addresses, depending on what type of site it is.


## Answer 15737

- posted by: [John Plummer](https://stackexchange.com/users/-1/4891-john-plummer) on 2010-10-28
- score: 2

I would suggest you use username as key identifier as you need to allow for users to change their email address.

You may consider also asking for (and verifying) an email address during registration incase the user forgets their password. ie. on the forget password form allow the user to enter a username or email.


## Answer 15843

- posted by: [Taryn East](https://stackexchange.com/users/-1/5160-taryn-east) on 2010-10-30
- score: 1

When I used to work a 9-5 job, I used to change job every few years... that meant I changed email every few years. If you set the login to be an email address once-and-for-all-time... and I change my email address, then I either have to lose my login for your system, or change the unique identifier that you use for me to login.

It's a much better idea to have a username that will always stay the same - and let me use the email address just for it's original purpose - ie getting in contact with me via email.


## Answer 15860

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-10-31
- score: 1

Why can't the user have the option: 

 - Email doubles as the Username if no username
   entered.
 - Login using either the email or
   username as the username.

This way, users that setup the account under a company email address can change it and keep it associated with the username for this account.

Obviously more difficult to implement, but the goal seems to make the user's experience as easy as possible without painting them into a corner.


## Answer 15836

- posted by: [Shree Mandadi](https://stackexchange.com/users/-1/1664-shree-mandadi) on 2010-10-30
- score: 0

If maintaining a User Demographics is not critical to your System, I would defer the Authentication to Other providers...

Open ID is good, But confusing to a lot of users... Better option is having multiple options.
90% of users have a Google/Yahoo/Facebook account. (I am making up the numbers here, But you get the idea).

Have options, which say, Login with your Google account, Facebook account, Yahoo Account or your OpenID. If you have neither, then and only then create an account on your System



## Answer 15837

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-30
- score: 0

I usually prefer email address as the login id. However the downside to that you will also have to provide the user an option to change the email id, just like change password. You'll have to develop a whole new process to validate by sending a link to the old email to confirm the change.


## Answer 15856

- posted by: [BBlake](https://stackexchange.com/users/-1/4274-bblake) on 2010-10-31
- score: 0

I've found the best sites are the ones that let you type either username or email in the username box.  Often times I find I can't remember my username for a particular site, but I'm pretty sure what email address I signed up with.


## Answer 50575

- posted by: [Dmitri Zaitsev](https://stackexchange.com/users/-1/27575-dmitri-zaitsev) on 2013-08-24
- score: 0

Since the question is about the simplest process, the answer seems obvious: Email and Password.

Why? Because you need to get back to user to send password reminder, so you need Email anyway. Then what is good about username?

It was mentioned that you can have the same user name easy to remember. What if next time you try to register, that username is taken? Now we are back to the problem of zillions of usernames. We already have problem with multiple passwords, do we want to add multiple usernames?

In contrast, little I remember better than my email. Forgot? Look in your mailbox! An objection mentioned when people change jobs or emails. But it is so easy to get a permanent email these days! Why not using that one?

Finally, if you really need to change the email, you can add it, validate, and allow the user to register with either one. Then the user can delete emails from the list. Slightly more complicated on technical site but not much so, comparing to the main security functionality of email validation and password recovery.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
