## What are use-cases?

- posted by: [Sriram](https://stackexchange.com/users/-1/8849-sriram) on 2011-07-30
- tagged: `project-planning`, `clients`, `presentation`
- score: 0

The startup I work for got asked by some potential clients to send them use cases. We are in the process of making one and I would like to ask the following questions about use-cases in general:  

1. What is it all about? I know that it details the steps between user and use-of-product (from Wikipedia).
2. Is it the final stage before a client accepts/orders the product?  
3. How verbose can it be? Or should it follow visual design principles (as in all information should be visual and easy to read and understand?  
4. Should it also include sections on the company goal, mission etc.? Is that overkill?  

I have read the wikipedia page on this which contains a specific use case for a software product. Here, though what we are selling is some software, it needs to go to a company that will in turn sell it to the masses.  

Any help on this is most welcome. 


## Answer 28123

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-07-30
- score: 4

<p>A "use case" can be visualized with a UML diagram. UML is an approach to describe technical software. You don't need to learn UML, don't be worried. The use case diagram is the most simplest diagram you can have. It looks a bit like a mind map.</p>

<p>Before you start, I would recommend you to use some a uml editor. One I love very much is Violet:
   - <a href="http://alexdp.free.fr/violetumleditor/page.php?id=en:installation" rel="nofollow">http://alexdp.free.fr/violetumleditor/page.php?id=en:installation</a></p>

<p>It is free of charge, has a beauty interface and is easy to use. On the other hand it lacks some top-pro features, but they don't touch you. Use case diagrams are complete. So, below you see a simple use case diagram made with Violet (image taken from product homepage):</p>

<p><img src="http://i.stack.imgur.com/7tX9Y.jpg" alt="enter image description here"></p>

<p>A use case is basically describing "what one can do with the software". Some elder people simple "feature" to it. Lets summarize a few use cases for a calendar software. First, you need to identify the actors. Actors can be human people or other systems. In our case we can say "Administrator", "User", "System". The last one is there for some clean up tasks. The first two are humans. Of course, a Administrator can be a User at the same time, but this does not reflect on the UML, except you have a button like "Make this user an Admin". The roles or Actors we identified are the human symbols on the screenshot.</p>

<p>Now the elipse are the use cases. We could draw one and write "Login" into it. The Administrator can login, the User can. The System cannot. This use case is not for it. So we draw lines from Admin and User to "Login".</p>

<p>Same goes for logoff. We could again draw a elipse with logoff and make some lines to it. But it would be better and more readable if we create an elipse "Authorization" and put the "logoff" and "login" elipse as a sub use case to "Authorization". Then we only need to draw lines from Admin and User to "Authorization", and "Authorization" has lines to "Logoff" and "Login".</p>

<p>Guess the principle is clear now.</p>

<p>The calendar can have more use cases:</p>

<pre><code>Calendar --&gt; Add entry
         --&gt; Delete entry
         --&gt; Show as month view
         --&gt; show as daily view
Profile  --&gt; Modify timezone
         --&gt; Reset password
</code></pre>

<p>Here are some of the Systems use cases:</p>

<pre><code>Cleanup users who have not activate account
Cleanup entries who are older than 1 year
</code></pre>

<p>And so on. </p>

<p>To your question 2), it is not the final stage (usually). If you have agreed on which use cases you implement, you probably must estimate how long it would take. probably they want to see other more fine diagrams or at least some wireframes were they can they how you have planned the software.</p>

<p>To 3) I would recommend you to note down everything "one can do with the software". But not company goals, mission or something. Show every feature the software will have and organize them nicely. This will show your understanding of modules of the product and show that you have not forgotten a desired feature. And, you can make a better estimation.</p>

<p>To 4) As already mentioned: no. </p>

<p>I have made the experience that it is very helpful to make comments into the diagram. In addition I always give the use cases IDs to identify them uniquely. On the phone we can find the discussed use case better. </p>

<p>In addition a small document, listing the use cases with id and name is very good. It should include </p>

<ul>
<li>a small description of the use case in words</li>
<li>necessary data to perform it (like for Login: "Username" (String, max 30 chars), "Password (String, max 30 chars))</li>
<li>expected outcome of the Usecase (User is logged in and can perform all other use cases, Time entry has been stored in the database)</li>
<li>Other comments (risks, for example System is deleting something a user currently views or some words on complicated tasks)</li>
</ul>

<p>Finally include a small description of your actors, who can be a user, who is an admin.</p>

<p>My guess is, you need half of a page per use case.</p>

<p>Last tip, don't put "future" use cases in your diagram. Make a "version 1" use case diagram, and if you know already about version 2, make a second diagram extending the first one. If you show one single diagram with 1000 use cases - everybody knows it will take forever to implement it. Make smaller steps, so you can show how the software grows during the time.</p>

<p>Hope the helps a bit!</p>

<p>Cheers,
Christian</p>



## Answer 28150

- posted by: [Bob Murphy](https://stackexchange.com/users/-1/5778-bob-murphy) on 2011-07-30
- score: 4

>[W]hat we are selling is some software... to a company that will in turn sell it to the masses.

That's a reseller. Unless they're super-technical and plan to integrate your software with an existing software product of theirs, they almost certainly don't want UML diagrams. What they probably mean by "use cases" is some examples of who might use your software and why. That will help them to evaluate whether they want to resell your software, and who they might sell it to.

You can often write those kinds of use cases as stories. For instance, "Laura works as an A at a company that does B. C and D happened at work, and that caused a problem because of E. Laura bought our software product F, and did G with it. That not only solved the problem, but made her division $H in extra profit that month.



## Answer 28141

- posted by: [Jordi Cabot](https://stackexchange.com/users/-1/12150-jordi-cabot) on 2011-07-30
- score: 3

In a more general sense, use cases are application scenarios that highlight the value/benefits of your software. I'm not sure your clients meant to get a list of UML use cases or just a more description of possible scenarios where the software would be useful for them 


## Answer 28196

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-08-01
- score: 3

<p>Technically, a 'use case' is an answer to the question: <em>who</em> is going to do <em>what</em> with a system, and <em>why</em>? </p>

<p>This is a richer framework than the traditional attempt to define business needs, which then gives rise to functional requirements. (Or more often in real world situations, to identify business needs and attempt to map them to functional characteristics of existing systems.) The additional richness comes from those two dimensions of <em>identity</em> (who are the 'actors'), and <em>purpose</em> (what are the 'goals').</p>

<p>So if you're being asked the question in that technical sense, you will certainly want to familiarise yourself with the terminology and visualisation of <a href="http://en.wikipedia.org/wiki/Use_case_diagram" rel="nofollow">the use case diagram</a>.</p>

<p><strong>But...</strong></p>

<p>This term has also slipped out into the wider world, where "show me your use cases" means something more like one of these questions: </p>

<ul>
<li>What are the situations where your product is the best way of accomplishing my goals?</li>
<li>What's the area where your skills are most relevant to my business?</li>
</ul>

<p>My guess is that the question in your case was probably in the latter category, so that the best way of answering it is much more about succinctly positioning your product or skill set into your prospective client's business context.</p>



## Answer 28367

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2011-08-05
- score: 1

There are some excellent answers here, but this seems too long for a comment.

You need to find a way to talk to them and check what actually want. I don't think it's detailed UML diagrams.

A Use Case helps the designers and potential users understand the purpose of the system and how tasks will be accomplished. If a reseller is asking this question, it could mean that they don't quite understand what the software does, what need it fills, and by extension who will buy it.

Consider a use case for the new-fangled telephone:

 1. Alice needs to ask Bob what time he will be home.
 2. Alice picks up the telephone "receiver". (see diagram)
 3. Alice listens for a continuous purring sound in the receiver.
 4. Alice presses the keys on the base unit for the unique number Bob has given her.
 5. She hears an intermittent purring sound.
 6. Bob hears a ringing sound from a bell inside the base unit of his telephone.
 7. Bob ... etc.

Notice how it is made clear what the purpose of the interaction is (Alice wishing to communicate with Bob) and the steps the user performs in order to achieve that purpose. At the end of this we have a very clear idea of the expected interactions between Alice, Bob, and the telephones. But nowhere is it specified how the new-fangled telephone works its magic. 

For reseller purposes the interaction would be described at a higher level, and might describe what the software does to external entities ("the system updates the database file to remove duplicates") 

For design purposes you might include obscure error conditions: *for sales purposes it is more likely that they are just after several typical usage scenarios that their salesmen can understand*:

 1. "Bob wishes to reduce staffing costs by 10%. 
 2. He selects *reduce staffing costs* from the main menu and selects the reduction required in the resulting dialog and clicks OK. 
 3. A homicidal robot is unleashed by the system. The number of staff on the payroll is automatically reduced by 10% ..."





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
