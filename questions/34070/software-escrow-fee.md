## Software Escrow Fee

- posted by: [jazar](https://stackexchange.com/users/-1/6750-jazar) on 2011-12-23
- tagged: `business`
- score: 3

Does anyone familiar with software (source code) escrow service, since I having some questions about this service?
1. How much this service will costs me ? Assuming I just have one beneficiary.
2. Is there any potential trap/pitfall for me as the source code owner that will be made by other party to acquire source code 'cheaply' by asking me to put the source code into escrow service.
3. Any recommended & affordable escrow service?



## Answer 34086

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2011-12-23
- score: 4

Software escrow is something that has been around for many-many years. It is usually used when a big company is licensing mission critical software from a small company and is concerned that the small company might go out of business (or the sole proprietor might get hit by a bus). 

The easiest way to satisfy the big company would be to simply license the source code to them and thus they would have a copy. There are times however when the small company considers the risk too great or is unwilling to do so and thus would prefer to incur the cost of using a third party escrow service that is trusted by both parties.

The way this works is that the software company gives a copy of the code to the escrow service and periodically also sends them any updates that are made. If all the service did was store some DVDs in a box, this would be easy and cheap. The issue for the big company is how do they know that the DVDs really contain the source code and not something else? This is an issue of trust, if the small company trusted the big company they would have simply given the big company a DVD to be opened "in case of emergency" only.

Since the small company does not trust the big company, it is unlikely that the big company will accept "trust us, the DVD contains the latest source code and all documentation" from the small company. Now here is where the big costs come in. The big company will want to have the escrow service quality assure the source code. In other words they will want the escrow service to take the DVD, compile the source code and verify that the program runs just like the executable (binary) file that the big company received from the small company. Further every time there is a change they will want the change verified as well.

From the point of view of the small company (the developer) they will need to trust the people at the escrow service. If you didn't trust the big company with the source code, why do you trust the people at the escrow service? That is why you need to find one that both companies can trust.

As you can see, to do this properly can be quite costly. This is a cost that should be paid by the big company and negotiated as part of the contract. Needless to say that the money they spend on the service will be money that they will not be going into your pocket.

You may very well find that it would have been much better for you to have simply licensed them a copy of the source code to begin with.

That having been said, escrow of source code is a well proven and accepted practice where major deals are concerned. If it is a multimillion dollar project then 10 or 20 thousand for escrow may be cheap insurance. 





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
