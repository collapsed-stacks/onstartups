## How to split up backend development?

- posted by: [JDH](https://stackexchange.com/users/-1/13136-jdh) on 2011-10-08
- tagged: `webdev`
- score: 0

My design & front end development is finished, and it is time to do things like add shopping cart, registration, and connect to database. I have read that it is safest to give the programmer only access to SOME of the files during development, to both protect your idea, and ensure that if the relationship doesn't work out, you can quickly hire someone else. My main question is how do I figure out *which* pages I send to the programmer, to work on specific features. For example, let's say it's time to create the user registration process. I send specs for what I want done, along with the html/css/js/etc files that are completed, and he works his magic. But how do I know that I've sent all the files that are needed for that particular process. I hope this question makes sense. Please don't just say "You'll have to talk to your developer." I understand that I will, but I want to get some basic knowledge about this first so I can do this the smartest way possible. Thank you very much. 


## Answer 31188

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2011-10-08
- score: 1

I think you have 2 options:

1. Develop the front end against a specification so that you can then get the developer to work straight from the specification (they won't need the front end if the specification is accurate). Effectively they don't care about the front end, and the front end doesn't care about the back end, they both just need to have the interaction specified (methods, parameters, etc.).

2. Get a developer that you trust and give them the whole lot to work with. If you need to, get them to sign some non disclosure/compete contracts.

I would go with #2, the extra work with #1 would be a large overhead, and if you get a developer with references then you should have enough confidence in them.

Number 1 would also likely require someone to tidy the integration when the backend is done (probably a developer type), as things will not all be right.


## Answer 31192

- posted by: [Alex](https://stackexchange.com/users/-1/12744-alex) on 2011-10-08
- score: 1

I've never encountered a situation where it's a good idea to restrict access for your developer. I don't see how it would protect your idea, or how it would help with hiring someone else. 

Would you need to turn over your documentation on your super-secret IP if it doesn't relate to the work he would be doing? No, of course not, but the developer will certainly need things relating to your project in order to do his job--it's better to give him everything from the start to make life easier for the both of you. The alternative is that stuff will likely be missed or left out, leading to a long drawn out back-and-forth between you and the developer.

If it comes down to trust issues: I'd suggest doing as much legwork as possible to find a solid developer, turn your business specifications over to them, and then say 'this is what I want.' For a lot of businesses, especially when the owner doesn't have a strong technical background, this can be the best route to take.


## Answer 31260

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-10-10
- score: 0

You hire established professionals who prefer not to lose their reputation by stealing a client's idea. 

You may not want the developer to have access to your live website (protect client data?), but you can give them files to create their own development site. Better yet, you should create a staging site for testing and give them access to that. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
