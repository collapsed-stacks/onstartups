## Software Licensing/Copy Protection - DIY or Buy?

- posted by: [Clare](https://stackexchange.com/users/-1/3610-clare) on 2010-06-08
- tagged: `software`, `licensing`, `copyright`
- score: 12

As an ISV/software publisher, would you produce your own licensing/copy protection solution, or would you buy into a professional solution?

Which route would you choose and why?


## Answer 11885

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-06-08
- score: 8

I've done both and in each case they were the right decisions.  (In my opinion)  

I rolled my own simple protection for software I sold for $99.   

My latest venture is licensed for $9000 to $25,000.  We use a dongle licensing scheme for that one.

Note that I have very limited experience with this aspect of development.  You need to just make a decision and move on and realize that you are never going to beat a determined hacker or group who wants to steal your software.  


EDIT

I suppose I should provide a bit more detail...

For the one I wrote myself it was a C++ desktop app that interfaced with some lab hardware through rs232.  It was a very niche product.  I did not provide the ability to give timed trials - rather the free version was limited in the number of devices it could attach to.  I eventually configured a database and paypal mechanism to automate sending the user a license code after a purchase.  I made a mistake early on in making that a manual process.  It was terrible.  However, many of the customers were running this on a machine that had no internet connectivity.

If you are going to write your own I would say keep it very simple and don't try to get fancy and solve all the problems.  You will always lose out in the end and you can't justify your time spent.

I think Jason C had a suggestion on how he made his initial licensing.  I will look for it and link it here.

Right now I am using Keylok.  They just happened to be recommended to me and my partner when we had a need for it.  It works for us.  The downside is the physical shipping to a location, but not a big deal as the configuration and sales issues take up significant time anyway.  


Whatever you choose I recommend making it very modular/easy to replace - especially if you roll your own.  Be flexible and be ready to change technologies, though one hates to waste cycles re-doing completed tasks.


## Answer 11891

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-06-08
- score: 7

The answer depends a bit on the environment you're targetting since that dictates how many licensing system options you have to chose from.

In general, time you spend developing and supporting your licensing system can be very steep, and it's non value add - it's taking time away from adding features and doing things your customers really want.  That said, sometimes it's worth it if there's something special about your licensing.  For example, perhaps you want to be very generous in your license enforcement; most systems tend to be very strict.

If you can fit your needs into an off the shelf system you are likely to be better off in the long run because they've already figured out that file permissions and encryption work differently on Windows XP Home than Windows Server 2008 or in Turkey or whatever.  These aren't problems you want to take up your time. 

Of the ISV's I've talked with about 2/3rds built their own systems.  Of those, I can't think of any that it hasn't been both a support hassle and a source of fear - fear that it's locking people out of being able to run trials or otherwise is costing sales.  I've seen transitions happen both ways (from in-house to purchased and purchased to in-house). 

There are some very good purchased systems.  I'd recommend you seriously examine them before investing significantly in your own system.  If you do invest in your own, have it be for a competitive advantage because it is going to occupy a sizable portion of your development budget if you're a small company, at least initially. 

In our case we ended up building our own because we're terrified of customers not being able to use our software when they need it - we needed a system to tend to let people run it, not block them and have some grace periods for things. This is unique to our situation:  We didn't want someone who needed to use our tool to fix a server find out they couldn't run it because the server couldn't contact the Internet or because our activation server was inaccessible or something.  That said, it was a close decision and we very nearly went with a third party option except we were scared off by some very dodgy press they got right around the time we were making our decision (moral of the story there: Don't pick a fight with a customer in public).  Despite us having a very solid engineering base to draw from in encryption and systems it still took 200% longer than we predicted.


## Answer 17589

- posted by: [the dictator](https://stackexchange.com/users/-1/473-the-dictator) on 2010-12-09
- score: 2

Just buy it, don't even consider writing yourself. Spend that valuable to time into the product.

If someone is going to crack it, they'll crack whether it's off the shelf product or a custom product. So there is no way to stop it. At least when you buy it you don't need to spend time on that (it's not a one time hassle, there'll be always on going process to fix bugs etc.). 

Last thing you want to do is pissing off paid customers.


## Answer 17592

- posted by: [alphadogg](https://stackexchange.com/users/-1/3197-alphadogg) on 2010-12-09
- score: 2

I agree with fx.

If there is a big enough "street cred" value, or a big enough market using the software, crackers *will* hack it. Especially in the latter case, malicious "black hats" will use it to distribute their payloads and increase the size of their botnets. 

Look at it this way, do you think you can create or afford a system better than BD+ on Blu-Ray?

It's been hacked since 2008, but was said to be foolproof.

To really build an unhackable system takes some serious cryptographic and application structure knowledge. For example, if your software process an install key with the same algo at the same place in each exe out there, your software is 100% hackable. If it hasn't been hacked, it's because no one cares to.

Furthermore, the bigger problem is that no matter how great the system, the "human layer" is a loophole. How many times have I had a client on the phone who claims they are validly installing it for the sixth time, beyond their allotted five installs? How do I really know? Or, do I play hardball and risk pissing them off?

Buy into a simple licensing system to put a road bump on the low-level, casual piracy and move on to making your offerings worth paying for.


## Answer 40467

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2012-07-11
- score: 2

<p>I agree with Kendall and "the dictator", especially the sentiment that your time is better spent making and marketing your product rather than wasting thousands of hours needed to make decent licensing in-house. </p>

<blockquote>
  <p>Just buy it, don't even consider writing yourself. Spend that valuable to time into the product.</p>
</blockquote>

<p>Obviously I'd recommend you trying (and then using) <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a> -- an online activation and licensing solution for Windows / Mac OS X / Linux. I'm the founder of the company that makes LimeLM, so of course I'd say that.</p>

<p>We also have an article that goes into detail about how to make properly designed hardware-locked licensing (a.k.a. online activation). See: <strong><a href="http://wyday.com/limelm/features/why/#hardware-locked-descr" rel="nofollow">How hardware-locked licensing works</a></strong>. This describes the steps you need to take to build hardware-locked licensing in-house. The article also goes into the common mistakes companies make when designing licensing (and how to avoid these mistakes). I believe it gives enough details to set you on the right path, but not so many details as to bore you to tears.</p>

<p>Tell me if it helps. Or if you think we're not giving enough details let me know (either comment on this post or send me an email at wyatt@wyday.com).</p>

<h2>Cracking can't be stopped</h2>

<p>Also, "alphadogg" brought up cracking:</p>

<blockquote>
  <p>If there is a big enough "street cred" value, or a big enough market using the software, crackers will hack it. </p>
</blockquote>

<p>This is absolutely right. I'll just expand this to say if it exists on a computer it can be cracked. That is, <em>all</em> software can be cracked (and easily) whether you have a big market or not.</p>

<p>So what's my point? My point is don't fall for companies promising "uncrackable" licensing protection or promise to "thwart hackers and crackers" with "anti-debugging" tricks. <a href="http://wyday.com/limelm/features/why/#snake-oil" rel="nofollow">These tricks are all <strong>snake oil</strong></a>. That is, "anti-cracking" are all bogus. You can't stop cracking. Full stop.</p>

<p><strong>Why have licensing if it can be cracked?</strong></p>

<p>The point of licensing is to increase your revenue by preventing casual piracy (using serials over and over again). There is real money to be made by stopping casual piracy. Don't worry about crackers because crackers don't buy and customers don't crack.</p>



## Answer 43942

- posted by: [ssec](https://stackexchange.com/users/-1/21396-ssec) on 2012-10-30
- score: 1

Writing effective custom software copy protection solution requires too much of your valuable time.

There are many ready-made software protection tools with different pricing (from cheap to really expensive) and licensing (from royalty free to per license fees) options you could choose from. 

Sure, there is no uncrackable system, hardware or software, if application works it can be cracked. Software protection tools are mostly intended for prevention of casual cracking and illegal distribution by ordinary (standard) users. Distributing commercial software without any kind of licensing control is simply wrong strategy which would shut down you business for good. 



## Answer 11887

- posted by: [Stefanos Tses](https://stackexchange.com/users/-1/3178-stefanos-tses) on 2010-06-08
- score: 0


A few months ago I did all the research in the world on this matter.
I've tested all products possible.

I ended up creating my own licensing engine and purchased SmartAssembly for protection/obfuscation.

It took me less time building my licensing engine than understand how others work and perform a real test.

Of course, all depends on your licensing needs. 


## Answer 40435

- posted by: [logicnp](https://stackexchange.com/users/-1/11650-logicnp) on 2012-07-10
- score: 0

<p>I would definitely consider using an off-the-shelf licensing product - developing a license scheme is not so easy and you are better off spending that time on developing your actual core product functionality. Have a look at <a href="http://www.ssware.com/cryptolicensing/cryptolicensing_net.htm" rel="nofollow">CryptoLicensing</a>.</p>

<p>DISCLAIMER: I work for LogicNP Software, the developer of CryptoLicensing.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
