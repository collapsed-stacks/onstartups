## Mobile platform of the future

- posted by: [kabir](https://stackexchange.com/users/-1/849-kabir) on 2010-03-07
- tagged: `ideas`
- score: 6

We are thinking of launching some applications on the mobile platform. However, I am not sure which platforms we should target among, iPhone, Blackberry, Symbian and Android. Any thoughts on which of these would be the dominant players in the years to come ? Any links to site that discuss similar trends would also be useful.



## Answer 8963

- posted by: [Brian Deterling](https://stackexchange.com/users/-1/496-brian-deterling) on 2010-03-07
- score: 6

As Shree said, it depends on your application's target market. As a coder, I also think that design is the hard part - once you have an app functioning the way you want it to on one platform, porting it should not be that difficult and could possibly be outsourced. So I would probably go with the platform that the tech people are most familiar with in order to get something up and running as quickly as possible.

In addition to looking at HTML5 as Shree suggested, I would also look at some cross-platform toolkits like Rhomobile or PhoneGap.

Update: one other thing to consider is that Apple has to approve your app. If your target market is mostly iPhone users, that may not make a difference, but I'd be skeptical of basing my business model on the whims of the app store reviewers. 


## Answer 8964

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-03-07
- score: 3

You might want to approach this question from a different direction. Instead of trying to decide which market will become dominent in the future, ask yourself what is the largest market my company can reach in the next year.

The iPhone has the current largest market, but it also has the most competition **and** the most restrictive selling environment. iPone apps can only be sold through the iPhone store so you are at the mercy of Apple to sell your product.

Android apps have a current smaller market share than iPhones. But there is much less competition between apps and you are not locked into the common company owned store model for selling.



## Answer 8970

- posted by: [Ben Edwards](https://stackexchange.com/users/-1/2786-ben-edwards) on 2010-03-07
- score: 2

Web-based apps, specialized for mobile devices, are going to allow you hit the most devices with the least amount of work/expertise/specialization.  That being said, if you still want native apps, which is probably a good idea, I'd target Android and/or iPhone (unless your target market is especially fond of BlackBerry).  Either way I'd try to make as much of your application web-based as possible.


## Answer 8967

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-03-07
- score: 1

<p>My take, as someone who has worked as a development project manager the mobile industry, is that the dominant mobile platform of the future doesn't exist yet.</p>

<p>I'm from Scandinavia; i.e. Nokia-land. And as such it's clear to me that there are <strong>large regional differences in installed base</strong>. Americans are always talking about Blackberry -- we practically don't have them here. Here are some numbers on <a href="http://theappleblog.com/2009/12/17/iphone-passes-windows-mobile-in-smartphone-os-market-share/" rel="nofollow">US smartphone OS market share</a>, and here <a href="http://www.mobilemonday.net/news/western-european-mobile-phone-market-in-on-move-again" rel="nofollow">on Europe</a>. And Asia is quite different and very diverse as well.</p>

<p><strong>You <em>can</em> write really nice <a href="http://java.sun.com/javame/index.jsp" rel="nofollow">Java ME</a> apps,</strong> and get them to run on many/most devices (not good for iPhone). But there are large differences in screensize, RAM, CPU and everything else amongst devices, so it's <strong>exceedingly hard work</strong> to be compatible with a wide range of handsets.</p>

<p><strong>I used to think PC web-browsers had deep compatibility issues. Hah!</strong> Ooh boy, current PC browser issues are nothing compared to mobile. You <strong>can</strong> make a cross-handset web-page in <a href="http://en.wikipedia.org/wiki/XHTML_Mobile_Profile" rel="nofollow">(mobile) XHTML</a>. But broswer support for CSS, tables and payload sizes (max size of CSS file fx) differs widely, so making it good-looking while retaining compatibility is hard. You could make a page in HTML5 for the iPhone, but support for this format on other handsets is extremely limited right now.</p>

<p><strong>So what to do right now?</strong> I'd say look at your target market, look at what level of interactivity (webpage vs rich application) you need, and do your best while expecting the market to turn at least a couple of times over the coming decade. Be sure to look <a href="http://mobiforge.com/designing/story/mobile-web-design-beyond-simple-xhtml-pages-i" rel="nofollow">outside "applications" and consider fx SMS</a> (texting) as well as email as input vectors.</p>

<p>XHTML webpages will get you the widest audience for least money. You could supplement XHTML with a native app for specific operating systems, the ones that have the highest ROI for your target audience. For iPhone, you could also supplement a XHTML main app with an iPhone-optimized HTML 5 app, for not that much additional development effort.</p>



## Answer 8955

- posted by: [Shree Mandadi](https://stackexchange.com/users/-1/1664-shree-mandadi) on 2010-03-07
- score: 0

Not knowing what applications you are building, Did you try working with HTML 5, All of these Platforms have some decent Browser to access internet, and using HTML5 and some CSS Magic, you could build customized Native look and feel interfaces.


## Answer 44964

- posted by: [Anastasiya](https://stackexchange.com/users/-1/21909-anastasiya) on 2012-12-12
- score: 0

Some people say, Android is a mobile platform of the future http://www.digitaltrends.com/mobile/android-most-popular-platform-2016/ . 
Others are confident that it will be iOS. Anyway, choosing a mobile platform for your business app, you need to consider your target audience,they age and interests, geo location etc. Have a look at the top mobile OS per country http://gs.statcounter.com/#mobile_os-ww-monthly-201211-201211-map 


## Answer 44986

- posted by: [Jon Dobrowolski](https://stackexchange.com/users/-1/22063-jon-dobrowolski) on 2012-12-13
- score: 0

Things are changing so quickly in this space, that 'the future' is vague time frame, and that future is moving faster than you probably will. Think about Amazon's kindle fire taking 23% of market share (Magid Survey number) of tablet in one year... Here are the real tips for making your decision if its a native one:

1. Which platform has the least fragmented install base... Android has so many flavors, and that variance changes a lot of what your able to do. 

2. It's not just about market size. Consumers who use iOS purchase a lot more through their phones than people in the Android market. This is key.


Someone said to me recently that they'd bet Android takes over as the dominant platform, and I mentioned that for the sake of any company wanting to dip a toe in this space, we should hope not. Developing the same app for multiple OS flavors is a headache I'd rather not have. 


## Answer 45024

- posted by: [Sree](https://stackexchange.com/users/-1/22028-sree) on 2012-12-14
- score: 0

<p>In my opinion <strong><a href="http://icenium.com/community/blog/icenium-team-blog/2012/06/14/what-is-a-hybrid-mobile-app-" rel="nofollow">Hybrid Applications</a></strong> have a great future. It makes look &amp; feel like native applications. I had a try with HTML 5, jQuery &amp; CSS3. it works in multiple platforms, and more developments are coming into this. Hope it will be the next trend.</p>

<p>Also I believe <strong>Android</strong> will be the widely using mobile platform in the world!!</p>



## Answer 45029

- posted by: [Dave Hilditch](https://stackexchange.com/users/-1/19968-dave-hilditch) on 2012-12-14
- score: 0

<p>If you want to charge for your app, iOS has the best success rate here.</p>

<p>If you want to distribute your app to as many people as possible Android has the <a href="http://marketingland.com/after-five-years-dominant-android-os-increasingly-identified-with-samsung-26413" rel="nofollow">largest (by FAR) penetration</a> (75% and rising).</p>

<p>If you want to publicly advertise your app, you should write your app for both iOS and Android. Another thing to bear in mind - if it's a social/sharing style app, you'll need to write it for all operating systems if you want it to succeed. There are too many instances of guys with Androids and partners with iPhones.</p>

<p>If you want to use familiar development tools and potentially target desktops with the same app, and potentially dominate a new market, go for Windows 8.</p>

<p>I wouldn't bother with Symbian.</p>

<p>I wouldn't rule out BlackBerry just yet - if it's a business app you're making, you may want to consider writing for their platform as they still have a lot of money to spend and will have learned a lot of lessons from the competition. Their new operating system and developer tools are <a href="http://www.afr.com/p/technology/rim_offers_music_to_the_ears_of_1SNdQUYGC7T8KJg7Xfq5PO" rel="nofollow">coming soon</a>.</p>

<p>As a general guide, Android is the biggest OS and will remain so for the next 3 - 5 years. Apple is losing ground and will lose much more ground over the coming years to Windows 8/Metro. The advance of Microsoft is inevitable as their developer tools are great and the fact that Windows 8 is on every new PC now will allow them to force their way into the market.</p>

<p>My personal best guess is that Apple iOS will be the third largest mobile operating system inside 2 years. I know it's great, I know Apple are huge, but they lose every time because of their <a href="http://www.forbes.com/sites/timworstall/2012/08/31/the-problem-with-apples-closed-apps-universe/" rel="nofollow">closed approach to everything</a>.</p>

<p><strong>My generic advice, for you and others:</strong> develop for the Android operating system as it's the clear winner for the next whoknowshowmany years and if your app succeeds, pay someone to port it to iOS and Windows 8 with the proceeds.</p>

<p>Also - if your developers understand Android, they will be well positioned to write apps for Google Glasses etc when they arrive shortly.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
