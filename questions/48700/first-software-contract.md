## First Software Contract

- posted by: [SnakeDoc](https://stackexchange.com/users/-1/25569-snakedoc) on 2013-04-23
- tagged: `contract`
- score: 2

I currently write a lot of proprietary code that's buried away in some corporation and will never see the light of day (or another coder's eyes for that matter). But this will be my first endeavor outside the "corporate veil". Luckily this first client is a close friend, so any mis-steps I make won't be judged too harshly - this is not to say I don't want to deliver anything but my absolute best and come across to this friend as a top professional in the field -- I hope to get future recommendations out of this friend, so I don't want to screw it up!

Couple of things that concern me:

`1) Who "owns" the code when the project is completed?` 
  - Assuming I don't have a contract that assigns Copyright over to him/his-business, do I legally still own the code? Wouldn't a normal client want to own the finished project and/or have the ability to take the code to another developer if they choose? Am I shorting my client by not assigning copyright over to them/their business? 

`2) What if I want to take this codebase and morph it into a new product of my own? Am I able to? What if I just release it as-is with no modifications/improvements?`

`3) What if I were to "Open Source" the codebase during or after development?` I use GitHub's free account to host all my source code management because it's free and easy. I can see how this might become a problem for a project that must stay under-wraps... is this something I should discuss with my client?

Basically to summarize, I feel like this project might be something that I want to continue to tinker with after the client's product is finished -- possibly releasing my own version at some time. I feel that if I just do the work, then assign copyright and all rights/ownership over to my client/his business, then I'm the one loosing out since I would then have to start from scratch and re-write the product if I have the inkling to keep playing with it. On the flipside - I feel like I might be cheating my client by not giving them full ownership and rights, since they then would have essentially paid me to invent, then only have the ability to use it while I'd have the ability to do whatever I wanted. I want to be able to use the project as part of my portfolio and be able to keep improving it over time if I so desire. 

This must be a common issue with small biz developers. Please advise.

`EDIT:        `
To clarify, the thing that holds me up over the copyright/ownership issue is once I think out and code a software -- I cannot `unthink` it. Does this mean if I do not have a contract with my client that expressly allows me to reuse the codebase or parts in any manner I choose, or allow me to keep ownership of the code - then any project I do under these conditions means I am forbidden from building a similar product in the future? This is because I'd likely redo the same work in a similar fashion... 


## Answer 48702

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2013-04-23
- score: 1

Common issue? Absolutely!

There are a couple ways this can be handled, but they are both handled via the contract. Either you own the code, and the client has the right of use, or the client owns the code, and you have no use. There could, of course, be stages in between.

If the contract states that the client owns the code, then you may not put the project into open source, nor may you publish the project (even with modifications) on your own. Failure to abide by that at best will generate ill-will between you and the client, and at worst, get you sued.

If the contract states that you own the code, or rights to the code, then you can do what you want - subject to the terms of the contract. After all, the client is paying you to do the work, so they will be the ones to set the terms for this.

That being said, if you talk to your client, and address your desires and ambitions for the project, you can likely come to some agreement regarding ownership and use.

**EDIT**

In regard to "un-thinking" your work, it basically comes down to whether or not you can re-use what you've written. If you haven't come to an agreement regarding usage, then the answer is that you probably can't copy the code over. However, if there is a particular module that you developed which on its own isn't the project (for example, if part of developing the application you wrote a piece of code for tracking and notifying people about errors, but this has nothing to do with what the application does as a whole), then you likely could get permission to use it, and you could likely rewrite it without any issues.

Contrary to what the other user wrote, IP does not generally belong to the developer if he is being paid to develop. The client came up with the idea, the client is footing the bill for it. They are highly unlikely to turn around and say "in thanks for being paid to do some work for me, you now own that work too!"


## Answer 48724

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2013-04-24
- score: 1

(1) In the US, if a work is not a "work made for hire," and hasn't been assigned to the client, then the copyright to the work is held by the work's author.  So, the author can do whatever he/she wants to with the work.  For programs, a work is "made for hire" if it's produced by an employee within the scope of his/her employment.  Deciding whether you're an employee isn't as straight-forward as you'd think, but in general, if you're doing work for different clients on your own computer in your own space, you're not an employee.

(2) Because of (1), good software contracts spell out EXACTLY what the client is getting.  Typically, they don't get pre-existing material that you're just customizing for them.  But, if they're paying you to create something, they will usually want to own the copyright to what they paid you for.

(3) It's common to have a 'residuals' clause in software agreements that basically says "We're producing this for you, and it's all yours.  But, by producing this, our people gain skill and knowledge that isn't specific to your product.  And they're free to re-use those skills and knowledge to serve other clients as long as they don't specifically re-use the code they produced for you.


## Answer 48703

- posted by: [user23843](https://stackexchange.com/users/-1/23843-user23843) on 2013-04-23
- score: 0

1. Typically the developer owns the code. However, the copyright to the code will depend on the specific scenarios. For Example,
 a.) You are working in the corporate world. Every thing or most of it you code there will belong to your company for the compensation that they have provided you.

 b.) A client who pays you by the hour, can get into a contract with you saying that you may not use that code elsewhere. However, this becomes very tricky as there could be many common modules. So most of the times they have a non-compete clause so that you do not use it in any competing product. That is fair enough for both the parties.

c.) You venture out with friends and partners. This is the most complex of all. Some things start with a hobby and with no formal contract. If it becomes a success, interests clash once a while and if not resolved properly and quickly, this could be a disaster. As the person who delivered the code and brought the product to life, you might feel that you have the right to have it under your control. But, there are other aspects in which your partners might see it and from a totally different angle. While, it is very important to maintain the proper relationship with them, it is always good to have formal agreement about your interest or stake. It could be a simple agreement like you own the rights for specific parts of the software or the right to reuse it else where with proper agreement. There is nothing wrong in this agreement. So don't be afraid. Otherwise, be prepared to handle any issues that happen in future in a friendly way.

2.) Yes, you can definitely do it as long as you protect yourself with a contract. 
Otherwise, you will be at great risk. You might have seen this in a corporate world. Company A uses a product from Vendor V. Now, they wanted additional features and Vendor provides them cost to deliver the changes with Price 'P1'. However, they also provide another option with price 'P2', where in they will throw a clause that they will make the changes requested as a feature of their product. Both parties win in this case. When selling to Company B, Vendor can market about the new futures and might even sell for a higher price and Company A is getting the features for a lower cost. So again a formal contract will help you.

3.) If you do not intend to open source it or allow others to peek at it, please use a private repository on GitHub. No compromise here, please. Yes, you should talk to your client about it. The moment he realizes that his code is available for anyone to download it, I guess he will be ready to pay for it, but don't even bother taking that pain. Protect your IP rights. You can also get a VPS where you can manage your code using something like SVN as well.

Good Luck!




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
