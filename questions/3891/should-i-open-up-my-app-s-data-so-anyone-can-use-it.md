## Should I open up my app's data so anyone can use it?

- posted by: [Codebeef](https://stackexchange.com/users/-1/1594-codebeef) on 2009-11-20
- tagged: `website`, `strategy`
- score: 3

I've built a site for climbers - a worldwide, user editable guidebook for climbers.

Recently, I've been toying with the idea of making all of the data that has been submitted to my site open (Creative-Commons) to everyone in the form of a downloadable archive and/or an API.

My thinking is that if I make the data available in a similar way to how Stack Overflow already does, then more climbers will be motivated to contribute, and more interesting uses of the data will come to light.

My only concern is that I may inadvertently kill my site to death by overlooking some glaring reason that this is a bad idea.

So my question is: Is opening up the data a good/bad/stupid/dangerous idea, and why?



## Answer 3901

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-11-20
- score: 5

<p>Open it now.</p>

<p>Remember you can always close it later if it's a problem (unlikely).</p>

<p>Techniques to deal with your worries:</p>

<ul>
<li>Limit the amount of API activity by IP address.</li>
<li>Require the user supply an "application name" with the API call so you can track apps that are using a lot.</li>
<li>If direct API use becomes a problem, do like StackOverflow and make "database dumps" available periodically over BitTorrent or some other "more free" service.</li>
<li>Put your data up on <a href="http://infochimps.org" rel="nofollow">infochimps.org</a>.  Free or not-free.  Either way, those guys pay for the bandwidth.</li>
</ul>



## Answer 3907

- posted by: [mrflip](https://stackexchange.com/users/-1/414-mrflip) on 2009-11-20
- score: 4

<p>infochimps.org is definitely the best venue for a bulk database dump, whether it's for free under a share-alike license or for pay with a "do whatever you want but don't build bouldr-only-different.com" clause. </p>

<p>We're soliciting entries for our Everything Jukebox: datasets with say "<code>geolocation</code>" on the left hand column and "everything about something" on the right hand columns -- in this case, "places to go climb and all attendant metadata".</p>

<p>What happens when this is out there? Nobody knows! It's the internet! But here are some plausible outcomes:</p>

<ul>
<li>Someone uses the data to build an iPhone/Android app for the site</li>
<li>One of your users ties it to <a href="http://infochimps.org/collections/aggdata" rel="nofollow">datasets from aggdata.com</a> with every REI, Walmart and Sporting Goods store in the country - now you have a "where to get gear" feature for your users and a natural focal point for advertising SEO.</li>
<li>Someone builds a connector to Twitter's new geolocation API and boom: social networking layer for your site.</li>
<li>A grad student studying public health is able to combine your site's data (as a measure for "popularity of alternative sports") with other public data to understand patterns of fitness and exercise.</li>
</ul>

<p>Some of these don't make you money, and some depend on others paying it forward as well. It's hard to explain why this is a good idea, though I think most people have a sense that it is. </p>

<p>But I do know two of the fundamental impulses that make people add content to your site are 1) the joy of sharing their passion and 2) the marginal utility they realize from other people building on the asset they helped improve. That means the best way to encourage contribution is to 1) make that story as widely available as possible, and 2) make the scope for incremental improvements as broad as possible. (Or as the philosopher Earl Hickey said, "do good things and good things happen to you").</p>



## Answer 3892

- posted by: [Brian Swanson](https://stackexchange.com/users/-1/1150-brian-swanson) on 2009-11-20
- score: 3

While content is what brings people to a community-driven site, it's not what keeps them there.  The community and relationships they build on that site are typically what bring them back time and time again.  Your content is of value, but it's the people creating it that can't be replaced.  This is why StackOverflow and other sites offer their information under Creative Commons License.  By doing so they are helping spread the valuable information that they have collected, and they know their community is really what makes their site worth coming too.


## Answer 3920

- posted by: [Amos](https://stackexchange.com/users/-1/1558-amos) on 2009-11-20
- score: 3

Open it.

Invite suggestions, extensions and inventions from the "community" as mrflip says who knows where it will lead. Get people onboard, there are various sites around with suggestions about how to build online communities, have a look at them.

If you inadvertantly kill the site, then start again, taking in to account whatever killed your project the first time around.

What have you got to lose? 

EDIT: I've had a quick look at your site, you've already got the start of a community, advertise it at the climbing walls round the North West, organise some get togethers, organise a meetup for some beers, basically open it and sell it to everybody you meet.


## Answer 15296

- posted by: [Eugene Osovetsky](https://stackexchange.com/users/-1/4870-eugene-osovetsky) on 2010-10-19
- score: 1

Opening your data is a great idea, as long as you do it in a *controlled* way:

 - You may want to control how much data you give out, to prevent someone from just stealing all of your data and just duplicating your site
 - You may want to put a license agreement in place for users of your data
 - You may want to only give the data to someone with a verified identity (e.g. email, telephone, etc), so that you can enforce the license agreement
 - **Most importantly**, you'll want to know exactly who's using the data (name, company, email, etc), because people who use your data are some of your best potential business partners, potential customers, etc. 


## Answer 6171

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-01-08
- score: 0

Open it up. Reminds me of the book: What Would Google Do?



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
