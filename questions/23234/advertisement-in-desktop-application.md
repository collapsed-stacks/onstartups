## Advertisement in desktop application

- posted by: [Arnon](https://stackexchange.com/users/-1/9332-arnon) on 2011-04-12
- tagged: `advertising`, `adwords`
- score: 2

I built a small and cool java-base desktop application.<br>
I want to release it for free, and put an advertisement for getting profits out of it -
Like <a href="http://www.evernote.com/">EverNote</a> doing on their Mac OS X App.

I don't want to sell the advertisements by myself(too much work, and I have no idea how to do it), but to use service like Google AdSense.<br>

My idea is to put a small browser component (like <a href="http://help.eclipse.org/helios/index.jsp?topic=/org.eclipse.platform.doc.isv/reference/api/org/eclipse/swt/browser/package-summary.html">org.eclipse.swt.browser</a> or the Web-Browser component from The DJ Project) at the bottom of the window and load a HTML page that include just the advertisements ads.
<br>
Well,  to do this, i rent a host (at Dreamhost if it matter...) create a simple blank HTML page on it, and try to sing up for Google Adsense.
<br>
As you can guess Google didn't approve the my request(for singing up), because the page is too empty...

So, now i need a recommendation for a good ads service that allow my to put the advertisements on my application.<br>
<b>Any suggestions?</b>


## Answer 23236

- posted by: [Fernando Martins](https://stackexchange.com/users/-1/1778-fernando-martins) on 2011-04-12
- score: 0

Get in touch with companies that do web advertisement and deal directly with them.
You may even specify what's your application about so that they can filter the ads to fit the possible user profile.


## Answer 23238

- posted by: [Kort Pleco](https://stackexchange.com/users/-1/7876-kort-pleco) on 2011-04-12
- score: 0

It's against the google adsense ToS to display ads in anything that's NOT a webpage, like to load the ads in a desktop or mobile application. The caveat is only if they're loading in a browser window that can navigate to other websites too. 

So you can put together a real website to load the ads on, but make sure that you're loading the ads an operational browser and not just displaying the banner ad. 

Sponsors are another option, or you can look into disabling some features unless you buy a premium version of your program. I decided to go the premium version route in my desktop application (C#), and I even built another program that does different things that I'm offering to free, as the audiences are similar for the programs, and it has my own advertisement for my paid program. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
