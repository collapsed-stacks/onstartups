## Should we charge the client for fixing bugs?

- posted by: [Contrazoom](https://stackexchange.com/users/-1/21821-contrazoom) on 2013-10-28
- tagged: `contract`, `customers`, `billing`, `clients`, `client`
- score: 8

<p>Our small firm provides custom web application services.  We always charge on a time-and-materials basis - we simply give an estimate up front and then charge for actual hours used.</p>

<p>One of our clients has a cloud app that is growing more complex as time passes.  They hammer us with emails every single day, asking for changes and new features - some small, some large.  There is no batching any of these things as a single project - it's just a constant daily flood of random change requests and shifting requirements, with many of their emails labeled as "URGENT!!!!".</p>

<p>Although we do some pretty intensive unit and user testing before deploying changes to their live site, bugs do sometimes slip through.  We fix them promptly.  The problem is that the client is now freaking out because we bill them for time spent fixing bugs that have made it onto the live site.  </p>

<p>Their position is that they have already paid for the hours it took to develop the feature, and that we should warranty it.  Our position is that we simply charge for the time we spend developing, and make no distinction between new development and bug fixing.  It's all just time to us, and we have not built anything into the original development cost that would cover warranty fixes.</p>

<p>How do I solve this in a way that both makes the client happy and protects our financial solvency?</p>



## Answer 51558

- posted by: [TS Haines](https://stackexchange.com/users/-1/28021-ts-haines) on 2013-10-28
- score: 9

<p>From an ethical standpoint, I'd side with the client - if you deliver buggy software that the client has paid for and originally-contracted requirements are not being met, that's on you to make it right. Legally, it depends what your contract states. </p>

<p>But I will point out that your contracting method puts all the risk on the client:</p>

<blockquote>
  <p>we simply give an estimate up front and then charge for actual hours
  used</p>
</blockquote>

<p>So the client should understand they are carrying all the risk, especially if they are mixing bug and new feature requests.  </p>

<p>A formal contracting agreement would specify acceptance criteria up front in the form of test cases or whatnot.  The client would then sign-off on everything when you deliver and that's that. It's up to you what and how you want to warranty (and write into the contract).  If you can sell the client on a maintenance contract, which may look like "$X per year, which includes up to Y hours of work", all the better.  </p>

<p>It sounds like you have a very loose agreement with this client that could benefit from some more formalities in order to protect both sides. Both sides reduce uncertainty, which is what it sounds like you are looking for. </p>



## Answer 51560

- posted by: [DataSmarter](https://stackexchange.com/users/-1/27274-datasmarter) on 2013-10-29
- score: 3

<p>As you say that it's mainly the case for one specific client, I can give you an indirect advice:</p>

<p>You should read the "<em>4 hours Working Week</em>" book of Tim Ferris - especially the section about <strong>using the Pareto law (80/20) to the client segmentation</strong>.</p>

<p>In short: it says that <strong>20% of clients are causing 80% of your troubles</strong>. And the solution might be to get rid of these 20% of "difficult" clients. <strong>There are clients that simply doesn't worth to be served (economically speaking).</strong></p>

<p>Put on balance the amount of worries this client causes you (organization of your work, demotivation of the programmers, time loss...) and the income he generates. Does it worth the pain?</p>

<p><strong>Talk to him, explain him that such a way of working is not suitable. Or he become more realistic in the requirements, or you charge him more, or there are other clients waiting to do business with you...</strong></p>

<p>I don't know if it is a substantial client to your company <strong>but maybe getting rid of him could free time and means to permit you to serve other - more profitable (and perhaps "easier") -  clients.</strong> </p>



## Answer 51559

- posted by: [RhysW](https://stackexchange.com/users/-1/28409-rhysw) on 2013-10-29
- score: 2

<p>Yes. It is impossible to write software that doesn't have bugs. You should always strive to deliver it with as few as possible but 0 bugs in new software isn't feasible.</p>

<p><strong>Meet in the middle</strong></p>

<p>A method you might be interested in doing is a way of 'meeting in the middle' with your client. </p>

<p>Make sure future contracts clearly state that initial development will be charged at £X per hour and that future bug fixes will be charged at £Y per hour (Y is usually a reduced rate between 50% and 75% of X)</p>

<p><strong>Contract</strong></p>

<p>When drawing up your contracts agree on what is to be delivered. What features it should have ect. Then stick to it. If they want to change the requirements once it is signed then they need to raise a change request. Which costs extra accordingly. </p>

<p>Then you need to make sure that the software you deliver has all of the agreed features. </p>

<p><strong>Learn the difference between Change and Bug</strong></p>

<p>A change is when they want something new that deviates from the agreed contract, a bug is something in the agreed contract that doesn't have correct functionality as specified by the contract. </p>

<p>Changes should each come with a new signed contract agreed on by both parties and should be charged full rate. </p>

<p>Bugs should be charged at the Y rate,  depending on what that is for your company. </p>

<p><strong>How does all this help?</strong></p>

<p>First of all it bring about structure and order, very important things to have in an agreement between both parties. </p>

<p>Secondly it makes it harder for them to raise changes willy nilly without grouping or structure, it makes they have to think about what they want and cannot demand it. You should find overall that this helps you write better software as each group of changes can be estimated, designed and delivered at once. </p>

<p>This stops discrepancies over charges. Once it is in the agreed contract you need to be firm, if you let people walk all over you they can and will!</p>

<p>Overall these points should help you bring about structure in future agreements. If you can get this process in place for your existing client then even better! Good luck!</p>



## Answer 51627

- posted by: [David Silva Smith](https://stackexchange.com/users/-1/6292-david-silva-smith) on 2013-11-04
- score: 1

<p>Charge clients for bugs and explain upfront that the clients will be charged for bugs.</p>

<p>I've worked for two software consultancies and now I own my own software consultancy. As you said to be financially solvent you need to bill the client for bugs. This is standard practice and I expect your client will have a hard time finding quality software companies that don't charge for bug fixes.</p>

<p>The process I follow is to generate an estimate of hours when work is requested. I give a low and high figure so the client has an idea the range the final amount will be in. As the project progresses I keep the client informed about where we stand regarding the budget. If I see a chance we are going to exceed the budget I would let the client know as soon as possible and give them options for staying within budget, probably by reducing scope. However by doing a good job with the high / low estimate I have been able to deliver projects under budget.</p>



## Answer 51606

- posted by: [Gavin Coates](https://stackexchange.com/users/-1/23633-gavin-coates) on 2013-11-01
- score: 0

<p>I think the first thing you need to do is take steps to address the bug issue. It is too easy in software engineering to take the a dismissive attitude and shrug it all off while saying "bugs happen". They shouldn't(1). </p>

<p>Bugs are bad for business. They are bad for your business as they create the situation you are in at the moment. They are even worse for your client, who might potentially be losing revenue due to the bugs in the system.</p>

<p>Your first step should be to look at the type of bugs that are being created, and look at how these can be addressed. Are the specifications not sufficient? Do you not have an accurate test environment? Do you not have sufficient time to complete a full test cycle on these changes?</p>

<p>Once you have identified the cause of most of the bugs, you can then return to your client and discuss ways of dealing with the problem.</p>

<p>From the sound of it, you are being paid for the time spent developing, and do not seem to have a formal contract. Speak to the client, show them you are serious about preventing the errors from occurring in the first place, and explain your findings on how you plan to do this. In most case the remedial actions will involve taking a longer time over each change request the client makes. Make this clear to the client, and come to a formal agreement on how you will deal with each change request, and on how you will deal with fixing errors in the system.</p>

<p>As in many cases, there is no right and wrong way of doing this, it all comes down to what has been agreed between each parties. That is why contracts are so key, and lawyers earn so much money. Remember that the contract is there to clarify the demands placed on each side, not to win favour for one side over the other.</p>

<p>(1) Ok, so bugs WILL happen, but you should be taking every step possible to ensure the system is as bug-free as is feasible.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
