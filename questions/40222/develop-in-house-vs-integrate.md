## Develop in House vs Integrate

- posted by: [Yehia A.Salam](https://stackexchange.com/users/-1/18565-yehia-a-salam) on 2012-06-27
- tagged: `api`, `core-values`
- score: 6

We're working on a mobile application that provides location based services like cinemas nearby, places, events and deals. I need to decide from now and then, **whether to integrate with an API to provide the location based service or to develop one on our own**. 

For example take the events service, I can already integrate with another company or develop it in-house but I'm afraid if I integrate everything the application won't have any value as I don't own the data so I can't count the data as one of my core assets.

Knowing that the development costs and the reliability of the 3rd party integration is not an issue, what do you suggest in this case?


## Answer 40223

- posted by: [Michael](https://stackexchange.com/users/-1/17905-michael) on 2012-06-27
- score: 6

Where would "your" data come from, if you do not integrate an existing API? You will either have to have user generated content or have to add the content on your own (or buy it).

If users should create it, then answer yourself the question why users would do that on your site/with your app and not on the already existing ones.

Furthermore, what are the USPs of your service? Is it a great app that aggregates content from multiple providers (APIs) and combines and present it nicely or is it more the great content itself? What do you want to be "famous" for?

If you can answer those questions, answering the above question yourself will be a lot easier!


## Answer 40232

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2012-06-27
- score: 1

Integrate gets my vote. The data collection is a solved problem by companies that have much larger pockets than yours and the chance of you being bought because of it is fairly low. 

You might find "value add" by having 

- A user base that is a specific demographic, thus advertisers know who they are targeting.
- A large user base that a buyer wants to aquire 
- Additional details over the already collected data. If smaller stores/coffee shops can have conversations with their customers through your app, eg. make bookings, offer discounts to proven regulars, say thanks to individuals for dropping in etc then your new data is probably more valuable than simply where the shop is.




## Answer 40231

- posted by: [JohnZ](https://stackexchange.com/users/-1/18439-johnz) on 2012-06-27
- score: 0

You have to start somewhere. 

As Michael mentioned, if you don't use other people's data, you'll have to create it yourself (lots of work), or have your users create it (why should they use a service with no data?).  

My advice is integrate third party tools when convenient to reduce your development time.  The value you provide might come from aggregating the data from multiple services, like Kayak does. It might come from adding data on top of a third party's data, such as housingmaps.com for Craig's List.  It might be your value proposition evolves over time.

Good luck!


## Answer 40289

- posted by: [saurabhj](https://stackexchange.com/users/-1/17589-saurabhj) on 2012-07-02
- score: 0

I feel it "depends" on what you are going after.

Is **data** going to be your unique selling point? This could be true in regions or places where data is not easily and reliably available. In that case, you could grow your own data (which as John mentioned is a lot of work).
It could also be that data is so expensive that you cannot afford to buy / license it - in that case, you will need to focus on getting the data yourself and perhaps sell it later as a licensed service?

If your service and its features form the core-engagement for your application, and data is easily and reliably available along with it being decently affordable, I'd say go for licensing it.

Companies which provide such data have based their entire business around doing just this and are more often than not good at what they do. If data is not your **core-business**, you should leave it to the experts even if it is slightly expensive sometimes as it will give you tonnes of time to focus on things that really matter - which is your site & service.

All the best!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
