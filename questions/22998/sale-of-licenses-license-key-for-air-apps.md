## Sale of licenses (license key) for Air apps

- posted by: [Astraport](https://stackexchange.com/users/-1/9202-astraport) on 2011-04-06
- tagged: `software`, `payments`, `licensing`
- score: 2

How (what services use) to better organize the protection, payments, sending license keys for shareware Air applications?


## Answer 23000

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-04-06
- score: 2

<p>I'm the owner of the company that makes <strong><a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a></strong>. We have a fully written example showing <a href="http://wyday.com/limelm/help/using-turboactivate-with-adobe-air/" rel="nofollow">how to add licensing to Adobe AIR apps</a>. LimeLM handles all the details for you. Plus you can use <a href="http://wyday.com/limelm/help/api/" rel="nofollow">our web API</a> to integrate the key generation into your website order process. We have full examples for PHP and ASP.NET so you don't have to write it all yourself.</p>

<p>Our type of licensing is hardware locked licensing. In other words LimeLM is a lot like Windows activation or Microsoft Office activation. You send a user the product key they enter it in your app, then you call an "Activate" function that sends the product key data along with a "fingerprint" of the computer. LimeLM then sends a cryptographically signed verification back to the user's computer. This "activation" locks the product key to the computer. That is, a user can't go use the product key on 50 other computers.</p>

<p>Of course you can make it easy for the user to move your product from one computer to another using "deactivation", but the point is the hardware-locked licensing (aka online activation) gives you complete control over the entire licensing process.</p>

<h2>Do it yourself</h2>

<p>If you have more time than money you can always develop this yourself. Obviously I would prefer you just <strong><a href="http://wyday.com/limelm/signup/" rel="nofollow">signed up for LimeLM</a></strong> (we even have a free plan), but I also know when you're just starting every penny counts. Plus, some of our biggest customers are companies (and individuals) who went down the "build it in-house" path and are glad to hand off the responsibility to us.</p>

<p>There's a huge amount of work that goes into making a licensing product, but the grand overview of hardware-locked licensing is this:</p>

<ul>
<li>Create a native library (aka a *.dll on Windows, *.dylib on Mac, *.so on Linux) that can create a unique hardware fingerprint based on all the components of the computer (motherboard, CPU serial, graphics card, memory serials, etc, etc.).</li>
<li>This library should also be able to verify product keys created using <a href="http://en.wikipedia.org/wiki/Symmetric-key_algorithm" rel="nofollow">Symmetric-key cryptography</a> (e.g. <a href="http://en.wikipedia.org/wiki/Advanced_Encryption_Standard" rel="nofollow">AES</a>).</li>
<li>Use <a href="http://en.wikipedia.org/wiki/Public-key_encryption" rel="nofollow">Public-key cryptography</a> on your servers to cryptographically sign the product key and hardware fingerprint. This "signed" response is then sent back to the user. Then you can check if the user is "activated" or not if the signed message is verified (this time you're using the other end of public-key cryptography).</li>
</ul>

<p>The great thing about <a href="http://en.wikipedia.org/wiki/Symmetric-key_algorithm" rel="nofollow">Symmetric-key cryptography</a> is that it creates small keys (e.g. ABCDE-FGHIJ-KLMNO-XXXXX) and the <a href="http://en.wikipedia.org/wiki/Public-key_encryption" rel="nofollow">Public-key cryptography</a> for all intents and purposes cannot be forged. Using the in tandem will ensure that your licensing design isn't the weak point in your protection.</p>

<h2>Hackers, crackers, and thieves</h2>

<p>You didn't ask about cracking, but I might as well bring it up. Nothing that exists on a computer is uncrackable. That being said, casual piracy (that is, a person or company using the same product key over and over again) is a greater threat to your business than crackers. So you should always use hardware-locked licensing (like <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a> or the "do-it-yourself" method described above) rather than just simple "serial" protection.</p>

<p>The way you handle crackers is to find all pirated versions of your software on the web and send DMCA notices. A very high percentage (> 90%) of these hosting sites remove illegal files based on DMCA requests. But it's a whack-a-mole proposition. That is, when you get 20 sites to remove your files, 20 more pop up the next week. </p>

<p>We've thought about this problem too, which is why we created <a href="http://wyday.com/pirate-poacher/" rel="nofollow">Pirate Poacher</a>. This is a service we offer (free for LimeLM customers) that handles the tracking &amp; removing of pirated versions of your software for you.</p>

<p>Tell me if this helps.</p>



## Answer 45320

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2012-12-28
- score: 0

I am currently looking into this and it comes down to a basic choice between bespoke solution of third party solution.  In the first instance I will be going for the latter.  As far as I can see the providers in this space are LimeLM (who have replied here) but alos Excel Software's AirLicense, NitroLM and Zarqon.  

I am in the process of contacting all of them to see how responsive their support is... I need a solution which i can implement either without major technical skills or hand over to someone with those skills and a clear set of instructions.

I will post more when i know more if anyone else is interested.

RomanCat




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
