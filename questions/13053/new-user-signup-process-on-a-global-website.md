## New user signup process on a global website

- posted by: [David Handel](https://stackexchange.com/users/-1/1737-david-handel) on 2010-07-25
- tagged: `design`
- score: 1

What is the best way to handle signups for new users when you want them to register anonymously but identify their country, city and Zip/Postal code?  Some countries don't have postal codes.  I would like to be able to show user location on on Google Maps.  Are then any API's to handle this process in a clean way?


## Answer 13054

- posted by: [Rahul](https://stackexchange.com/users/-1/2109-rahul) on 2010-07-25
- score: 1

<p>You can grab user's IP address during sign up, find out his location based on that IP address and then use the location info for google map.  Here are couple of solutions that you can use to find out location based on IP</p>

<ol>
<li><p><a href="http://www.maxmind.com/app/ip-location" rel="nofollow">MaxMind</a></p></li>
<li><p><a href="http://www.ip2location.com/" rel="nofollow">IP2Location</a></p></li>
</ol>



## Answer 13059

- posted by: [Ross](https://stackexchange.com/users/-1/1390-ross) on 2010-07-25
- score: 1

<p>I can suggest MaxMind and if you use nginx web server <a href="http://wiki.nginx.org/NginxHttpGeoIPModule" rel="nofollow">NginxHttpGeoIPModule</a>
 that can be used with MaxMind.</p>



## Answer 13065

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-07-25
- score: 1

<p><strong>The answer to that comes in 3-parts:</strong></p>

<ol>
<li><p>The best way right now is probably to ask the user with a form, preferably a spiffy Javascript driven one that appears in a context where it's useful for the end user. Ideally you'd ask the user for as little as possible, and then put together a precise location on your backend. F.x. you could present the user 2 inputs, "Country" and "Zip code or City", and then normalize data on your back end.</p></li>
<li><p>In the long term, the HTML5 Geolocation APIs are going to be the preferred way of handling this. There is very limited browser support for this already, fx Google Chrome 5 and <a href="http://www.mozilla.com/en-US/firefox/geolocation/" rel="nofollow">Firefox 3.6</a> support draft versions of the spec now.</p></li>
<li><p>IP location databases such as <a href="http://www.maxmind.com/" rel="nofollow">Maxmind</a>, now being suppleanted by IP location services. There are a couple of providers who will sell you an IP address to location map. These are imperfect, but even so, they probably get it right more than 95% of the time. The next wave of this will be online services that use multiple data points, such as wireless LANs in the neighborhood and GPS if available, to provide better precision. An example is Google <a href="http://code.google.com/apis/gears/api_geolocation.html" rel="nofollow">Geolocation API</a> (currently only available through Google Gears) or <a href="http://simplegeo.com/" rel="nofollow">SimpleGEO</a> (trying to be a geo-marketplace and not just location lookup).</p></li>
</ol>

<p>If you're just starting out, I would suggest just asking the user with an unobtrusive form. It is the simplest solution, it works, and it does not have any dependencies on browsers or 3rd party services.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
