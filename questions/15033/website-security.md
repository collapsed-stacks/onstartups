## Website security

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-10-12
- tagged: `website`, `recommendations`, `security`
- score: 2

Last Saturday my site received an unusually high volume of brute force attacks. Yep, those darn teens from Western Europe or smart scripts from academic towns in Siberia, trying tirelessly to break into my site authentication.

Now, I'm thrilled with this development. That means I'm finally getting out of obscurity. Yey!

I spend an entire day restarting my server and applying solutions that would deflect those attacks. It seems to be under control. I am not going to disclose here my defense strategy but I would like to probe and see what others have done to defend their properties.


## Answer 15034

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2010-10-12
- score: 2

The single most important thing you should do is make sure the OS, all servers and all web applications are always up to date.

Everything else is specific to the attack (I've recently added a completely trivial to bypass "security" check on one of my comments forms, it's stupid but it stops the specific spam bot that is hitting that page)


## Answer 15060

- posted by: [Zuly Gonzalez](https://stackexchange.com/users/-1/2692-zuly-gonzalez) on 2010-10-13
- score: 2

Here are four simple things you can do:

 1. Keep everything updated, as Nir mentioned.
 2. Use strong passwords.
 3. Disable all services not in use. For example, if you don't need FTP, disable it. Every service you have running is another attack point.
 4. Run your services with as little priviledges as needed.

Also, keep regular backups just incase you need to reload your data on a fresh server.




## Answer 15272

- posted by: [user2387](https://stackexchange.com/users/-1/2387-user2387) on 2010-10-19
- score: 1

I've read an article about an open source security package for web servers on http://www.untwistedvortex.com/ You'll have to look for the article yourself, was about a month ago.

Haven't tried it myself yet, but I will *after* the next attack on my site :-)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
