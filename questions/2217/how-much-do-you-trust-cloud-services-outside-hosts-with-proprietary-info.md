## How much do you trust cloud services / outside hosts with proprietary info?

- posted by: [cemerick](https://stackexchange.com/users/-1/1083-cemerick) on 2009-10-23
- tagged: `outsourcing`, `infrastructure`
- score: 4

I've long been of the opinion that the core assets of a software company (e.g. source code and any system that touches it, continuous integration environments, internal wikis containing design/planning docs, etc. etc) should always be closely-held.  In other words, hosted in-house, maintained by employees, and not managed by outsourced vendors.

However, I'm starting to revisit this line of thinking.  Some counterarguments, in no particular order:

 - We've outsourced email *forever* (because the associated admin is just way too costly), and there's plenty of confidential / "proprietary" stuff flowing through email (not on the level of source code, but certainly business terms, technical discussions, etc)
 - No one really cares about our stuff that much. We're a small software company, and in a hosted environment, the changes of us being targeted for theft, etc., seems absurdly small given much more lucrative opportunities for such things.  (This the apparent vs. actual risk aspect.)
 - We don't have a dedicated sysadmin, so just think of all the time and resources being spent/wasted managing various internal systems only because of some amorphous fear.
 - Of course, even worse is the opportunity cost of the admin time/resources.  Maybe we wouldn't be so small if we weren't fiddling around with CI server admin and such ;-)

Thoughts?

EDIT: Just FYI, by "cloud/outside hosts", I mean operations like Amazon AWS, Rackspace, et al.; decidedly not second or third tier hosts, startups, mom-and-pops, etc.


## Answer 2242

- posted by: [pbreit](https://stackexchange.com/users/-1/239-pbreit) on 2009-10-23
- score: 8

We are a very successful Silicon Valley startup and we don't have a single server on our office network. Everything is in the cloud. Gmail and Google Apps, bug tracking, SVN hosting, dev/qa servers, CRM, telecom...everything. The fact is, your secrets probably aren't very valuable and a snapshot of your company is of little use. Companies create value over the long term by having a great team execute on good ideas on a continuous basis.


## Answer 2224

- posted by: [Cary](https://stackexchange.com/users/-1/937-cary) on 2009-10-23
- score: 5

The key to answering this question is that as a startup, you don't have the resources to innovate on a non-functional concern.

Outsource what is not your core competency to someone who does it better, cheaper, etc.

The truth is that Amazon, Google, etc. are not going away any time soon, if ever.  You're data, email, etc. is likely much safer there than it would be on your private network which probably has a wireless access point that could be hacked by other close by companies/employees.

The most important thing here besides security is continuity and the cloud can offer that to you, cheaply.




## Answer 2219

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2009-10-23
- score: 3

I find mysef to be pretty trusting when it comes to data passing over other networks through the cloud: I really don't think that a nosey sysadmin on their end will snoop our data and, if they do, it will take a lot of snooping before they find any "juicy" stuff.

However, **I don't trust the cloud to keep our data safe**. I hear story after story of cloud failures, insane theft stories ([Ocean's 11-style](http://www.datacenterknowledge.com/archives/2007/12/08/oceans-11-data-center-robbery-in-london/)), floods, etc. And then there's the fact that a cloud provider could just all of a sudden shut down. No warning, just gone.

That scares me. We're a sotware company and spent hundreds of thousands of dollars to develop soft assets. I trust a federally-regulated and insured bank with my assets, but not Google or any other company with "we can change it whenever we feel like it" terms of service which state their not liable for loss, blah blah blah... 

But **I do believe that both our in-house apps and the cloud will <i>not</i> fail simultaneously**. Whatever we put in the cloud, we have a redudant copy in the office. Exchange server, local mailbox. Local back-ups that go to the cloud for backup. Etc.

Yes, it costs  more in terms of time... but it's worth it to know the data is safer.


## Answer 2320

- posted by: [Dror](https://stackexchange.com/users/-1/1057-dror) on 2009-10-24
- score: 3

Off the top of my head, I can think of 4 approaches to hosting.

1. In the cloud (let's lump all the different options in here.).

2. Hosted either either managed or unmanaged at an ISP.

3. Low budget, low reliability in house. In other words, put it on your DSL line and hope for the best.

4. Expensive, somewhat reliable in house. 

For a startup #4 will never be as reliable as either 1 or 2. Not by an order of magnitude. Do you really want to deal with servers, UPSs, connectivity from multiple vendors, etc, when you can get a small instance from ec2 for $72/month?

Looking at #1 and #2, they're really equivalent. It's a question of who you let access your data. Overall, I believe it's certainly worth it. We're fully hosted on ec2/s3.



## Answer 2220

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2009-10-23
- score: 1

If you are worried that some of your data is proprietary then you can perhaps encrypt it, but the decryption would be on the software in the cloud so it is only limited protection.

As more people move to doing software in the cloud then it will be harder for the companies to really be able to mine the data as easily.

But, if you are really concerned then just host it yourself.

We are looking at putting the software in the cloud mainly for uptime, as we are developing software to be used by safety engineers, and if they need to make a change while the crane is waiting, they can't wait for a computer to reboot.

So, the convenience is more important than what they may learn from the database.


## Answer 2319

- posted by: [kabir](https://stackexchange.com/users/-1/849-kabir) on 2009-10-24
- score: 1

Cloud hosting and data center companies are professional companies that earn their bread-n-butter through providing these services. "For a startup"  , It is safer to host the data at one of these companies than to manage it yourself on counts of uptime, cost efficiency , reliability, flexibility and even data security. I also agree with Alex that a redundant copy of the same needs to be maintained locally as well. The beauty and bane of digital data is that it can be copied easily and backups maintained. 


## Answer 3703

- posted by: [Darius Dunlap](https://stackexchange.com/users/-1/1470-darius-dunlap) on 2009-11-16
- score: 0

All good advice... especially regarding backups & encryption.

I'll just add a point regarding security: 

Enforce secure connections. Most systems can be set this way, to require https: and SFTP, for example. This is even a good idea for things like your blog platform control panel and other such "non-critical" resources.


## Answer 4833

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2009-12-09
- score: 0

If they are holding your data/code, you need some agreement where they can place it in escrow and agree to send you backups on DVD's if they go out of business.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
