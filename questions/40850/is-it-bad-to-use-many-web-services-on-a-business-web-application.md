## Is it bad to use many web services on a business web application

- posted by: [Derek](https://stackexchange.com/users/-1/18951-derek) on 2012-07-26
- tagged: `webservices`, `webdev`
- score: 0

I'm the sole developer on a web application project that a friend and I started up. I'm handling development and my friend is handling the business side. It's a guerrilla operation and with what our application is trying to achieve I could never develop it on my own in a reasonable time. So I'm planning on using many services to run the application. AppFog for hosting and deployment, MongoHQ for the database, Searchify for document indexing, Filepicker.io for file uploads, and AWS for misc utility needs. Besides the obvious worry about one of these companies going under, are there any other reasons why I should absolutely not be doing this?
I figure if our application actually takes off and we make any kind of revenue, at that point, I could then put resources into building solutions to take the place of different web services I'm currently using.


## Answer 40852

- posted by: [JJJ](https://stackexchange.com/users/-1/18911-jjj) on 2012-07-27
- score: 2

- If you're paying all the licenses and fees as you should be (and not breaking terms of service)...
- And you're not guaranteeing some sort of an up-time that's quite impossible to keep...
- And you have a backup plan should one of your main service providers goes under or changes terms that make it impossible for you to use...
- And you're aware of integration and update effort if you're relying on a large number of external services

then you should be OK.

I don't think using many services is bad in itself - it's neither productive nor reasonable to build everything by yourself. 


## Answer 41614

- posted by: [NW Architect](https://stackexchange.com/users/-1/19419-nw-architect) on 2012-08-26
- score: 0

You definitely want to leverage what is out there, but protect your core competencies. 

The earlier point about building in flexibility in case you need to swap providers is a very good one. In Object Oriented design, that is called an abstraction layer.  Your tech team should design for flexibility and anticipate swapping things out down the road.

Also consider how slow the site will load if the back end jumps off to half a dozen APIs spread out all over the cloud. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
