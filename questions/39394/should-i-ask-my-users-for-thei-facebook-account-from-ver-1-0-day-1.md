## Should I ask my users for thei facebook account from ver.1.0/day 1?

- posted by: [Ted](https://stackexchange.com/users/-1/14069-ted) on 2012-05-25
- tagged: `mobile`, `users`
- score: 0

I am about to launch my mobile app which should be useful to many users. It is free of charge to download and use.  
I have a dilemma where I am not sure whether I should ask my users to login (either with facebook or with a simple login details+email address) or not.  
I could give my service to anyone using the app, but I do think that having my users contacts (facebook or email) may be a good idea.  
I do know that using push notifications is a way to communicate but having a facebook login would yield a lot of leverage to my customers and the users.  
I think that the downside of this might be users unwilling to give their faceobok details.
Of course, I could change things as I move along versions, meaning - not asking for personal info right from the start, but as soon as the next version will be out, I can ask for login details.

Would love to hear all your ideas.
What are your thoughts ? 


## Answer 39397

- posted by: [Matej Zlodej](https://stackexchange.com/users/-1/15950-matej-zlodej) on 2012-05-25
- score: 1

I had the same dillema when was designing my own mobile app. I think you should avoid requesting data which is not necessary for apps functionality, mainly because you don't want potential downloaders to turn away just because they don't feel like sharing their FB information (additionaly, there is still fair percentage of people who don't have facebook profile).

When i was analysing user feedback on apps similiar to mine, I noticed plenty of complaints related to necessary FB interaction, so negative effect doubled: 1. users didn't download app 2. those who did, gave poor rating on android market.

Ofcourse, facebook within app can be very useful, but I think it should be optional. However, you should find a way of rewarding your users for sharing FB info and mentioning your app (or whatever way you integrate FB in your app). For example: check in and get someting extra (but again, this should not be the only way to get that extra thing). 

So be careful with collecting personal information, people are less and less willing to share their personal infromation, especialy when they don't see any benefits in it (another related point to this subject: sometimes you should explain why doing something is beneficial for user i.e. give us your home address and you will recieve free gifts every christmas)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
