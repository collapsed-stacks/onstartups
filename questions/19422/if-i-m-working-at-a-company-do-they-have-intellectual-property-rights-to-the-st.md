## If I'm working at a company, do they have intellectual property rights to the stuff I do in my spare time?

- posted by: [John](https://stackexchange.com/users/-1/6839-john) on 2011-01-26
- tagged: `employees`, `intellectual-property`
- score: 328

I was interviewed by a lady from Zynga and she told me that Zynga doesn't allow developers to have side projects.  Is this true for companies in general, or just a minority that Zynga is a part of?  Is this sort of restriction legally enforceable?  I'm in California, for what it's worth.


## Answer 20136

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2011-02-12
- score: 352

<p>The original question was "whether employees are allowed to have side projects." I assume this was just an oversimplification or a misunderstanding by the "lady from Zynga," because I doubt they care if you <em>have</em> side projects... the real question is whether they claim to <em>own</em> what you do in your spare time.</p>

<p>Before I start: Be careful before taking legal advice from this thread. I see enough wrong information here that you could get in trouble.  Non-US readers should also be aware that the law and legal practice could be completely different in their country.</p>

<p>There are two pieces of information you would need to know to answer this question: </p>

<ol>
<li><p>what state (or country) you are employed in?</p>

<p>There are state laws that vary from state to state which may even override specific contracts (<a href="http://answers.onstartups.com/questions/19422/if-im-working-at-a-company-do-they-have-intellectual-property-rights-to-the-stu/20126#20126">tghw covers those well</a>).</p></li>
<li><p>what does <em>your</em> contract with your employer say?</p>

<p>In the US, in general, courts are very lenient about letting people sign any kind of contract they want, but sometimes, state laws will specifically say "even if you sign such and such a contract, the law overrides."</p></li>
</ol>

<p>Before I can even begin to explain these issues, we gotta break it down.</p>

<p>Imagine that you start a software company. You need a programmer. So you hire Joe from across the street and make a deal whereby you will pay him $20 per hour and he will write lines of code for your software product. He writes the code, you pay him the $20/hour, and all is well. Right?</p>

<p>Well... maybe. In the United States, Joe still owns the copyright on that work. That is kind of weird, because you might say, "Well, I paid him for it." It sounds weird but it is the default way copyright works. In fact, if you hire a photographer to take pictures for your wedding, you own the copies of the pictures that he gives you, but he still owns the <em>copyright</em> and has the legal monopoly on making copies of those pictures. Same applies to code.</p>

<p><em>Every</em> software company is going to want to own the copyright to the code that its employees write for them, so <em>no</em> software company can accept the "default" way the law works. That is why <em>all</em> software companies that are well managed will require <em>all</em> programmers, at the very least, to sign an agreement that says, at the very least, that</p>

<ul>
<li>in exchange for receiving a salary</li>
<li>the programmer agrees to assign (give) the copyright to the company.</li>
</ul>

<p>This agreement can happen in the employment contract or in a separate "Proprietary Invention Assignment" contract. The way it is often expressed is by using the legal phrase <a href="http://en.wikipedia.org/wiki/Work_for_hire">work for hire</a>, which means "in this case we have decided that the copyright will be owned by the company, not the employee."</p>

<p>Now, we still haven't said anything about spare time work yet. Suppose, now, you have a little game company. Instead of making software, you knock out three or four clever games every few months. You can't invent all the games yourself. So you go out and hire a game designer to invent games. You are going to pay the game designer $6,000 a month to invent new games. Those games will be clever and novel. They are patentable. It is important to you, as a company, to own the <em>patents</em> on the games.</p>

<p>Your game designer works for a year and invents 7 games. At the end of the year, he sues you, claiming that he owns 4 of them, because those particular games were invented between 5pm and 9am, when he wasn't on duty.</p>

<p>Ooops. That's not what you meant. You wanted to pay him for <em>all</em> the games that he invents, and you recognize that the actual <em>process of invention</em> for which you are paying for him may happen at any time... on weekdays, weekends, in the office, in the cubicle, at home, in the shower, climbing a mountain on vacation. </p>

<p>So before you hire this guy, you agree, "hey listen, I know that inventing happens all the time, and it's impossible to prove whether you invented something while you were sitting in the chair I supplied in the cubicle I supplied or not. I don't just want to buy your 9-5 inventions. I want them all, and I'm going to pay you a nice salary to get them all," and he agrees to that, so now you want to sign something that says that <em>all</em> his inventions belong to the company as long as he is employed by the company.</p>

<p>This is where we are by default. This is the <em>standard</em> employment contract for programmers, inventors, and researchers.</p>

<p>Even if a company decided, "oh gosh, we don't want to own the 5pm - 9am inventions," they would soon get into trouble. Why? Because they might try to take an investment, and the investor would say, "prove to me that you're not going to get sued by some disgruntled ex-employee who claims to have invented the things that you're selling." The company wants to be able to pull out a list of all current and past employees, and show a contract from <em>every single one of them</em> assigning inventions to the company. This is expected as a part of due diligence in every single high tech financing, merger, and acquisition, so a software company that isn't careful about getting these assignments is going to have trouble getting financed, or merging, or being acquired, and that ONE GUY from 1998 who didn't sign the agreement is going to be a real jerk about signing it now, because he knows that he's personally holding up a $350,000,000 acquisition and he can demand a lot of money to sign.</p>

<p>So... every software company <em>tries</em> to own <em>everything</em> that its employees do on paper. (They don't <em>necessarily</em> enforce it in cases of unrelated hobby projects, but on paper, they probably can.)</p>

<p>Software developers, as you can tell from this thread, found this situation to be upsetting. They always imagined that they should be able to sit in their own room at night on their own computer writing their own code for their own purposes and own the copyright and patents. So along came state legislators, in certain states (like California) but not others (not New York, for example). These state legislatures usually passed laws that said something like this:</p>

<ul>
<li>Anything you do on your own time, with your own equipment, that is not related to your employer's line of work is yours, even if the contract you signed says otherwise.</li>
</ul>

<p>Because this is the law of California, this particular clause is built into the standard Nolo contract and most of the standard contracts that California law firms give their software company clients, so programmers all over the country might well have this in their contract even if their state doesn't require it.</p>

<p>Let's look at that closely. </p>

<p><em>On your own time.</em> Easy to determine, I imagine. </p>

<p><em>With your own equipment.</em> Trivial to determine. </p>

<p><em>Not related to your employer's line of work.</em> Um, wait. What's the definition of <em>related?</em> If my employer is Microsoft, they do <em>everything.</em> They made a goddamn BARNEY PLUSH TOY with a computer in it once. Are plush toys related? Obviously operating systems, compilers, desktop applications, search engines, and games are related to Microsoft's line of work. Hmmm.</p>

<p><img src="http://i.stack.imgur.com/WRP7h.jpg" alt="Barney"></p>

<p>OK, what if my employer is a small company making software for the legal industry. Would software for the accounting industry be "related"? </p>

<p>I don't know. It's a big enough ambiguity that you could drive a truck through it. It's probably going to depend on a judge or jury. </p>

<p>The judge (or jury) is <em>likely</em> to be friendly to the poor employee against Big Bad Microsoft, but you can't depend on it.</p>

<p>This ambiguity is meant to create enough of a chilling effect on the employee working in their spare time that for all intents and purposes it achieves the effect that the employer wants: the employee doesn't bother doing any side projects that might turn into a business some day, and the employer gets a nice, refreshed employee coming to work in the morning after spending the previous evening watching TV.</p>

<p>So... to answer your question. There is unlikely to be substantial difference between the contracts that you sign at various companies in the US working as a programmer or in the law that applies. All of them need to purchase your copyright and patents without having to prove that they were generated "on the clock," so they will all try to do this, unless the company is being negligent and has not arranged for appropriate contracts to be in place, in which case, the company is probably being badly mismanaged and there's another reason not to work there. </p>

<p>The only difference is in the stance of management as to how hard they want to <em>enforce</em> their rights under these contracts. This can vary from:</p>

<ul>
<li>We love side projects. Have fun!</li>
<li>We don't really like side projects. You should be thinking about things for us.</li>
<li>We love side projects. We love them so much we want to own them and sell them! </li>
<li>We are kinda indifferent. If you piss us off, we will look for ways to make you miserable. If you leave and start a competitive company or even a half-competitive company, we will use this contract to bring you to tears. BUT, if you don't piss us off, and serve us loyally, we'll look the other way when your iPhone app starts making $40,000 a month.</li>
</ul>

<p>It may vary depending on whom you talk to, who is in power at any particular time, and whether or not you're sleeping with the boss. You're on your own, basically--the only way to gain independence is to be independent. Being an employee of a high tech company whose <em>product</em> is intellectual means that you have decided that you want to sell your intellectual output, and maybe that's OK, and maybe it's not, but it's a free choice.</p>



## Answer 20126

- posted by: [tghw](https://stackexchange.com/users/-1/7274-tghw) on 2011-02-11
- score: 110

California's Labor Code, [Section 2870](http://www.leginfo.ca.gov/cgi-bin/displaycode?section=lab&group=02001-03000&file=2870-2872) reads:

> a) Any provision in an employment agreement which provides
> that an employee shall assign, or offer to assign, any of his or her
> rights in an invention to his or her employer shall not apply to an
> invention that the employee developed entirely on his or her own time
> without using the employer's equipment, supplies, facilities, or
> trade secret information except for those inventions that either:  
>
> 1. Relate at the time of conception or reduction to practice of
> the invention to the employer's business, or actual or demonstrably
> anticipated research or development of the employer; or  
> 2. Result from any work performed by the employee for the
> employer.  
>
> b) To the extent a provision in an employment agreement purports
> to require an employee to assign an invention otherwise excluded from
> being required to be assigned under subdivision (a), the provision
> is against the public policy of this state and is unenforceable.


There are a number of other states with similar laws. I've compiled a list of states that have laws restricting what IP employers can claim ownership of:

* California* - [Cal. Lab. Code 2870-72](http://www.leginfo.ca.gov/cgi-bin/displaycode?section=lab&group=02001-03000&file=2870-2872)

* Delaware - [Del. Code Ann. tit. 19  805](http://delcode.delaware.gov/title19/c008/index.shtml)

* Illinois - [765 Ill. Comp. Stat 1060/2](http://www.ilga.gov/legislation/ilcs/ilcs3.asp?ActID=2238&ChapAct=765%26nbsp%3BILCS%26nbsp%3B1060%2F&ChapterID=62&ChapterName=PROPERTY&ActName=Employee+Patent+Act.)

* Kansas - [Kan. Stat. Ann. 44-130](http://kansasstatutes.lesterama.org/Chapter_44/Article_1/#44-130)

* Minnesota - [Minn. Stat.  181.78](https://www.revisor.leg.state.mn.us/bin/getpub.php?pubtype=STAT_CHAP_SEC&year=2006&section=181.78)

* North Carolina - [N.C. Gen. Stat.  66-57.1-.2](http://www.ncga.state.nc.us/EnactedLegislation/Statutes/HTML/ByArticle/Chapter_66/Article_10A.html)

* Washington - [Wash. Rev. Code Ann.  49.44.140, .150](http://apps.leg.wa.gov/RCW/default.aspx?cite=49.44.140)

* Utah - [Utah Code Title 34 Chapter 39](http://le.utah.gov/~code/TITLE34/htm/34_39_000300.htm)

*\*The California statute also requires an employer to inform employees about the law.*

Note that the laws that govern your employment contract are usually based on the state in which you work, not the state the company is incorporated in. And, as always, if you have questions about your employment contract, have a lawyer help you understand it and how it applies to state law. Also, this list may not be comprehensive. If you know of any other states, please add a comment and I'll update the answer.


## Answer 19428

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2011-01-26
- score: 40

By default (i.e. without a contract in place), no. Anything you do for them "on the clock" is considered "work for hire" and is theirs, but anything you do "off the clock" is yours.

**However**, a growing (and f!@#$ing stupid) trend is that, through your employment contract, your employer owns everything you do, on and off the clock. Their logic being, you're being paid salary and therefore you owe your life to the company. I find this absolutely appaling, but as you've seen from Zynga, a lot of employers are idiots... and sadly, a lot of employees are hungry to work and put up with it. Consider this a big red flag.

Sadly, this is enforcable and has been enforced several times... and I believe even affirmed in 9th District. Consider the long-standing case of [DSC Communications v. Evan Brown](http://www.unixguru.com/). Short story: dude had been working on a hobby project (some reverse compiler), took a job at DSC, quit, and then spent several years in court, only to lose the idea he had been developing before and during his tenure.

So, be careful. If you want your employer to own your thoughts... then sign with Zynga. Otherwise, there are plenty of other places that would be happy to have you.


## Answer 19443

- posted by: [Russell Steen](https://stackexchange.com/users/-1/6826-russell-steen) on 2011-01-26
- score: 39

Rather than spend hours worrying about whether or not they can enforce a given contract, I have solid universal advice that will apply regardless of the state you are in.

**Don't work for people whose policies you detest.**  Don't bank on them not being able to enforce a contract in your logic for taking a job with them.  If you don't like their employment practices, don't work for them.  It's that simple.

When they can't find top talent because of the abusive policy, they'll either fix their practices or suck as a company, but that won't be your worry.  The solution here is to vote with your feet.


## Answer 20137

- posted by: [George Grellas](https://stackexchange.com/users/-1/7307-george-grellas) on 2011-02-12
- score: 31

A few thoughts on this (answer ported over from [HN](http://news.ycombinator.com/item?id=2208819)):

1. I have done transactional work and litigation in and about these areas for nearly 30 years in Silicon Valley. Based on that experience, in practical terms, the risk you deal with in doing side work boils down to this: it is rare that an employer will make a claim to IP you develop on your own time and using your own resources but, when it does happen, its effect is pretty horrific.
2. California gives you more scope only because it has a law on the books that generally prohibits employers, on public policy grounds, from making claims to IP generated by employees working on their own time and using their own resources.
3. Even in California, however, an employee owes duties to his employer and one of those is that you don't misappropriate your employer's IP for your own use. This is why the California law says that you don't keep your side-project IP for yourself if it is in your employer's line of business or anticipated line of business. You can imagine the chaos that would result if any employee could state that, "no, that valuable IP that I came up with might have directly concerned what my employer was paying me to develop, but, in fact, I developed that particular key piece on my own time, etc."
4. In this sense, there is a common sense element to this area of law as applied in California. You typically will sense, without being told, whether the work you are doing on the side is capitalizing on the things your employer is doing or if it is truly unrelated.
5. That said, don't mess around with this sort of thing. It is both contract-specific and local-law-specific. That means general statements you hear from time to time (including those I just made) may or may not apply to you. If what you are planning to do has commercial value, then make sure to get it checked by a good local lawyer who can guide you through the pitfalls and explain alternatives. This is particularly so if you are not in California.


## Answer 19426

- posted by: [Bob Murphy](https://stackexchange.com/users/-1/5778-bob-murphy) on 2011-01-26
- score: 20

Regarding California, that lady from Zynga is full of hot air.

Since the 70s that I'm aware of, courts have repeatedly ruled against companies that try to pull the "we own anything you do in your spare time" or "you can't do side projects" nonsense.

In California in particular, moonlighting is heavily protected by law. Basically, as long as what you're doing on your own is legal and doesn't compete with your employer or otherwise "actually constitute a material and substantial disruption of the employer's operation", they can't say boo. In fact, if they let you go for moonlighting that doesn't truly adversely affect their "enterprise-related interests", you can sue them for lost wages and benefits and force them to reinstate you in your job.

California courts also tend to side with employees on things like this. For instance, *even if you sign a non-compete agreement*, the company pretty much can't enforce it in California. There have been several situations where people at Microsoft had signed non-compete agreements, quit, moved to California, joined Google in direct competition with Microsoft, and Microsoft couldn't do a thing about it.

Try typing "california moonlighting law" into your favorite search engine. You'll turn up lots of useful hits. Interestingly enough, I didn't see anything about any court cases, which may mean employers haven't wanted to try to enforce anti-moonlighting clauses in California since a change to the labor code that expanded workers' rights back around 2000.

Of course, I'm not a lawyer, your mileage may vary, void where prohibited, etc. but I've done side projects at every California job I've had since I moved to the state in 1987 and never had a problem.



## Answer 20148

- posted by: [lgritz](https://stackexchange.com/users/-1/1078-lgritz) on 2011-02-12
- score: 11

Joel and other have put it well -- almost certainly, any serious company will have you sign an agreement that will claim that they own basically everything you invent at any time until you leave the company.  This is fairly standard.

The best, most reliable way to solve your problem is to tell them about a side project you want BEFORE you start working on it (or, when starting employment, anything you've done before or already started) and get a written addendum that excludes that project from the employment agreement.  Usually they will still stipulate it needs to be done on your own time and with your own equipment.

Most reasonable companies will allow you to amend your list of project not owned by the employer if it is not directly competitive with what they do.  Some employers are not as nice, and will want ownership even if it's not related.  Maybe you shouldn't work for them.



## Answer 20151

- posted by: [Tim](https://stackexchange.com/users/-1/5712-tim) on 2011-02-12
- score: 11


Let me give a brief example of why companies may ask for this sort of thing.

I was called in to a (non-software) company where they had a small team of developers writing software for in-house use. An employee was writing one of their key software packages - version 1 was in use and everyone was happy... then he wrote version 2 but (and here's the stinker) his version 2 had a strong dependency on [his claim:] "a piece of software he'd written himself in the evenings that was nothing to do with their business" (it was basically a large sparse matrix library that did some of the heavy lifting of the business logic).

He'd built v2 on top of this library, but was happy to let them have a license to use "his software" for free, but he retained the source code (the debate was at what point any of this had been arranged and supposedly agreed)

They now wanted him to develop a v3 with various new features, but he claimed the new demands would require a new version of "his software", and he's only do this if they agreed to pay for a license. It was only at this point that the management became aware of the issue.

The guy was a chancer and was basically holding them to ransom by with-holding the source of a component that he claimed belonged to him, but had been written entirely while he worked for them and was designed solely for use with the software he developed "during the day".

Now how can they avoid this again - they could try and draw up employment contracts that say that you can work on your own stuff as long as it doesn't overlap, but they're not technical enough to make judgements and line calls, and what would happen if some-one claimed that some of their business logic had been thought up "at home while watching TV" and they'd just happened to write the code the next day.

So it was far easier for them to stipulate a blanket clause that they claim ownership over any software you write, day or night, while you work for them. There's a risk they might lose some potential employees, but that was a risk they could broadly account for, but being held to ransom by a rogue employee was not a chance they were willing to take again.

Big companies are rarely that interested in the side projects you have as long as you're doing your job properly (although I know some companies who think that if you have the time and intellectual capacity to still code in the evenings then you're not working hard enough and would perversely then mark you down as a slacker if they thought you were doing so) but they DO care about the risk of someone claiming personal ownership to something that they paid for. And blanket claims of IPR are an easier starting position for any fine calls...




## Answer 20154

- posted by: [Just Outsourcing](https://stackexchange.com/users/-1/7472-just-outsourcing) on 2011-02-12
- score: 11

Friendly reminder: contracts ***can*** be negotiated (and dumped in favor for something else as already mentioned).


## Answer 20159

- posted by: [Steve Hanov](https://stackexchange.com/users/-1/1958-steve-hanov) on 2011-02-12
- score: 9

Before accepting any employment agreement, look for terms that allow side projects. My employer has fair and clear terms layed out, which allow me to do lots of things in my spare time, and not have to rot my brain watching TV.

These are essential terms in a fair and balanced employment agreement

* **A clear definition of External Developments**. These are your side projects, and they should be allowed. But there should be restrictions to make it fair to the employer, too.
* **External developments must not use company time, equipment, or other resources**. Why should the company sponsor your hobbies?
* **External developments should not relate to the business of your employer**. It is wrong to take your knowledge and create a competing product. Of course, *everything* is related to the business of some large companies. So you have to use your judgement and keep the risk of being sued low.
* **You must not use an External Development, or allow your External Development to be used by the employer or incorporated into your employer's products** without permission, and if so, you give the company full use of the source code to use as it sees fit. 

These are paraphrased from Research in Motion's agreement in Canada.

It is not in anybody's interest to let your employer turn you into a couch potato. Even if your side projects are explicitly disallowed by a company, you have to balance the risk of being sued which may be really, really low. Keep on your employer's good side. Be a valuable and indispensible employee, build a stellar reputation, and the odds are that they will "hold the bus" for you and not bother you about it. Of course, if you are hiding things, demanding licenses, and being a jerk, you are asking for trouble.




## Answer 20175

- posted by: [Dmitriy Likhten](https://stackexchange.com/users/-1/7556-dmitriy-likhten) on 2011-02-13
- score: 9

To add to Joel's point, I think it is important to note that if you want to do a side project while working at a company you need the following:

a) review your contract. Joel's point will most likely be valid.

b) Notify your employer: "I will be working on project foo, it does not conflict with your business. I want an agreement that work I do on foo will be owned by me"

b/a) Your employer agrees, all is great. Have it in legal writing.

b/b) Your employer does not agree. You either drop the project or get another job.

**EDIT**

A big note here: Not all companies are greedy. Sometimes they may claim rights only to IP you created that is related to your field of employment. Lets say you are working for airline ticket company, they might request that any IP created to buy/sell tickets or any underlying system created for that purpose they can claim. Which means you can still write video games and not violate your contract or be forced to give up rights.


## Answer 20215

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-14
- score: 9

Very interesting discussions, and one I've had with employers.  I've had contracts rewritten, and turned down jobs based on their "Intellectual Property" clauses.  There is one thing that seems to have slipped by this conversation:  The language of the IP clause.

Here's the thing:  You're looking for the phrase "during the term of your employment".  In English, and some lawyers may argue this is not relevant, this means "from the time you began your employment until the time you ceased your employment", 24/7/365.  This is the "old style" clause, and gives everything to the employer.  What you're looking for is something which clarifies this by specifying what is for the purpose of your work with the employer in question.

If you have the old style phrase in your contract, and something which says you can moonlight, you might still lose rights to your side-project code.


## Answer 19432

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-01-26
- score: 6

If I were you, I would ask for specific details, before jumping to conclusions. "You can't have side projects" could mean an awful lot of things, but it certainly can't (enforceably) have its apparent literal meaning of you can't do any software development in your spare time.

So look at the policies and contracts and understand what they are actually asking you to agree to. Find out whether the emphasis is on (i) restricting your activities, or (ii) asserting ownership of their results. Look at how broadly or narrowly this is defined. And if there is something specific you want to be free to do and it seems to you reasonable, discuss it with your prospective line manager.

This kind of policy is against the broad trend, but in intensely creative industries I think it will stay entrenched for years to come.


## Answer 20325

- posted by: [Bozho](https://stackexchange.com/users/-1/5707-bozho) on 2011-02-16
- score: 6

All companies that I've worked for presented a contract stating something similar to "All products and services created by the employee, in and outside of business hours, are considered intellectual property of the employer". Since I _do_ have side projects, I have always negotiated the removal or rephrasing of this point. And so far it has worked. (Note that I'm in an eastern-European country, so things are likely to differ in the US)

So - read _your contract_, and negotiate the parts that you don't like.


## Answer 20138

- posted by: [orcmid](https://stackexchange.com/users/-1/7303-orcmid) on 2011-02-12
- score: 5

This is an interesting thread, but I wonder if there is another aspect to the question and the answer received.  Since Google, and perhaps other Silicon Valley firms, are noted for supporting on-the-job side projects (the result of which I imagine Google still owns, a different question and something Google might be generous about), the interviewer may have understood the question to be about that kind of "side project."

It would seem that the questioner might have needed to be more specific.

Something I did, when going back into corporate employment after 10 years as an independent, was identify my owning of a sideline business that I would continue to operate on my own time and have segregated from anything that I did related to my responsibilities as an employee of the hiring corporation.  There wasn't even a peep about it.  That was over 20 years ago, but the work-for-hire doctrine was already law.


## Answer 20140

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-12
- score: 5

If this was any company but Zynga you would [probably] be fine. Zynga *will* sue you (see mob wars), don't risk it with them. Also it's a crappy place to work.


## Answer 20139

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-12
- score: 4

There is a pretty good recent discussion in this article:
http://www.businessweek.com/managing/content/nov2010/ca2010112_650227.htm


## Answer 20267

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-15
- score: 4

I guess the biggest problem I have with the whole issue is that very few programmers are treated any differently than other production employees, except when it comes to the fruits of our labour.

If I work as a welder building trailers, my employer will be justifiably upset if I'm also building that kind of trailer for sale using my own equipment in my own shop. I've yet to hear of a such a shop getting upset at an employee for building something different at home, even if it's just a different kind of trailer that the employer doesn't deal in. Although I have heard of custom welding shops getting upset with an employee that also does custom welding from home, most shops know that there is very little overlap in the kinds of jobs the shop takes on versus what the home welder takes on. In most cases, the shop actually expects the employee to have access to welding equipment at home and to be using it, often to supplement income. (For the record, I actually worked as a journeyman welder.)

My problem is that, as a programmer, I have many of my own tools at home, yet I'm not permitted to use those tools to supplement my income they way I could when I was a welder. To make matters worse, I also happen to supply my employer with my most important tool, my brain. That feels to me like the equivalent of using my own welding equipment at the shop and then being prohibited from using it at home. Another big difference is that my own tools are frequently far superior to those provided by my employer, another clear difference with the welder. The welders in our shop are using welders that cost 10's of thousands of dollars each, a far cry from what they might have at home. My home computer is faster than my work computer and, in my opinion, has better development tools installed.

I know there are differences between intellectual property and physical goods, so maybe that's the only way to make it work. However, many of those differences are set aside when it comes to the sale and distribution of the actual product. In addition, no trailer manufacturer has an EULA that in any way resembles the standard EULA for a software product. In a lot of ways, I feel that companies are trying to play both ends against the middle. 


## Answer 19427

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-01-26
- score: 3

It is pretty standard for software companies to claim all your work while in their employ. If you go to work for Zynga, make sure you include in your contract a comment about prior inventions still being your own. This will protect you from the company claiming rights to your former "side projects".


## Answer 21113

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-03-03
- score: 3

Curious - how do they intend to prove one way or the other that something you invented after your term of employment wasn't created during your term of employment? They could claim (and if you are "unscrupulous" for various values of the term) you could mark in a different date into all the source files and change the date-stamps on the files.




## Answer 19434

- posted by: [John Sjölander](https://stackexchange.com/users/-1/5866-john-sj-lander) on 2011-01-26
- score: 1

**Not by default.**

It should be governed by your contract.

If you have a section to the lines of "software developed on company time and/or using company resources" pertaining Intellectual Property the width of that defines your rights.

Also, what kind of project you may undertake is commonly governed by your *Non-compete clause*.

As Alex points out, I hear the trend being companies applying this clause very widely. Too sad.


## Answer 19439

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-26
- score: 1

Yes they can do it, at leat in Germany dunno whats about USA, but think there is the same "idea" behind the law.

Programmers arent artists, or working at car production for example. They use code (which could be copyrighted) The fear "behind" this idea. Is that you c&p code from Zynga and use it at home. Well Iam not quite sure if they cole could say "everything you create is us". But they could say: You are not allowed at all to work for others including opensource projects.




## Answer 20550

- posted by: [James](https://stackexchange.com/users/-1/7946-james) on 2011-02-21
- score: 1

If the company took the extreme example, that it owned the results of your labor 24/7, then you would be if not a "slave", at least some type of indentured servant.  I can not believe that such contracts would be enforceable anywhere in the US anymore.  However, non-compete contracts that don't allow employees to produce directly competing during or shortly after their employment generally can be enforced to a greater or lesser degree. 

I have to say Joel's answer is nonsensical on why companies force employees to sign these contracts.  Every line of code that an employee writes 9-5 on the job with a company computer belongs to the company.  Any line of code that an employee writes in their spare time with their own property should never be checked in to the employer's code base.  That is a clear cut diving line and prevents any scenarios of one programmer allegedly holding up an acquisition.


## Answer 22678

- posted by: [Kilo](https://stackexchange.com/users/-1/1375-kilo) on 2011-03-31
- score: 1

What if I travel for my company?  When I go back to my hotel room [paid by my employer], pull out a personal laptop I brought along on the trip (I can fit two laptops in my computer bag), and punch out some code on my personal laptop.... am I still on company time?  Do I still fall into the category of "working for hire" or being "on the clock?"

I have no employment contract with my employer.  They essentially hired me with a letter saying I will work on various projects for a salary.  I write software.

My personal laptop has development tools that I paid for.  Nothing on my personal laptop belongs to the company or was paid for by the company I work for.  I had the personal laptop before I joined the company... In fact, I brought this laptop to an Interview to demonstrate some projects I worked on.

I'm really curious about what constitute company time when you travel for your employer...


## Answer 20185

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-13
- score: 0

I don't have experience with this in the US but the typical IT contract I've worked with says that any material produced **for** ACME corp is the property of ACME corp.

This negates the 9-5 argument which I think is perhaps a too narrow a way to look at it since your contractors will no doubt work longer hours than specified throughout a project.


## Answer 20389

- posted by: [Nilesh](https://stackexchange.com/users/-1/6985-nilesh) on 2011-02-17
- score: 0

Usually, there is no loyalty factor if you are working on side projects. For example if your work at employer and your side projects are in the same line then any innovative thing you come up, who has got the claim to it? For if your employer is having a product called 'Project management" and you are the super duper java,php coder assigned to write a new piece of the same product. Since you are so efficient, now you have lot of spare time in the evening. You know you can develop a project management application in a short period and maybe better than the product at your employer. So will you be loyal to your employer?

So ethically speaking, even if you decide to side projects and your employer allows you pick a niche that does not clash with your employer's product.


## Answer 48784

- posted by: [Bob](https://stackexchange.com/users/-1/7689-bob) on 2013-04-26
- score: 0

If I work for a software company and write a novel that is published. Can the software company claim they ownership of the novel and take all the profits? Could they legally force me to sit down and type up any ideas I have in my head about the novel and claim ownership of it? 

So if I work for a software company that is basically a big contracting company and does not produce any products. Can they claim ownership of anything I develop? Most of the employment agreements are pretty generic. We own everything. Just because they are in the 'software' business would they own a product then? Even if their contract says 'we own everything'.

Virtually every employee makes you sign something that says we own everything. It is not like you have alot of options. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
