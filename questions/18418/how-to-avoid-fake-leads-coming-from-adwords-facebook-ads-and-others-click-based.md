## How to avoid fake leads coming from AdWords, Facebook Ads and others click based advertising?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-02
- tagged: `advertising`, `facebook`, `adwords`
- score: 6

I'm experimenting **Facebook Ads** since a week or two as I got very disappointed by **AdWords** recently. But Facebook is acting exactly like AdWords.

> I suspect that most of leads that come from them (I paid for each of them) are generated by an apparently non human system.

I spent a week monitoring each lead that came from them using a special live stats software. I observed their behavior on the website and I noticed some patterns. I compared them to what I call **legitimate users** which also have a specific behavior pattern that is specific to how the website is designed (where the buttons are placed on the screen etc). 

However those I suspect to be **robots** doesn't see buttons. They see text links. The possible automatic system is pretty well designed. When you set "goals", it is able to detect them and systematically go trough them, without any coherent behavior. The only objective seems to generate a click and if possible, match one of the goal you defined in AdWords, then leave the site.

I also measured the difference by comparing download page hits (it's a goal) and actual welcome screen display (when the software is installed, the user is redirected to that page). None of the suspected automatic leads access that page.

Have you experienced the same behavior? How to avoid those fake (and paid) leads?


## Answer 18427

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-02
- score: 7

<p>Ok I answer my own question. I hope it will be useful to others.</p>

<p>My suspicion was correct. Here is how they do it:</p>

<ol>
<li>They create <strong>bot-nets</strong> by infecting thousands of machine world wide.</li>
<li>They create page full of <strong>AdSense contextual Ads</strong>.</li>
<li>They <strong>control their bot-nets remotely</strong> to access their pages and "<strong>click</strong>" on the ads.</li>
</ol>

<p>Google <em>is working</em> on the problem since a long time. <a href="http://adwords.blogspot.com/2007/04/new-case-study-on-botnet-based-click.html">Here is a page</a> found on their own website that explains the process. It was published 4 years ago. The process is described in details in <a href="http://www.usenix.org/events/hotbots07/tech/full_papers/daswani/daswani.pdf">this document</a>.</p>

<p>Has Google found a solution to shut them down and therefore reduce dramatically their own profits? Nope.</p>

<p>Here the solution I found from different sources.</p>

<ol>
<li>Click on <strong>Campaigns</strong></li>
<li>Click on <strong>Network</strong> tab</li>
<li>Scroll down and expand <strong>Exclusions</strong> link</li>
<li>Add <strong>domains</strong> to exclude in the box.</li>
<li>If you want to exclude IP Addresses, click on <strong>Manage IP Addresse Exclusions</strong></li>
</ol>

<p>Now how to determine which leads are coming from bot-nets?</p>

<p>Use one of the following methods:</p>

<h2>Method 1 (Manual)</h2>

<ol>
<li>Download and install a <strong>live website tracking</strong> software. I use <a href="http://www.providesupport.com/">ProvideSupport.com</a></li>
<li>Turn on <strong>sounds on "new visitor"</strong> event</li>
<li>Each time a new visitor come in, <strong>watch it's behavior</strong>. With practice, you will identify fake users pretty fast. They also have something in common: they all come from few similar websites.</li>
<li>Exclude those websites in your AdWords account</li>
</ol>

<h2>Method 2 (Semi-Automatic)</h2>

<p>If you want to automatize the process, install some server-side tracking tool that will record referrer from Google and IP Address (it's in the Referrer variable). Check which IP Address subscribed to your newsletter, website, software or anything. Check which referrer generated the lowest conversion rate (I never saw any generating more than 0%).</p>

<p>I prefer to use the </p>

<p>Take this seriously, for each $1000 I invested, almost $950 was junk.</p>



## Answer 18422

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2011-01-02
- score: 2

First and foremost, what you are paying for is **visitors**, not **leads**. This is a critical distinction.

**Visitors** are the people who walk into your store. How many times have you walked into a store, looked around real quick, and then walked out. Maybe it's the store's fault (they words "crackers with your purchase" were not visible between FREE and BEER). Or maybe it's your fault (you wanted to window shop).

**Leads** are *identifiable* visitors who've actually expressed interest. Maybe they tried on some clothes. Maybe they talked to a salesperson. Perhaps they grabbed a brochure. Only some leads turn into sales... again, it could be their fault (no money) or your fault (poor sales ability).

That said, you are **asking the wrong question**. Having done a whole lot of advertising on behalf of software companies, I can say with 99% certainty that there are no robots who are clicking around your site from ads. 

But let's say there are. So what? In the end It's not about ensuring *all* visitors behave a certain way, but a *reasonable percentage*. Determining what the % is requires crunching a whole lot of variables like targeting, copy, goals, design, etc.

In the end, the question you should be asking is, *how can I get more visitors to do this...* And to begin answering that, you need to identify a whole lot of those variables.


## Answer 28520

- posted by: [Volodymyr M. Lisivka](https://stackexchange.com/users/-1/12571-volodymyr-m-lisivka) on 2011-08-09
- score: 1

There are hot areas on web pages: near scroll bar, near to tabs bar, near to embedded flash games, etc. Users can click on ads in these areas accidentally. Page will be valid for Google, but will generate suspicious traffic anyway.

I recommend to visit referred pages and to look at position of banners. If they are in hot areas, then you should ban them, because they will generate lot of accidental visitors.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
