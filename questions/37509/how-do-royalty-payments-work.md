## How do Royalty payments work?

- posted by: [7wp](https://stackexchange.com/users/-1/10600-7wp) on 2012-03-24
- tagged: `payments`, `business-model`, `accounting`, `billing`, `royalties`
- score: 3

I have been asked by another company to build them some software to operate some machinery.  

The company sells this machinery to their own customers and wants to provide the software I write along with the machinery they sell.

I could charge the company one lump sum to build them this software, they will own all resell rights.

However there could be another option.  They don't pay anything up front for the cost of the development of this software, instead they pay some agreed upon royalty fee for every copy they include with every unit they sell.

That way the company does not lose any money if they don't sell a lot of units, however, if they do sell a lot of units, well the company makes money and so do I.

The question is, if the company should agree with such an arrangement, how can it be enforced?   The company might sell 10 units in a year (they are very expensive) and report back to me that they only sold 5 so that they don't have to pay me as much royalty fees.

I guess it would work on trust, but when it comes to money and human beings, trust only goes so far...

I understand that the radio business does something similar for music they play on the radio, they keep track and pay royalties to the artists.

I'm wondering how this sort of thing can work with software, and how does one enforce the policy to make sure the company is not cheating.



## Answer 37532

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2012-03-25
- score: 2

The standard way is to (1) have a precisely defined royalty and (2) detailed computation of the royalty, combined with an audit right.

In most contracts calling for a royalty to be paid on IP, payments of royalties usually happen on a periodic basis -- monthly, quarterly, annually, whatever.  As part of that, the licensee usually has to give an accounting of how the royalty was calculated.  On top of that, the licensor usually gets an audit right -- the right to go in (or, actually, to have an accountant go in) and look through the licensee's records to ensure that they're paying the correct amount.

Recognize that there are several ways to cheat.  You've identified one: just fibbing about the number of units sold.  Another is in the calculation of the royalty itself -- often, the royalty is x% of sales AFTER a bunch of line items.  Each of those line items is an opportunity for the licensee to reduce your royalty.  Another way to cheat is to sell the product with other products or services and allocate most of the revenue to those other products or services, instead of to the licensed product where it belongs.




## Answer 37510

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-03-24
- score: 1

First off if it is a major company (say a Fortune 100) selling high priced industrial machines they will not want to risk getting sued for cheating you out of commissions. It is too easy to prove your case.

Since the machines are high priced, do they have serial numbers? If so ship the software directly to the customers yourself and license it for use on that serial number machine only. You can also include a licensing dongle if you like so that your software will not run without the dongle.

You may want to also charge the customers an annual maintenance fee for software upgrades. Once again ship the upgrades directly to the customers yourself and once again tie the upgrade to the particular serial number so that it can not be used to upgrade any other copy.

People who buy million dollar industrial machines are quite used to such practices as well as paying substantial ongoing maintenance fees. This is not consumer software.


## Answer 37512

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-03-24
- score: 1

First- there is a third option you have not mentioned. You get paid a fixed amount to write the software, and then a royalty on each unit sold. The payment does not cover all your costs in writing the software but does ensure you get something from the deal and that the other party is serious about the deal.

The answer to your question is: **You must have a written contract** with the company that spells out all rights and obligations. It will **require** a lawyer *(on both sides)* to negotiate this contract. We have done this hundreds of times with our software products *(we have standrd license agreements specifically for our products.)*

Things to look out for:

 1. Indemnity- will the other party protect you if they are sued when their machine does something bad.
 2. Specify exactly what the royalty payment is based on.
 3. Specify how often the royalty payment is made, what the penalties are for late payment, and give you the right to audit their books to ensure the royalties are correct. *(Typically you pay for the audit, and if they under report sales by x% they have to pay for the audit, plus of course pay back royalties.)*
 4. One nice item tom add is something to prevent them from writing the same software themselves and then dumping you. *(This often happens if your software becomes a big success- they can then afford to write the same software and stop paying you.)*



## Answer 37520

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2012-03-25
- score: 0

<blockquote>
  <p>I'm wondering how this sort of thing can work with software, and how does one enforce the policy to make sure the company is not cheating.</p>
</blockquote>

<p>There are 2 ways to enforce how your customer use your software: contractually and technologically. You should use both methods in tandem. Gary E covered the legal and written-contract side of things, so I'll just cover the technological way of enforcing how your customers use your software.</p>

<h2>(Technologically) Enforcing how your customers use your software</h2>

<p>The way you limit how many times your customers install your software is by using "hardware-locked" licensing. I'm founder of the company that makes <strong><a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a></strong> (hardware-locked licensing for Windows/Mac/Linux/etc.), so obviously I'm going to recommend you go with our solution. But I'm also going to describe how to build this yourself. And I can go into further detail if you want.</p>

<p>The most commonly used method of hardware-locked licensing is online activation. This is what greater than 99% of end-users of companies using LimeLM use. There are other variants of hardware-locked licensing ("offline" activation, dongles, floating licensing, etc.). However, for most companies, online activation is the best bet.</p>

<p>Most people have encountered the "online activation" type of licensing when they purchase a copy of Microsoft Windows or Microsoft Office.</p>

<p>When a customer uses well designed online activation it looks nearly identical to “serial-only” licensing. That is, the customer buys a copy of your software and gets a 20 to 30 character serial number like “ABCD-EFGH-IJKL-MNOP-…”. The customer enters this serial number into your program or your program’s installer. Then, when the user clicks an “Activate” button, some “magic” happens behind the scenes. Your app will either let the customer use your app on that machine or your app will tell the customer to buy another license.</p>

<h3>What’s the “magic” behind online activation? (a.k.a. how to build it yourself)</h3>

<p>If you don't want to buy a 3rd party licensing solution like LimeLM, you can always build it yourself. But what you build has to be technologically sound.</p>

<p>The broad overview of how any well-designed online activation licensing system works is like this:</p>

<ul>
<li>Your customer enters a serial (e.g. “ABCD-EFGH-IJKL-MNOP-…”).</li>
<li>Your software generates a “fingerprint” to uniquely and anonymously identify the customer’s computer.</li>
<li>This serial and the computer's unique "fingerprint" are sent to an activation server.</li>
<li>If the server allows the activation then the serial &amp; fingerprint are cryptographically signed and sent back to the user.</li>
<li>Based on this cryptographically signed block your app or installer will know whether the user is allowed to use your application or not.</li>
</ul>

<p>The whole activation process is a huge topic that can get exceedingly technical. This is the condensed version. The hardware "fingerprinting" in itself is a gigantic topic. There are a thousand wrong ways to do it (using an IP address, MAC address, etc., etc.).</p>

<p>The best way to get a fingerprint for a computer is to use every piece of hardware in the computer (RAM, CPU, motherboard, bios, primary hard disk, networking card internal details, etc., etc.).</p>

<p>If you want me to go into further detail, just ask.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
