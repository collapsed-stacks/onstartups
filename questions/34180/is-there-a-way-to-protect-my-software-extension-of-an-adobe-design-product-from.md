## Is there a way to protect my software EXTENSION of an Adobe design product from piracy?

- posted by: [Mitya](https://stackexchange.com/users/-1/15255-mitya) on 2011-12-27
- tagged: `software-licensing`, `piracy`
- score: 1

What we are doing at the moment is asking companies how many users they have on site and charging them per user, and then emailing them the extension.

The problem is that there is currently nothing that prevents them from just installing the extension on as many computers as they want.

Is there a good way to set up at least a nominal barrier to keep most people from doing this? I understand it's not possible to stop a determined hacker, but just something to discourage the practice.

Thanks for your help.


## Answer 34199

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-12-28
- score: 2

<blockquote>
  <p>The problem is that there is currently nothing that prevents them from just installing the extension on as many computers as they want.</p>
  
  <p>Is there a good way to set up at least a nominal barrier to keep most people from doing this? I understand it's not possible to stop a determined hacker, but just something to discourage the practice.</p>
</blockquote>

<p>This sums up the casual piracy problem eloquently. And the way you protect extensions to products is the same way you protect full application: <strong>hardware-locked licensing</strong>. But before I continue explaining what hardware-locked licensing let me first correct a common misunderstanding.</p>

<h2>E.T., don't phone home</h2>

<p>I see that Jay made a comment on your question about "calling home" to your servers. This is a common misunderstanding of what proper licensing is. There's a big difference between proper hardware-locked licensing (like online activation) and just "pinging" and server. Just pinging a server to get an "OK" or "Not OK" response is worse than useless. It's actually harmful. But let me first explain why it's useless then I'll continue with an example of why it's harmful.</p>

<p><strong>Why phoning home is <em>useless</em></strong></p>

<p>"Pinging" a server to see how many times a customer is using your software is useless because there's no accurate way of telling which computer they installed it on. That is, many computer can be behind the same IP address, so you can't use that as a "indicator of uniqueness". In fact generating a unique "fingerprint" based on all of the hardware components is the only way to correctly ID computers.</p>

<p><strong>Why phoning home is <em>harmful</em></strong></p>

<p>If you're just "pinging" a server (i.e. you're not using the computer fingerprint and you're not cryptographically signing your results) then there's absolutely no way to accurately limit your users. If you try to limit users based on a "false ID" then they will get enraged when your app suddenly fails to work.</p>

<p>For instance, let's say you used the IP address of the computer as the unique ID of the computer. They install your extension on their computer and everything works fine. <em>Happy customer!</em> At the end of the day they pack up their laptop and bring it home to make a few last minute changes to their work. They get home, open their laptop, start the Adobe product and start using your extension. But they can't because their IP address is different. <em>Angry customer!</em></p>

<p>There are other bad "false ids", of course:</p>

<ul>
<li>The MAC address.</li>
<li>The computer name.</li>
<li>The "volume ID" (partition ID) of harddrives.</li>
<li>Etc, etc.</li>
</ul>

<p>I can list exactly why these are bad if you want.</p>

<h2>Hardware-locked licensing (online activation, dongles, etc.)</h2>

<p>There are many varieties of hardware-locked licensing. There's online activation (à la Windows Activation, Office Activation, or Adobe Activation), there's hardware dongles, and there's floating license servers, etc. But the basic concept behind hardware-locked licensing is the same between all varieties: your app gets the "fingerprint" of the computer and it gets a cryptographically signed response verifying the user has permission to use your app.</p>

<p>But the whole point of getting the computer "fingerprint" and getting the cryptographically signed response from a server is that you can limit how many computers a customer can install your extension on.</p>

<p><em>That is, if a customer buys 5 licenses of your extension they can only use it on 5 computers.</em></p>

<p><strong>How is the "fingerprint" different from the "false IDs"?</strong></p>

<p>A proper "fingerprint" of a computer takes into account all the hardware components of a computer. A good fingerprinting algorithm must have very low false negatives (seeing computers as different when they're really the same) and false positives (seeing computers as the same when they're really different).</p>

<p>If you're going to build hardware-locked licensing yourself then you need to spend a considerable amount of time perfecting this algorithm. This includes buying multiple computers of the exact same model to ensure you reduce chance of false positives. And you need to handle cases where customers modify their computer (thus to reduce chance of false negatives). In other words the customer shouldn't need to contact you if they reformat their computer, or replace a harddrive, or increase their memory, etc.</p>

<p>If you're planning to build this licensing yourself then it can get complicated quickly.</p>

<p>I'm founder of the company that makes <strong><a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a></strong> (a licensing solution for Windows, Mac and Linux), so obviously I'm going to recommend you buy a 3rd party licensing solution (namely us). There are even a couple of our competitors that are worth trying out (and thousands of our competitors that you should avoid like the plague).</p>

<p>Also, see: <strong><a href="http://answers.onstartups.com/a/29055/5714">What's the use of copy protection? (a.k.a. Everything can be cracked)</a></strong></p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
