## What is the best way to test whether people would pay for a web application?

- posted by: [dynZack](https://stackexchange.com/users/-1/4095-dynzack) on 2011-09-13
- tagged: `pricing`, `webapp`, `freemium`, `charging`, `testing`
- score: 9

I am currently implementing a relatively simple web application, as I'm trying to dive into Ruby on Rails. It turns out be going quite well and, in my opinion, it will appeal to a lot of users. But I'm only speculating, I haven't actually tested this.

I never thought of charging the users, but I'm starting to think whether users would be willing to pay a small fee (e.g. 1$/month) to use this app. 

My question is, what is the best way to test if the subscription model would be successful, without killing the app altogether? 

(I guess the safe answer is to first give it for free, see how it goes, and then charge the users accordingly. However, I tend to think that is much harder for a user to **pay**, when he had the same service for **free** before.)


## Answer 30051

- posted by: [bwasson](https://stackexchange.com/users/-1/12611-bwasson) on 2011-09-13
- score: 5

What the general strategy tends to be is to offer a free version of the application for testing, and to build traction with your users, and then come out with a paid version once you have a significant user base. A portion of your existing user base will convert to the paid version, netting you income, and you wont piss of the rest of your customers. 

Another thing to think about is that you might be able to more effectively monetize your application by another method. 

IE, using your user base and traffic to generate advertising revenue. If you do implement it well, users wont mind at all, and you might actually generate far more income from advertising than you would from subscriptions, and you don't have to worry about all of the administrative overhead that comes with managing a subscription service. 

Also remember, you will pay credit card processing fees for your subscriptions, so a $1/month subscription would likely only net you around $0.30/month/user.


## Answer 30069

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-09-14
- score: 3

Congratulations! You've accidentally discovered the profound truth that strict constraints (being new to Ruby, say) sometimes produce better products (you stayed simple and users liked it!).

Your best test may be to introduce the charge soonest, with, say, a three month free trial, with no need for people to pre-enter payment details. 

That gives you time to work out how best to bill - and to see if your metrics fall through the floor just for having a visible fee.

You now have the basis for split testing. You can start sending out offers to incentivize people to sign up early, for 12 months at a crazy discount. Remember, at this stage you should care far more about *whether* people will pay than *how much* they'll be willing to pay. 

Build your own confidence - knowing you can always bail, either to free, or freemium. But if you have something of value, straight charging (if it works out) wins every time. 


## Answer 30065

- posted by: [John](https://stackexchange.com/users/-1/13157-john) on 2011-09-14
- score: 2

You might consider segmenting the market into paid and unpaid by feature-set. For example, for free, users get feature A, B, and C. For the silver package ($1/mo.) a user can also get features D, E, F, and G. I'm sure you get the idea. Then, you see how many people sign up for the silver vs. gold vs. platinum package. If you find too few users signing up for the free version then you might want to move some features from the silver package to the free package.

Eventually, the answer will come.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
