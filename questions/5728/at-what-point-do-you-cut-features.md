## At what point do you cut features?

- posted by: [Sam Saffron](https://stackexchange.com/users/-1/258-sam-saffron) on 2009-12-31
- tagged: `products`, `management`, `apps`
- score: 3

I have a couple of features in my product that are really important but, as it stands, are not fully implemented / designed or integrated. 

At what point do I remove them from the product? 

I know that this is a soft question so I will add a few parameters. 

- I would like to ship something to a customer in short order. 
- I am proud of my work, I dislike a disjoint user experience. At least a couple of months of refinement would be beneficial to the product.
- One of the features is critical to the user experience. 

Do you ever ship a product with half finished features?



## Answer 5738

- posted by: [Benjamin Wootton](https://stackexchange.com/users/-1/2094-benjamin-wootton) on 2009-12-31
- score: 5

I would always favor cutting features rather than delivering anything half finished.  Do one small thing very well and you can can always document upcoming features in your product roadmap and add them in over time.

Release early, release often, is an overused mantra, but still has lots of value in it.

One idea... have you considered a private beta program so you can start getting feedback early?








## Answer 5732

- posted by: [Jakob Buis](https://stackexchange.com/users/-1/2057-jakob-buis) on 2009-12-31
- score: 2

It depends on what "half finished" is. 

I worked on a private project just this week, that included a number of distinct features; and I faced the same question (even though it was a rather minor issue).

For example, one feature of the application worked perfectly. It's wizard that guided the user through entering some data and finally generating a PDF-file. Everything worked perfectly, all beautiful code with a fully AJAXified interface. One minor issue: the PDF contents were wrong. Because the PDF is the most important part of the feature, I didn't release it until I fixed the errors.

Another feature of the same application, maintains a members table. Ultimately, this table will contain 900+ entries, so speed and a handy interface are quite important. The feature currently has neither, but that isn't a problem: the table won't have more than 100 entries for another month. All required features (adding, removing and editing rows) work, so I released it.

My point: determine the minimum set your features must have to help your customer, built it and release. Keep improving and releasing them until they match your quality criteria.


## Answer 5737

- posted by: [Fernando Martins](https://stackexchange.com/users/-1/1778-fernando-martins) on 2009-12-31
- score: 0

Sam,
I've never shipped with half-finished features and I've cut features by looking at the the feature priority assigned to each feature in the requirement document.
Start by cutting the "nice to have", then the lowest and so on. 
This answers the question "what features to cut".

My answer to the question "when to cut features" is also simple. Do it when you have a dead-line that you cannot miss or you need to ship faster for any reason.
Obviously there is a balance between shipping and including "must-have" features, sometimes one really needs to delay the ship date in order to have a solid product.

My 2 cents for a solution to your problem is to check the feature priority on your requirement document and find a balance between the features and the ship date.
Maybe you can ship a simple version to comply with your customer dead-line date that suits him/her and later supply the full version.


## Answer 5744

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2009-12-31
- score: 0

From a business perspective, you want whatever you ship to your customers to be what they paid for. Releasing early is an OK strategy as long as you set the customers expectations. Benjamin had an excellent point about a private beta program. That is something to consider but more importantly, you don't want your customer to feel that they are getting a poor product.

My mantra on this is under commit and over deliver. Set expectations with your lead customers and then exceed them. If you have critical features, which to me means absolutely has to be in, then don't release. 

If you are worried about losing your customer, then go talk to them. Explain the situation and set expectations correctly. If you talk to your customers, then maybe that critical feature is not so critical.

The other side is why do you need to release early? Do you need the revenue or feedback?


## Answer 5749

- posted by: [Brian Swanson](https://stackexchange.com/users/-1/1150-brian-swanson) on 2009-12-31
- score: 0

What is the least number of features you need to make your Minimum Viable Product (MVP)?  Are the features you are considering cutting needed to make the MVP?

Talk to your customers, fund out what the minimum number of features they need to make your product useful to them.  That should be your feature-set for your first release.  You can always add more functionality later.  If you implement a way for releasing often (continuous deployment), then you can work on those features and get them to your customer(s) quickly.

The challenge with any feature is figuring out whether it's a feature the customer wants, or whether it's a feature we think they want.  Getting an MVP released to your customers will help you decide what your feature priorities should be.


## Answer 5770

- posted by: [Jeff](https://stackexchange.com/users/-1/876-jeff) on 2009-12-31
- score: 0

If you (And I am assuming you are in touch with users needs) are not comfortable with the product, and don't think the user will like it, don't ship it. It's very hard to undo a negative first impression of product. (Windows ME and Windows Vista come to mind as examples) 


## Answer 6378

- posted by: [Tristan St.](https://stackexchange.com/users/-1/2151-tristan-st) on 2010-01-12
- score: 0

I've got the same issue: I've got some really great stuff that are not always "finished enough" to put in a version I'm shipping to my users.  Some were just at the "idea" stage, others were partially implemented.

But I didn't "remove them from the product": I simply moved the ones that weren't 100% mandatory and that were slowing me too much to the TODO list for version 1.1.

From a more technical point of view: you say that they may not be fully implemented so I take it they're partially implemented.  Don't delete them, don't throw away that code: I've got several unit tests that are currently "ignored" for they capture correct behavior for features that aren't fully working yet.  But the tests are already in the project, so are the unfinished implementation and they're staying there.  I'm not throwing that away.

I'm simply de-activating these features as of now in the build that make it to the beta-testers.

So to answer your question "at what point did I remove them": I didn't remove them but put them aside when I approached the beta testing phase.  The product is already great and eases customers' pain so even tough I could keep making it better and better forever at one point I decided it was time to ship.

And who knows, maybe the features temporarily put aside will prove so great that they'll warrant a version 2.0 and 1.x customers may be happy paying an upgrade fee to get them in version 2.0 :)





## Answer 6426

- posted by: [ThomPete](https://stackexchange.com/users/-1/1186-thompete) on 2010-01-12
- score: 0

This essay talks about exactly that.
http://000fff.org/beyond-aesthetics-design-tips-for-startups/

Basically I use a hammer as an analogy.

The hammer has one fundamental job which is to help you hammer in nails. Everything else you put on that hammer are features that you can cut depending at what stage you are on.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
