## How the startups manage to afford cost of web servers and other hardware

- posted by: [vikas devde](https://stackexchange.com/users/-1/19257-vikas-devde) on 2012-08-15
- tagged: `startup-costs`, `expenses`, `hardware`
- score: 1

i want to know, how startups manages their cost of hardware, like servers and other hardware. do they buy brand new material or the second hand, what about room to keep their servers and all other electricity, broadband connections, buying bandwidth etc etc expenses. can you give me example of current famous sites like facebook, twitter etc, about how they managed their expenses on these things.


## Answer 41381

- posted by: [JeffS](https://stackexchange.com/users/-1/15873-jeffs) on 2012-08-15
- score: 7

Most startups have someone else think about it.

It's very common to host your application in an environment where adding additional servers is a 1 minute task, and can be done on an on-demand basis.

A small VPS, even with only 512MB of RAM is often enough for an application that is in testing. If you're not building something where performance is going to be a huge problem (you're not processing huge amounts of data), then this is usually the ticket.

Good providers for on demand scalable hosting include Amazon and Rackspace.



## Answer 41398

- posted by: [jrg](https://stackexchange.com/users/-1/12807-jrg) on 2012-08-16
- score: 3

<p>They get someone who knows what they are doing, and then they go do it.</p>

<p>They normally start with either a <a href="https://en.wikipedia.org/wiki/Virtual_private_server" rel="nofollow">VPS</a> (I hear a lot of people use <a href="http://www.linode.com/" rel="nofollow">Linode</a>) or a VM that the developers run, and then when they go public, they generally look into moving to <a href="http://www.rackspace.com/" rel="nofollow">Rackspace</a> or <a href="http://aws.amazon.com/" rel="nofollow">Amazon Web Services</a>. </p>

<p>However, there are a lot of tools that can be be used to make it a lot simpler, and some of them are covered in various ServerFault questions. </p>

<ul>
<li><p><a href="http://serverfault.com/questions/75476/toolkit-habits-for-linux-network-system-administration">http://serverfault.com/questions/75476/toolkit-habits-for-linux-network-system-administration</a></p></li>
<li><p><a href="http://serverfault.com/questions/3004/resources-for-beginning-linux-administrators">http://serverfault.com/questions/3004/resources-for-beginning-linux-administrators</a></p></li>
<li><p><a href="http://serverfault.com/questions/70932/linux-system-administrator-guide">http://serverfault.com/questions/70932/linux-system-administrator-guide</a></p></li>
<li><p><a href="http://serverfault.com/questions/375/good-book-for-a-software-developer-doing-part-time-linux-system-administration">http://serverfault.com/questions/375/good-book-for-a-software-developer-doing-part-time-linux-system-administration</a></p></li>
<li><p><a href="http://serverfault.com/questions/32876/good-resources-for-linux-sysadmin-tools-techniques-and-practices">http://serverfault.com/questions/32876/good-resources-for-linux-sysadmin-tools-techniques-and-practices</a></p></li>
</ul>



## Answer 41412

- posted by: [Mihaly Borbely](https://stackexchange.com/users/-1/13257-mihaly-borbely) on 2012-08-16
- score: 3

This is a very typical mistake that founders, usually technical founders make. I went through this myself, so I know how hard it is to realize and accept this, but its true:

**It doesn't matter at all what hosting environment you prototype on!**

At first I also took this very seriously, but in the end, guess what our first test server was: an ancient laptop running in my kitchen. p3, with 384 MB ram. Later we "upgraded" to Amazon free tier, so now we have an awesome amount of 600 MB ram. Did we ever have server load or performance problems? Not one time.

Why? Because in the prototyping phase, 100% of your problems will be connected to lack of traction. If not, then you are the luckiest startup ever, you've got market fit, and investors will kill each other to give you money. But until that happens, please, don't buy servers. Don't even rent a VPS. You will not need it.

Go with the free options: your old pc at home, Amazon free tier, or MS BizSpark.

http://gettingreal.37signals.com/ch04_Scale_Later.php


## Answer 41376

- posted by: [theonlylos](https://stackexchange.com/users/-1/11985-theonlylos) on 2012-08-15
- score: 1

In general it's simply a matter of scaling at a reasonable rate. Typically when I have a client who has an ambitious project, we'll usually have a long private beta where we'll issue x licenses and then as the project progresses we issue more accounts until we have a public launch.

For prototyping, usually a VPS is an affordable alternative to a dedicated system since you literally can scale up and down based on what you need. In many cases a VPS will be sufficient for the early stages (private beta).

On the other hand, Dedicated servers come into play when you need large amounts of CPU power, because with a VPS while you have dedicated storage/ram, you do share the CPU with the other sites on the server. Still - the premium of a dedicated server usually makes it only practical when you are really rolling.

So to answer your question, there really is no specific guide you can follow on how many servers to buy. Rather you just have to start from square one and scale accordingly. If you simply control the amount of signups, that will go a long way to getting your prototype up and running, from which you can then pursue investors or funding.


## Answer 41419

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2012-08-17
- score: 1

Either use a cloud computer provider like AWS or a VPS like Linode.

It's crazy to buy and maintain equipment these days unless you have a specific reason to.

Also, I wouldn't use facebook and twitter as examples that mean anything to you, I am guessing your business is a lot different to theirs.


## Answer 41410

- posted by: [Brent Pabst](https://stackexchange.com/users/-1/19274-brent-pabst) on 2012-08-16
- score: 0

As someone mentioned above you can take a look at Microsoft's BizSpark program which offers free Azure Compute hours.  In addition you may also want to sign up for an MSDN subscription because that too includes a specific number of compute time.

Just an FYI if you didn't know Microsoft's Azure platform does provide Windows and Linux environments and has pretty much supported PHP applications from day one so cross-platform should not be an issue here.

No reason not to use free!


## Answer 41417

- posted by: [james](https://stackexchange.com/users/-1/5800-james) on 2012-08-17
- score: 0

IIRC Google built their own out of mainboards and power supplies, mounted 4 per layer in a server rack, there's one in the computer history museum in Mountain View,  California. e.g. http://archive.computerhistory.org/resources/physical-object/google/102662167.4.lg.jpg

The other answers explain how to get a good hosted server. If you want good deals on used servers try finding an off-lease equipment dealer. We've found some great deals on 3 year old top tier equipment that's been removed from data centers (too old, too hot, too much energy) and replaced by new hardware. I wouldn't use it for customers but the hardware has plenty of years left in it for internal use. 




## Answer 45257

- posted by: [usabilitest](https://stackexchange.com/users/-1/3024-usabilitest) on 2012-12-25
- score: 0

You need to understand well what the technical requirements for your business are. If you don't know exactly, talk to someone. Most of the hosting companies will be quite honest with you about the costs and what you get for your money. And normally you should start with a minimum. It is easy to add on the capacity these days. Quite rarely you will even need to deal with the hardware. Let professionals do their jobs.

For example, if you start a landscaping business with a buddy, you probably need just a single truck, and at that the one that can haul dirt well and costs the least. You probably won't start by financing a fleet of shiny trucks, even if you think you have that "great idea" how to interrupt the business you are trying to enter.

Also, don't compare yourself to odd-balls like Facebook and Twitter. Facebook started on a shared server space that belonged to a college network with couple of guys probably sharing a single keyboard. By now I'd assume they own server farms all around the globe to protect the content through redundant storage and adequate bandwidth scalability. And because they had such a phenomenal growth people were throwing money at them in order to grow. Yep, both of the ones that you mentioned started on borrowed money.

My guess, you are not there yet. But you are on the right track - asking questions. Those are free. Good luck! 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
