## I've got a great algorithm, now what?

- posted by: [Amichai](https://stackexchange.com/users/-1/3066-amichai) on 2010-04-11
- tagged: `outsourcing`, `seed-funding`
- score: 10

I have an algorithm for doing OCR (Optical Character Recognition) in a way that no one has ever done before. I've built rudimentary prototype software and I've tested my algorithm against the existing OCR softwares on the market today and the results were all very positive. I want to turn this algorithm into a business venture and I have some seed money that I'm ready to invest, but I don't know where to begin. I've taught myself c++ and Qt but I have no other programming or project management experience.

I'm thinking about developing a software to sell and distribute online. Outsourcing might be an inexpensive way to go about the software development project (I could even keep the method of the algorithm a secret from my programmers) but I don't know which skills I would need to hire?

Any suggestions? Other ways of doing this? Anything else I should know before venturing down this path?



## Answer 10083

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-04-11
- score: 9

<p>Phew, that's a hard one. Maybe I'll come back with better ideas later. For now, some initial thoughts:</p>

<ul>
<li><p>You have written about this algorithm you have, but not much about your own dreams and desires. <strong>What do you want?</strong> Maybe your invention can lead to a pile of money, but money alone isn't a good reason for becoming an entrepreneur.</p></li>
<li><p><strong>Absolutely keep your algorithm secret for the time being.</strong> And go see a good patent &amp; intellectual property lawyer. In most jurisdictions you cannot patent an algorithm per se, but there are other means of legal protection that might be available to you. Take a hard look at what legal protection you can get, and how much it will cost you in fees. (Keeping secrecy now may be a requirement for obtaining a patent. And if nothing else, it keeps your competitors from copying your algorithm, and keeping your invention as a <a href="http://danashultz.com/blog/2009/11/19/you-can-have-a-successful-business-even-if-you-dont-have-a-patent/" rel="nofollow">trade secret</a> may be the final solution you'll end up with.)</p></li>
</ul>

<p>About what to do with the algorithm... Maybe it's just me, but I think it's surprisingly hard to say...</p>

<ul>
<li><p>The market for desktop OCR software is not that big; most users are already invested in one of the existing OCR software systems; and it's not clear to me that current users are looking for a better solution. And from hard-won experience, I can say that a B2C desktop application takes a lot of work to mature. There is always opportunity in an existing market, so don't let this discourage you.</p></li>
<li><p>Webapps are the new hotness, and a webapp doing OCR isn't a completely horrible idea, but it's not easy either ... big files that need to be uploaded to the server, usability challenges, market risk.</p></li>
<li><p>You could <em>license</em> your invention to someone. That's often quoted as the entrepreneurs dream, sitting in your living room sipping good wine while your invention is doing all the work for you... But licensing inventions can often fail due to the 'not invented here' syndrome.</p></li>
</ul>

<p>Some thoughts about what you could think about:</p>

<ol>
<li>What would motivate you personally, is there anything in the above or elsewhere that is looking super-exiting to <em>you</em>? Building a company or product is hard work, and if you do it in an area that is motivating for you personally, then you improve your chances considerably.</li>
<li>Without telling us secrets, are there any elements in your technology that naturally point it in a specific direction? Does it excel at uncommon words (scanning texts in small languages, nice business jargon), handwritten text (scanning medical prescriptions?), or is there something else that your tech naturally lends itself to?</li>
</ol>



## Answer 10097

- posted by: [Alex Lam](https://stackexchange.com/users/-1/1281-alex-lam) on 2010-04-12
- score: 9

<p>I've recently brainstormed up an OCR related technology - here are my notes.</p>

<ol>
<li><p>Create an API that third party folks can use - A lot of data is currently being captured at the consumer level and used at <a href="http://www.evernote.com/" rel="nofollow">Evernote</a>. They are still small and growing rapidly - create a model that allows their users to use your algorithm.</p></li>
<li><p>Create an iPhone/Android app that can utilize your algorithm. You are tied to one niche, but that's okay - if your algo is better - as folks such as Evernote grow very intensely, you'll be in the sweet spot for them to acquire.</p></li>
<li><p>Adapt your API to work with <a href="http://www.dropbox.com" rel="nofollow">Dropbox</a> - while Dropbox has yet to release their API yet - their user growth is tremendous (more than 4 million now in less than a year?) Ride that wave.</p></li>
<li><p>Legal firms - look up the Discovery market - they deploy a lot of OCR and manual person reading - these guys need solutions that can scale very well. May require a combination of recognition and search - but with <a href="http://www.websolr.com/" rel="nofollow">third party search</a> coming up - you can probably get away with just concentrating on OCR. Discovery market is fantastic - has big expenses - the only issue may be that they have lots of regulation issues on where the data resides (they are usually in the midst of litigation or lawsuits). If you can provide a rack solution, pretty much ready to rock. Each project easily goes from 100,000 pages to 5 million pages. They tend to employ hundreds of people per project and are now faced with international discovery - which if your OCR can scale to handle multilingual well (bi directional, Chinese, Japanese, Logo, signatures) - you are set.</p></li>
<li><p>Google's book scanning project - they <a href="http://mashable.com/2009/09/16/google-acquires-recaptcha/" rel="nofollow">bought out the re-captcha folks</a>. If you can build out a proof case and plug it online - you might just get calls.</p></li>
<li><p>Jesper had some good questions/suggestions - if it's successful in the medical area - there's so much of the lab process/research portions to investigate in.</p></li>
<li><p>Prominent background impression - If your algo can recognize words in photos - run it through on flickr see what emerges. You might just hit on a "trend" list like that of twitter. It's a project that would consume a lot of bandwidth and processing - but that's what cloud computing is for. If you can recognize the trends of things coming up - write a paper, do a case study and call Malcolm Gladwell quick. The fashion market would love this data. Heck, if you can do a logo count (ie Canon vs Nikon) and chart it out - this is very interesting market data. </p></li>
<li><p>Take screenshots of websites and measure the words. Now, web crawlers already can recognize text out there - but there are some content that's embedded inside the graphics - which until this idea is available - it's essentially a market that's been largely ignored by search engines. There are folks like <a href="http://www.cooliris.com" rel="nofollow">CoolIris</a> who are looking at a visual search of things - but it's still missing something - searching on text stuck inside graphics. </p></li>
<li><p>Logo count - but on film - How much product placement hours did Coca-cola have last year? Break down films to each frame and then recognize and count. It's a branding research data which advertisers would love to get hold off.</p></li>
<li><p>Employee tag recognition on CCTV - It's competing against RFID - but yours is better as its less paranoia inducing.</p></li>
<li><p>Sports analysis - you'll have to be passionate about this - but if you are, check out Michael Lewis's book - <a href="http://en.wikipedia.org/wiki/Moneyball" rel="nofollow">Moneyball</a>. (Or wait for the movie coming out next year!) Once you can recognize players in videos, photos, you'd get fame measurement, branding, game analysis, et al. </p></li>
</ol>

<p>If you're keen to explore further, feel free to contact me.</p>

<hr>

<p>Alternative business models -</p>

<ul>
<li>Consulting - </li>
</ul>

<p>The legal firm work would be able to throw a lot of business your way with solutions - if you enjoy the algorithm work and have exception cases floating up to you - then you can work with a group that already services these folks. Talk to KPMG or any of the big accounting firms.</p>

<hr>



## Answer 10116

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2010-04-12
- score: 1

You may have a product superior to the ones currently on the market, but you you have the resources to out-market the competition?
Is there a single competitor of multiple? Can you sell it to established players? Perhaps you can pitch it to several at the same time and not make a secret of it; that way you may get them bid higher against each other.


## Answer 10091

- posted by: [GRex](https://stackexchange.com/users/-1/2475-grex) on 2010-04-12
- score: 0

I may start by analyzing every OCR software in the market, examine each segment's potential and challenges.

By the end of that, pick one particular segment and build a competing product for it.

The result of your research above will determine the direction you take with project management, costs, outsourcing options, marketing and pretty everything your business will be down the line.


## Answer 10104

- posted by: [philobus](https://stackexchange.com/users/-1/2812-philobus) on 2010-04-12
- score: 0

OCR software is needed very much for AR.
Imagine someone can take a foto of a chinese sign and your software gives him the translation.


## Answer 10107

- posted by: [Mike](https://stackexchange.com/users/-1/2696-mike) on 2010-04-12
- score: 0

<p>You got some great ideas and input so far. </p>

<p>Jasper's idea of building a web app seems like a good way to go.</p>

<p>A web app will extend your market reach and simplify the sign-up/licensing process to use your solution. It will also allow you to test your business model and get feedback from beta users.</p>

<p>If you decide to try this channel out and need to get a prototype built fast to test the idea and show to investors, you might want to <a href="http://www.outsystems.com/goto/startups" rel="nofollow">take a look at the Agile Platform and the special offers for startups</a>. I work for OutSystems so feel free to DM me if you want to discuss it in more detail.</p>

<p>Hope this helps</p>



## Answer 10156

- posted by: [Dmitry Leskov](https://stackexchange.com/users/-1/2093-dmitry-leskov) on 2010-04-13
- score: 0

1. Even though I hate software patents, but - patent your algorithm now, before someone else discovers it.

2. Aim at licensing your algorithm to big players. Build some free apps for desktop/Web/mobile to popularize it. Stay away from spammers.

3. Outsourcing the development is OK, but do not expect it to be **that** cheap. Disclosure: we did create core IP for a handful of startups.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
