## Business model for a GPLed software product

- posted by: [Anton Gogolev](https://stackexchange.com/users/-1/3720-anton-gogolev) on 2012-06-29
- tagged: `business-model`, `gpl`
- score: 0

I have a working prototype of a Mercurial repository browser/management tool for Windows and I'm thinking in creating a potential business out of it.

While developing this, I looked a lot inside Mercurial source code and this apparently [makes _my_ code GPL too][1]. This means that even if I sell this tool to someone, I have to redistribute my source code, there's nothing to stop them to go ahead and redistribute source code for free.

Now, to my knowledge Atlassian distributes source code along with its software, but it's not GPL (or is it?) so their source code is protected.

Is it worth trying to start a business _selling_ this software? 

Is it better to build up a consultancy around it? 

Or just opensource it for the geater good?


  [1]: http://programmers.stackexchange.com/questions/151515/rewrote-gnu-gpl-v2-code-in-another-language-can-i-change-a-license


## Answer 40275

- posted by: [PPC](https://stackexchange.com/users/-1/17530-ppc) on 2012-06-29
- score: 3

Taking those questions one by one:

- **Is your software GPL by force**: the GPL (both v2 and v3) state that it "contaminates" the freedom if you use GPL code in your binary. So it totally depends on your interfaces to mercurial. If you copied Mercurial code, or if you link (statically or dynamically) to a mercurial .o, .so, .dll or the like, then yes, you are GPL (or another compatible license, your choice). If you only call it by commandline, RPC, IPC or black magic, then you're free to go. Which doesn't mean it would be a bad move to make it GPL anyway

- **Atlassian**, like many professional tools, ship their source to customers, which is a way to guarantee the software quality. If (as I guess) it comes with a NDA, companies won't take the risk to break it: much to lose, little to win.

- **Nothing prevents you from selling GPL products**, some very successful businesses do (Canonical sells Ubuntu); but they adapt their business model. They often sell maintenance, guarantees, hosting or installation included in the package. Also think in their shoes: if your customers are businesses (which I could guess if they use Mercurial), what would they gain from disclosing source code that they have. The answer is not automatically no, but not automatically yes either. Ask yourself also: what would you lose if they do? It is better for you that people use your product for free instead of another product (you gain visibility, and small for-free customers may lead to big paying customers); it's only bad for you if they use it for free instead of using it for a fee.

- **Customers who have open source SW** in their hands tend to contribute if they find the fix is easier than the maintenance; and generally feel more involved into it. So you can benefit from having customers through code quality and features. Think of Eclipse. Think Mercurial users are geek and many geeks like open-source

**I didn't say** this is a working business model. I say it can, depending on your product, your customers, your/their philosophy, your ideas... As any other business :)

I suggest a lot of reading, Google is your friend.
If you read french: http://blogs.gplindustries.org/node/53



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
