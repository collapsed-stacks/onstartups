## How will HTML5 impact the internet landscape?

- posted by: [Birender Saini](https://stackexchange.com/users/-1/5019-birender-saini) on 2010-11-11
- tagged: `development`, `internet`
- score: 2

I attended [Geek Fest][1] today in Charlotte, NC and attended a session from Hunter Loftis ([@hunterloftis][2]) Along with some new cool features of HTML5, I learnt that HTML5 has huge potential for being used for browser games with not-so-basic graphics.. 

How else do you foresee HTML5 changing the internet landscape? Do you all think that most of today's websites will be re-written in HTML5? 


  [1]: http://www1.cpcc.edu/thegeekfest
  [2]: http://twitter.com/hunterloftis


## Answer 16347

- posted by: [deizel](https://stackexchange.com/users/-1/5340-deizel) on 2010-11-11
- score: 3

<blockquote>
  <p>How else do you foresee HTML5 changing the internet landscape?</p>
</blockquote>

<p><strong>As a standard</strong>: I believe more people will be willing to invest in HTML5+CSS3 as a platform, rather than relying on other RIA platforms that are tied to a single vendor (eg. Flash, Flex, Air, Silverlight).</p>

<p><strong>On the desktop</strong>: There will be a greater push to bring web applications to the desktop (either on a traditional PC, netbook or mobile device) or as alternatives to desktop applications. <a href="http://www.google.com/chrome" rel="nofollow">Chrome</a> and Mozilla's <a href="http://mozillalabs.com/prism/" rel="nofollow">Prism</a> allowing you to create desktop application shortcuts to web applications. iOS and Android both have browsers capable of delivering HTML5 and allow developers to specify if web applications should show the browser controls (ie. back/forward/etc) or cover the status bar (ie. go fullscreen). We also have <a href="http://en.wikipedia.org/wiki/Google_Chrome_OS" rel="nofollow">ChromeOS</a> on the horizon which assumes from the start that everything you need is available on the cloud, as a web application somewhere.</p>

<p><strong>Application caches</strong>: HTML5 allows applications to store themselves (the JavaScript client-side code) and their data offline (ie. to disk). This ties in with the last point as, when you take devices like netbooks or mobile phones offline, there is still capability to run the web applications (which exist online) in an offline environment (eg. like <a href="http://mail.google.com/support/bin/answer.py?hl=en&amp;answer=97535" rel="nofollow">Google Mail</a>, without the need for vendor-specific technologies like <a href="http://gearsblog.blogspot.com/2010/02/hello-html5.html" rel="nofollow">Google Gears</a>)</p>

<p><strong>Canvas</strong>: Apart from being used for <a href="http://benfirshman.com/projects/jsnes/" rel="nofollow">games</a> and other obvious things, <code>&lt;canvas&gt;</code> will allow developers to create richer user interfaces. Examples include web applications that look like desktop applications (eg. <a href="http://mochaui.org/demo/" rel="nofollow">MochaUI</a>, <a href="http://mozillalabs.com/skywriter/" rel="nofollow">SkyWriter</a>), more native online mapping (ie. <a href="http://concentriclivers.com/slippymap.html" rel="nofollow">draggable canvas</a>, <a href="http://cartagen.org/" rel="nofollow">vector mapping</a>, <a href="http://cs.smu.ca/~c_adams1/3DEarth3/" rel="nofollow">3D worlds</a>), image manipulation programs (eg. <a href="http://canvaspaint.org/" rel="nofollow">CanvasPaint</a>), and more.</p>

<p><strong>Geolocation</strong>: HTML5 allows web applications to request permission to see your location (provided by your device/browser). This means for example that you don't need to create a native iPhone app for location-awareness, as an HTML5 web application accessed through Mobile Safari can access the GPS on your device also (given permission).</p>

<p><strong>Video Element</strong>: Three words: YouTube, Flash, iPhone. HTML5 gives browsers the ability to play video using the native video player installed on the host OS. This means that installing proprietary browser plugins is no longer strictly necessary to play video.</p>

<p><strong>Web Workers</strong>: HTML5 brings threading to JavaScript, allowing developers to spawn background threads that can do processing without affecting the performance of a web page. Say goodbye to this dialog:</p>

<p><img src="http://i.stack.imgur.com/cM6K7.gif" alt="alt text"></p>

<p><strong>And more APIs</strong>: Native drag and drop between OS and browser allows you to drag files <a href="http://gmailblog.blogspot.com/2010/04/drag-and-drop-attachments-onto-messages.html" rel="nofollow">into</a> and <a href="http://gmailblog.blogspot.com/2010/08/drag-and-drop-attachments-to-save-them.html" rel="nofollow">out of</a> web applications. Notifications API allow web applications to <a href="http://twitter.com/#!/googlecalendar/status/10735753517" rel="nofollow">pop up reminders</a> or IMs/tweets. Web Sockets provide push technology to web applications so instead of continuously polling using AJAX for fresh data, a connection can be kept open to wait for data to be pushed.</p>

<blockquote>
  <p>Do you all think that most of today's websites will be re-written in HTML5?</p>
</blockquote>

<p>Existing sites that want to utilize any of the above features will need to <em>add</em> support for - this doesn't necessarily require a complete rewrite - although newly created websites/startups may take a more wholly approach to HTML5 adoption.</p>

<p>Obviously, not all browsers support these new features yet so graceful degrading is necessary in places still (eg. to Flash for video) until there is a wider adoption of HTML5 by both browser vendors and users.</p>

<p>It is also important to note that since the HTML5 specification is backwards compatible with HTML4, newer browsers actually parse HTML with their newer HTML5 capable renderers these days regardless of whether any of the above features have been implemented.</p>



## Answer 16346

- posted by: [cfrech](https://stackexchange.com/users/-1/5331-cfrech) on 2010-11-11
- score: 2

I'm actually somewhat dubious about HTML5's ultimate impact. Yes, it's a big step forward for a markup language that's been stuck in a "mono-media" state. Yes, it's a boon for open standards and the "open web," but consider also:

* Adoption of the standard will likely be slow and patchy for at least a couple more years. I'd move cautiously on a technology that a good chunk of your audience won't be able to access (at least not fully) for sometime.

* Flash has provided designers and developers with a means of pushing the boundaries of what can be done for years now. Yes, it's in vogue to be be anti-Flash these days, but Flash has offered the capabilities of HTML5 -- and then some -- for sometime. Not to say Flash doesn't have its shortcomings, but I just don't see HTML5 sparking a creative revolution in web design.

* Javascript/jQuery and CSS already offer great enhancements over plain vanilla HTML4. And they enjoy much wider support at the moment.

As for sites being rewritten...maybe. If the site's delivering a lot of Flash-based video and getting on mobile Apple devices is a priority, than yes, rewriting to HTML5 makes a lot of sense. In most cases, though, the juice won't be worth the squeeze.

Bottom line: I wouldn't recommend an entrepreneur invest heavily in this technology, unless he/she fits into the video/Apple mobile camp. Otherwise, wait it out a few years and let the standard 'settle in.'


## Answer 16331

- posted by: [Stark](https://stackexchange.com/users/-1/5338-stark) on 2010-11-11
- score: 1

It's like Internet Explorer, sometimes some components gets updated, but not all of them.

I believe alot of sites will be re-written, but on the other hand, alot of them wont.

Furthermore, I think web designers will become more and more creative with their content and the looks of their site.


## Answer 16340

- posted by: [BhargavPatel](https://stackexchange.com/users/-1/3998-bhargavpatel) on 2010-11-11
- score: 0

HTML5 is great. It has been proven to speed up the loading of websites too! One of the most benefitial thing about HTML5 is that it requires me to type shorter code.. for example..

Now, if I want to type a javascript.. I can just type <script>//Code here//</script> shorter right??

I think it'll take longer for the change because its not mandatory.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
