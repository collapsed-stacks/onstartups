## Is there any issue if my service APIs are very similar to my competitors

- posted by: [Steve](https://stackexchange.com/users/-1/10240-steve) on 2011-05-04
- tagged: `intellectual-property`, `api`
- score: 3

We have a web service and offer APIs for customers to integrate and create other customizations. Since following ReSTful design, we found our design eventually are so much alike our competitors. If we use different verbs, it will make the API methods quite long and not intuitive. All the CRUD operations are almost same. Before we release the APIs, we'd like to make sure there's no issues for us using the exact same http API methods. Please kindly advise. Many thanks!


## Answer 24435

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-05-04
- score: 3

The only potential claim by your competitor I could see would be a copyright claim.  There is probably weak, if any, copyright protection to API names, but an aggressive or pissed off competitor could conceivably make it.

Your worst case scenario would be if your competitor's API had distinctive method names, e.g, `doZingGaBang()`, and you copied them.  My understanding is that this is not the case here.

If your competitor's method names are common things like `init`, `put`, `get`, etc., and you copied his entire API exactly, including argument lists, then there is a potential risk that he could make a claim for copyright infringement (albeit a weak one).

If your competitor's method names are common things like `init`, `put`, `get`, etc., and by coincidence some of these are the same as yours, then you have nothing to worry about.  Where it is easy to do so, you might as well make your API different from your competitor's, but your competitor does not have a monopoly on common words to describe common operations.


## Answer 24486

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-05-05
- score: 1

Something to bare in mind by it's very nature your API is going to be similar to your competitors. You are both writing your API in a RESTful way, you both are going to have similar functionality. Presumably their are some differences, and as you are not first to market you have the advantage of being able to see what is working and what does not for your competitor.

Also having a similar (though hopefully better) API to your competitors also will make life easier for the person integrating especially if they have to deal with both yours and your competitors API. The worst case scenario for you is if you decide to abandon or modify your RESTful design and create a confusing mess for developers, especially if the developers then turn to your competitor.

Use similarity to your advantage, emphasis the differences and learn from your competitors API to enhance your own. Follow common design methodology and you will be fine. Though I am not a lawyer though I do work with and design APIs for a living.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
