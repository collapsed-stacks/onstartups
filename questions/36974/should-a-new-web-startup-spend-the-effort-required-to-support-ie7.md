## Should a new web startup spend the effort required to support IE7?

- posted by: [Mike Christensen](https://stackexchange.com/users/-1/16340-mike-christensen) on 2012-03-08
- tagged: `website`, `webdev`
- score: 2

I'm currently in the final testing stages of launching the release version of my website.  Over the past couple days, I've been testing the entire site on IE7 as it's a browser I would *like* to be able to support, though it's not one I run myself.  It's becoming increasingly clear that the level of effort required to fully support this browser will be quite high.  It will probably be at least another week of full time work before I can have the major issues worked out.  First off, the browser itself is slow and unstable.  A lot of the bugs I run across are extremely hard to track down, cause either the browser itself or the debugger to actually crash, or do not actually repro under the debugger due to weird timing issues.  My frustration levels are near volcanic eruption at the moment.

The obvious answer to this question would be "Well, it completely depends on your target audience."  My site is a cooking related site, and according to Google Analytics, is mostly used by middle-aged housewives with kids.  IE is definitely the most commonly used browser, however the statistics I collected during the beta release showed that only between 3 and 4% of my users were on IE7.  The majority were either IE8 or Firefox (yay for techie housewives!)

**My Questions:**

1. Are new consumer oriented web startups bothering with IE7 support?
2. Is there a rough formula or rule to determine at what point it's no longer cost-effective to support a certain browser?
3. Would it be a reasonable compromised to get the site *basically* working under IE7, with perhaps a few minor cosmetic bugs but still functional?  Note that this of course increases the test-matrix for *future* development work.

I'd love to hear any feedback.


## Answer 36975

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2012-03-08
- score: 2

<p>In my experience, there are two cutoff points that make sense:</p>

<ul>
<li>IE 6 and never</li>
<li>IE 8 and never</li>
</ul>

<p>I practically never see IE 7 in logs. IE 6 used to be 'the corporate standard', but companies almost completely ignored IE 7. And most corporate desktops now have IE 8 or IE 9, though a few admittedly are still on IE 6.</p>

<p>IE 8 is the new IE 6, in the sense that it must be supported due to its market share, but web designers will groan because it is missing many key technologies (CSS3, HTML5 only via Javascript shims, etc).</p>

<p><strong>And then about supporting IE &lt; 8:</strong> Well, I personally would not bother because today <a href="http://www.ie6countdown.com/" rel="nofollow">IE 6 is almost exclusively used in rural China</a>. Due to the geographical &amp; cultural distance most of these people won't shop on your site anyways.</p>

<p>I did notice that you wrote that up to 4% of your target audience might be using IE7. I would still not support IE 7, it really never took off in the market. Those IE 7 users are most likely private individuals who can freely install a more modern browser, they just don't know it. I would suggest to:</p>

<ul>
<li>Use <a href="http://www.quirksmode.org/css/condcom.html" rel="nofollow">IE conditional comments</a> to selectively show your IE &lt; 8 users a banner linking to <a href="http://www.beautyoftheweb.com" rel="nofollow">http://www.beautyoftheweb.com</a></li>
<li>Write a FAQ entry about which browsers get A-grade support, and which get B-grade; inspired from <a href="http://yuilibrary.com/yui/docs/tutorials/gbs/" rel="nofollow">Yahoo!'s graded browser support for YUI</a>.</li>
</ul>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
