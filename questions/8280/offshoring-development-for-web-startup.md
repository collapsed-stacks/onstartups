## Offshoring development for web startup

- posted by: [William Lannen](https://stackexchange.com/users/-1/2174-william-lannen) on 2010-02-21
- tagged: `web`
- score: 7

I'm considering the option of employing a developer from oDesk to work on my web startup.  My rough plan would be:

 1. Write a detailed specification.
 2. Produce the design (in terms of class diagrams, etc, not visual design).
 3. Create the skeleton project (I'm going to be using Zend Framework).
 4. Setup the project in SVN and my continuous integration server (so that I can run automated checks on the quality of the code, upload to a staging server, etc, on each commit).
 5. Employ someone on oDesk to work on the project for 2 days per week. When they are not working on it, I would be doing as much as I can.

How concerned should I be with sharing the full idea/specification and (more importantly) the full source with someone that, initially at least, I cannot completely trust.

What options do I have to limit the risk? An obvious one would be not to expose the full source to them and instead simply give them individual tasks (i.e. create a Zend controller which does xxx, create a Zend form which looks like xxx). However this would increase the amount of integration I would need to do considerably so would not be ideal.




## Answer 8282

- posted by: [Tom](https://stackexchange.com/users/-1/2610-tom) on 2010-02-21
- score: 4

We did it with a very limited scope of work (non-critical tasks). It was quite ok. 

In your case you've listed your main concerns - trust and quality of work and monitoring. I would also add to the list cultural differences. 

I think it all boils down to a main question - how do you want to treat your offshore developer? As a potential future partner? As a cost efficient coder? If I were you I wouldn't disclose the full scope of your project but rather employ someone to work on a specific tasks. It's the only way to build trust and doesn't expose you to a significant risk. 

One more thing - good documentation is the key here. 

Good luck!

Tom


## Answer 8286

- posted by: [user2608](https://stackexchange.com/users/-1/2608-user2608) on 2010-02-21
- score: 3

<p>I think Documenation will take you long way. But building a good rap with them will take long way to. Integrate with the team, educatate the team the way u want them to work. Communication is key the more u talk to them the better. </p>

<p>Make deliverys small. Every 1 , 2 days they will keep on delivery something agile is best bet. Make u build process is CI that way u can find issue fast. Establish good process (Low level Design,Frameworks ,Code reviews , Automated Unit Testing etc..) will reduce lot of effort later. </p>

<p>About shareing the document, now all the compnies in the world have one or other form a global team. As long is it not core secrate you can share with the team. Not just the codeing, u can explore the options of QA as well. This is one good area you can offshore. If you are really serious go and meet them in person. </p>

<p>Some time back i came across this very good podcosts Worth listening
<a href="http://www.dotnetrocks.com/default.aspx?showNum=162" rel="nofollow">Steven Forte on outsourcing and globalization
</a></p>

<p>Good luck in finding right people</p>



## Answer 8456

- posted by: [Gary Valan](https://stackexchange.com/users/-1/2650-gary-valan) on 2010-02-24
- score: 0

Both answers before mine are very good, I'll add more on the business side:

1) Communication: make sure you speak the same language and within that be sure you understand each other. American style of communication is different than what is understood or used in various countries.

2) Qualification: ask for reference and follow up. There are experienced software professionals and there are basic coders who are ambitious but may not be able to deliver.
Also check up on their knowledge. if its web 2.0 type work, you need to find out what they know about latest techniques, dev packages etc unless you are willing to let them learn and iterate on your dime.

3) Payment: Don't make a big deposit. Ask for a bit of work upfront so that you can evaluate performance, trust building is important.

4) Deadlines: Very elastic in some countries.

5) Support: Timely bug fixes + updates should be in the contract for a fixed fee, not per hour.

6) NDA- not worth the paper or pixels its written on except if you are working with a large established company

7) Asymmetrical relationships: If you are a one/two man shop don't work with a mid sized or large company. Asymmetrical relationships don't work, you are a small fish in a large pond.

I lost my shirt so you don't have to...



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
