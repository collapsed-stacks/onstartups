## Do 2 Part time Developers = 1 full time developer?

- posted by: [iScotts](https://stackexchange.com/users/-1/10904-iscotts) on 2012-06-01
- tagged: `co-founder`, `development`, `open-source`
- score: 1

If I could partner with 2 or more part time developers, would this be enough and as good as having a full time developer? Eg 4 part time developers = 2 full time developers? 

I am basing this on the idea of open source development. I am guessing all the developers are part time and some of the things they develop are very good. So am I correct in my logic here? I just need some clarification.


## Answer 39595

- posted by: [Keith DeLong](https://stackexchange.com/users/-1/888-keith-delong) on 2012-06-01
- score: 7

There's been a ton of research and writing in this area. It's been pretty clearly demonstrated that there is a geometric complexity in the relationships between developers. This means that a second developer's productivity may well not be simply additive in terms of raw productive output and multiple developers will often actually reduce the overall productivity. 

Think in theses terms, two developers have to spend time creating as well as collaborating. Collaboration is often complicated in a creative process. There are other issues as well, but the point is to consider that there is a relational element in working together towards a single creative goal. This may well enhance the result but it often actually slows the process. 


## Answer 39570

- posted by: [Matthew Galloway](https://stackexchange.com/users/-1/15145-matthew-galloway) on 2012-06-01
- score: 4

Check out the mythical man month:
http://en.wikipedia.org/wiki/The_Mythical_Man-Month

Basically it talks about how 200 developers is quite possibly going to make it SLOWER than 100 developers rather than the "twice as fast" you might guess! (well, in the specific example of one which is running late but I think it can be generally have some other applications too here)

So, you're going to find there is a fair amount of duplication between the two (or more) developers. There is overhead too, making sure they don't step on each others toes etc. But good policy/practice such as using github and a wiki can partially reduce these negative side effects.

I'm sure you're aware of the saying "too many cooks spoil the broth", remember that.

My answer might not be too satisfactory as really "it depends". On the people, how you're doing it, and what the project is (some can easily be broken into little pieces to be shared about, others can not be. Oh, and of course the breaking it up and sharing it about is yet another overhead...).

Anyway, on the flip side now I've mentioned a few of the negatives I'll now mention a positive:

Several people are sure to have a greater range of a talents than one person will have (for instance if game programming, one guy might be good at AI/Graphics/Sound while the other is good at Physics/Graphics/Networking. Together they're much better than they are apart). Also, even IF they have exactly the same range of talents there is benefits to have a fresh pair of eyes they can call upon if they get stuck.

In conclusion, where N is the number of (part time) developers then for small N it is likely to scale well (greater than linearly) but for large N it will scale less well (a lot less than linearly!).

I leave it as an exercise for the reader to calculate the optimal value of N! ;-)


## Answer 39571

- posted by: [user983248](https://stackexchange.com/users/-1/17900-user983248) on 2012-06-01
- score: 0

It depends on.

A: They are developing the same thing ?
B: They are developing different parts of the same thing ?
C: They are developing different stuff.

They all must be in perfect harmony and synchronization as well as having the same objectives and goals otherwise things can go wrong. Sometimes there is more than one way to achieve or develop something, and in these cases you need all your developers focused on the main goal and working together on a solution that makes everybody happy.

Having two part time developers is not equal to one full time as two heads think, argue and solve problems more efficiently than one.




## Answer 39599

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2012-06-01
- score: 0

Let's get some comon sense here. No, it wont work, AND YOU SHOULD KNOW. SImple maths.

THis is like saying "Two 2 3 seat cars have the same passenger capacity than a 4 seater" - no, because oyu need 2 drivers, instead of 1.

Basically the week has 40 hours, 2 devs are 2x20 hours. Everything which is a fixed administrative overhead (scrum meetings, planning) costs double. Communication between the 23 people costs more time than one person just doing. And that is why I say you sould know it - this is basic common sense.

But: YOu loose in the week let's say half an hour per day for planning meetings. THat is 2.5 hours for 1 developer, but 5 for 2. Same goes on with pretty much everything. So, the administrative losses are higher - simple like that. Also part time devs are not concentrating only on you - not saying they betray you, but when you do another project on the side, your mind is split.


## Answer 39601

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2012-06-01
- score: 0

Having two developers creates complexities that require additional time to resolve, depending on how you integrate the work they produce, just as writing/performing a speech or piece of music involves more complexity when more minds/voices are involved.

Every dev has his/her own coding habits and logical reasoning and if you have two of them work on the same project, they will have to spend time reviewing each others' code and likely run into conflicts that break the code. However, if you plan to have them work on relatively self-contained independent projects that takes a simple hook to integrate, then the two-developer arrangement might be more cost effective - but it's unlikely integration will be simple. It all depends on how much integration there needs to be for their work, and based on what you've presented, they will probably need a lot of integration.


## Answer 39605

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-06-01
- score: 0

In addition to some of the good answers, I would like to address the Open Source point.

Some of the huge Open Source project have people working who are paid for doing it. For example IBM pays some OpenOffice developers. Red Hat pays some JBoss developers.

Some companies have their business model upon OSS. They pay a few developers for writing the tool as Open Source, and then send out tons of consultants to help their users (paid of course). Phonegap for example has paid devs (paid from Adobe) and it seems they want ot make money with "phonegap build".

Of course there are many unpaid open source devs out there. For example Apache log4j or Apache Struts or (meanwhile) Apache Cocoon are fully unpaid projects. People are all volunteers. While software is good, it takes a good amount of time. Sometimes it takes weeks before a commit comes into the repository. Sometimes not. It depends on how much time is on the weekend. On the other hand they safe time because in the OSS world usually there are not so many limitations: there is no marketing, no distributor, no boss etc. 

After all 2 OSS devs are clearly better than one from quality perspective. I say only peer review and motivation. Don't expect something to happen "quick" - and this is, what you need when writing proprietary software. Here 1 dev can make decisions quicker than 2 halftime devs.


## Answer 39670

- posted by: [Anurag](https://stackexchange.com/users/-1/4475-anurag) on 2012-06-04
- score: 0

No.
Depends on how you structure the development,project management is the key.


## Answer 39569

- posted by: [Nick Stevens](https://stackexchange.com/users/-1/15902-nick-stevens) on 2012-06-01
- score: -2

Theoretically 8 hours of development time is 8 hours of development time, regardless whether it's 1 person or 8 people.

That said - you need to take into account handover/catchup and communication time. 
You can minimise/delay this a bit by ensuring that you have good developers and that each developer is working on different tasks, but sooner or later they're going to need to communicate.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
