## DNS Hosting Services

- posted by: [Terence Johnson](https://stackexchange.com/users/-1/2378-terence-johnson) on 2010-02-04
- tagged: `hosting`, `domain`, `dns`
- score: 5

Can you recommend a good DNS hosting service?

I'm looking for a happy median between the free (and not reliable) providers and the staggeringly expensive ones.


## Answer 7609

- posted by: [roacha](https://stackexchange.com/users/-1/802-roacha) on 2010-02-04
- score: 5

We use DNSMadeEasy and it is very smooth.  Reasonably priced and they have not had any downtime in 2 years.  We also use they for our SMTP mail as well which makes things easy.


## Answer 7618

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-02-04
- score: 4

<p>For some reason, I'm a bit of a DNS geek, and have followed this area for years.</p>

<p>DNS hosting is basically a solved problem, i.e. it is not that hard to build a good DNS infrastructure and get perfectly good speed and reliability. There are quite many good providers out there.</p>

<p>In addition to the good answers already given, I'd like to mention <a href="http://www.gandi.net" rel="nofollow">Gandi</a>. Their DNS servers are not <a href="http://en.wikipedia.org/wiki/Anycast" rel="nofollow">Anycast'ed</a> (i.e. no multisite with the same IP addresses BGP routed for failover and speed), but they have been perfectly reliable and responsive for me for years. They have 4 things that I like:</p>

<ol>
<li>You can <strong>register domains</strong> in most top level domains (TLD) with them. They can be a one-stop shop for all your domain needs (as long as you don't need the exotic TLDs).</li>
<li>They are <strong>cheap</strong>. Hosting DNS doesn't cost anything, it comes free with registration.</li>
<li>Their web interface is fairly <strong>simple to use</strong>. And DNS experts can skip the web interface, and edit the BIND zone file directly.</li>
<li>They have <strong>spam filtering</strong>. For the <a href="http://www.kloth.net/services/whois.php" rel="nofollow">domain ownership information</a> they publish an alias for your real email, and  this alias is valid but spam filtered. Quite nice, since whois records are a major spam-source.</li>
</ol>

<p>In addition to Gandi, I would suggest <strong>DNSMadeEasy &amp; DynDNS &amp; EasyDNS as other good recommendable providers</strong> (no particular order, their services and prices differ a bit, take a look around).</p>

<p>If reliability is a major decision point, maybe I'd say DNSMadeEasy looks a bit better than Gandi, and <strong>DynDNS Dynect</strong> seems best of them all. But note, that's just based on their implementation and past performance, I cannot make any promises for future performance.</p>



## Answer 7602

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2010-02-04
- score: 2

<p>We've used <a href="http://zoneedit.com" rel="nofollow">ZoneEdit</a> at Smart Bear for years.  No down-time and not expensive.</p>

<p>If you do your own DNS someday they can also act as DNS backup.</p>



## Answer 7603

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2010-02-04
- score: 2

DynDns has a good paid offering with a SLA: <http://www.dyndns.com/services/pricing/#dns>.  At $300/year it does not seem very expensive, and does offer a SLA, so it's better than self-hosted.

My knowledge about this is limited though, there might be other hosts out there who can beat this deal.

You could ask in <http://ServerFault.com>, they for sure can give you more options. Outsourced DNS services is not something us normal folk use very often, so you will probably have better luck in ServerFault.


## Answer 7699

- posted by: [Doug Martin](https://stackexchange.com/users/-1/2126-doug-martin) on 2010-02-05
- score: 2

<p>I've used several DNS hosts, including ones mentioned on this list.  The one I like best is Nettica (<a href="http://nettica.com" rel="nofollow">http://nettica.com</a>).  Great interface and great pricing.</p>



## Answer 7623

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-02-04
- score: 1

DynDNS, without a doubt.  I did some consulting work for them a few years back and no the service well.  Great redundancy, great customer experience.


## Answer 7625

- posted by: [Apollo Sinkevicius](https://stackexchange.com/users/-1/2119-apollo-sinkevicius) on 2010-02-04
- score: 1

I have used DNSmadeEasy for hosting DNS for some productions systems we ran. It has that nice failover feature and customizability. Price is right too.


## Answer 9133

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-03-11
- score: 1

I've been using DNS Made Easy for years now and have been very happy with the service they offer. I've been pretty impressed with the progression of the service over the years they have really increased network speed and are doing an excellent job.  For the price that they offer DNS services I find it sickening that these other companies get away charging so much for their services...




## Answer 20362

- posted by: [shaymus](https://stackexchange.com/users/-1/5401-shaymus) on 2011-02-17
- score: 0

<p>I just found out about <a href="https://dnsimple.com/" rel="nofollow">DNSimple</a>, checked them out and their service looked awesome. The UI is fantastic, just 2 screens, so makes registration ridiculously easy to setup and manage. Transferring my domains from GoDaddy to there as we speak. </p>



## Answer 32445

- posted by: [clyfe](https://stackexchange.com/users/-1/14346-clyfe) on 2011-11-10
- score: 0

https://entrydns.net/ is a free DNS service I built in my spare time together with a sysadmin friend.

We hope to support it via donations and/or unobtrusive affiliate sales, and add more features in the future. Give it a try.


## Answer 8078

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-02-15
- score: -1

<p>You can also get the web hosting service here <a href="http://www.thewebpole.com/" rel="nofollow">http://www.thewebpole.com/</a>   @ cheap price..
It has three hosting plans..such as economy, deluxe and unlimited hosting package..If you need , get it from this..It provides the web hosting service from the starting price is $3.99 ..visit for more details..</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
