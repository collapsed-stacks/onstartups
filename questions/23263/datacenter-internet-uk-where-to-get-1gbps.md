## Datacenter internet UK? (Where to get 1GBPS?)

- posted by: [joesavage](https://stackexchange.com/users/-1/9331-joesavage) on 2011-04-13
- tagged: `internet`, `uk`, `data-request`
- score: 2

I'm planning to have one good server computer (Intel Xeon processor) running some linux server distro handling all the files for my file hosting website. I can buy it plenty of space (I assume I can just buy it huge hard drives) so that it will last the site's lifespan, and hopefully using 100% of the hardware and internet should give good speed for users downloading files.
My issue is that I'm not sure how fast internet I'll need (obviously I'll need something with unlimited broadband, fast upload, and fast download speeds).
How fast do you think I'll need? And do you recommend any companies in the UK that would be able to offer these services for "fairly cheap"? (Preferably <£70 a month)


Thanks,

Joe


## Answer 23265

- posted by: [Jeremy McGee](https://stackexchange.com/users/-1/1152-jeremy-mcgee) on 2011-04-13
- score: 2

<p>Rather than get (and maintain) your own hardware, better to go for one of the hosting firms out there. </p>

<p>You've two general options: renting your own server or renting a virtual instance. Until you're well established I'd strongly recommend renting a virtual instance -- you can start small and grow, and it's much cheaper until your traffic gets to the stage where you should be generating enough money to afford something bigger!</p>

<p>Amazon are a huge player in this market (see <a href="http://aws.amazon.com/ec2/" rel="nofollow">Amazon Web Services</a>) and have a data centre in Dublin that works just fine for the UK and Europe. For something tiny, though, they're quite expensive.</p>

<p>Alternatively, a less expensive option might be to go for something like the Miniserver at <a href="http://www.memset.com" rel="nofollow">Memset</a>. £10/month +VAT gets you root on a 512Mb box with 20Gb and 50Gb transfer/month - they have a range of packages that scales up, all the way to a network of full servers if you find you need to go there. I've no affiliation with them other than as a happy customer.</p>



## Answer 23491

- posted by: [Matt](https://stackexchange.com/users/-1/8784-matt) on 2011-04-16
- score: 2

**You're seriously misunderstanding how broadband, hosting and websites work.**

Let's say you get 8Mb broadband.  (20M broadband or cable isn't much better than this example)

In the UK on a home class line you get at best 8Mb Download **448k Upload**.
Upload is the speed YOU send data to the internet.  In other words it is the maximum possible speed your website visitors (ignoring more than one at once) can download a file from your site.  You'll be pleased to know upload is almost never included in the data transfer limits by broadband providers.

You **can** run your own server over broadband, but this is typically for light traffic or hobby sites.  You'll be limited to normal broadband speeds and contend with the fact it is a shared service - your users will be sharing that 448k upload speed with other users of your website, and any other traffic on your broadband block.  I have no idea what broadband contention ratio is these days.

The other way of hosting at your own premises is via a leased line.  They are ridiculously expensive, so we'll completely ignore those.

You could go SDSL or VDSL which give faster upload speeds - Upload 2M to 10M at best and £300+ per month.

Look at http://www.zen.co.uk or http://www.spitfire.co.uk for SDSL/VDSL providers.  Both are business grade providers with good reputations.

So, the only affordable option left is web hosting at a data centre...

 - You can have a "colocated" server at
   a web hosts' data centre - You
   own/rent the server at their
   premises.  They may handle backups. 
   They will have tools for you to manage it remotely.
   They have a chunk of backup power,
   fire extinguishers and the like.
 - You can have a "VM" server at a web
   hosts' data centre - Same as above,
   but cheaper, as you only get a
   **part** of a server.
 - You can have a webhosting package -
   You get some shared space on their
   server, but won't decide what it runs
   outside their defined limits (for instance you won't be choosing your own Apache modules).  **They
   will almost certainly exclude file
   downloading hosts in their Ts & Cs**

With colocation you almost NEVER get the opportunity to buy your own hardware and send it to them - you choose one of their own offered servers - from their point of view it's the only sane option.  It makes replacement and repair feasible if they are all the same make.  From an admin point of view, all being on the same OS means they can offer backups and the like.

A VM server is probably your easiest and most cost effective option.  I'd look at http://www.memset.com/ as Jeremy suggested.


## Answer 23282

- posted by: [edralph](https://stackexchange.com/users/-1/9362-edralph) on 2011-04-13
- score: 1

**Try RackspaceCloud** for easy online management of server instances with a transparent pricing model that will scale with your needs and very well supported.  Top tier hosting company.

http://www.rackspace.com/cloud/

Sounds like I work for them doesn't it (I don't, I just use their services and I'm pleased with them)


## Answer 23271

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2011-04-13
- score: 0

<p><strong>Your needs and your willingness to work don't meet up.</strong> You want a "large file hosting service" and "to handle a LOT of people". Yet your planning for scalability and server resources doesn't involve doing basic math to calculate required line speed, and your budget is &lt;70£ / month.</p>

<p><strong>Here is some info I hope can be of help:</strong>
Two of the leaders in cheap Internet connectivity for bulk data transfers (cheap, lower quality bandwidth measured on uptime, latency, and route diversity) are <a href="http://www.he.net/" rel="nofollow">Hurricane Electric (HE)</a> and <a href="http://www.cogentco.com/" rel="nofollow">Cogent</a>. I'm not sure you can connect to any of those in the UK; look towards the USA which is the world's best market for cheap bandwidth.</p>

<p>If you're paying less than about 1 USD per MBit per second (i.e. less than 1000 USD/month for a 1 Gigabit connection), then you're probably getting lower quality network -- for example Cogent.</p>

<p>There are providers who specialize in high-bandwidth cheap hosting, f.x. <a href="http://www.fdcservers.net/specials.php" rel="nofollow">FDC Servers</a> who right now offer 1 Gbit for 700 USD/month. If you need additional names in cheap bandwidth, then the <a href="http://www.webhostingtalk.com/" rel="nofollow">Web Hosting Talk.com</a> forums are usually the best place on the Internet to inquire about cheap hosting.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
