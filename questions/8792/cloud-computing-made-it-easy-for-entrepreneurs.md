## Cloud computing made it easy for Entrepreneurs

- posted by: [Siddharth](https://stackexchange.com/users/-1/969-siddharth) on 2010-03-03
- tagged: `entrepreneurs`
- score: 0

Entrepreneurs with brilliant ideas for a software startup (but not enough money at the beginning) would have faced the issue in the beginning: Where should i start building the alpha version of my software, how should i make it available for the people to review, how should i give demos to the investors? The usual practice is the software is running in my laptop and i need to carry it for the demo but what if your partner is in the other side of the globe and he wants to show a demo? Another possibility can be invest some money, buy a server, buy your domain and run your software over there and access via internet. Another possibility can be share it with a hosting infrastructure company but the rick can be how to protect your idea/IP! All these are not very efficient or requires money which you may not want to spend in the initial days of your Entrepreneurship.
Off late cloud computing is becoming very very popular. The best part is some brilliant platforms are just available free! You can develop your application and deploy it for free over internet! Thats amazing is n't it? Some great cloud computing frameworks you can try:

 - Cordys process factory ([http://www.theprocessfactory.com][1])
 - Google app engine ([http://code.google.com/appengine/docs][2]/)
Once you are comfortable, got an investor, you can decide how to go forward with your beta product. Either you can continue with these frameworks or can have your on premise deployment

Recently i was associated with a startup as the architect and we developed our alpha version on one of these frameworks. We did not have to spend a single $. My partners were accross the world and they could give the demo from the internet! that was quite exiting.

I strongly feel the evolution of these cloud frameworks have simplified the life of Entrepreneurs in the initial days of their venture to a great extent!

Feel free to share your thoughts on this. Also feel free to share your experience on these cloud frameworks.

regards,
Siddharth 





  [1]: http://www.theprocessfactory.com/
  [2]: http://code.google.com/appengine/docs/


## Answer 8808

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-03-03
- score: 1

<p>I don't see cloud solutions offering a revolutionary change - its more an evolutionary step in virtualization (don't get me wrong - i'm a big fan of cloud computing).</p>

<p>The bigger change came when companies didn't have to allocate capital to run their own t1's &amp; fill a co-lo rack with their own equipment - and - hardware performance per rackspace increased to the level that a densely packed rack could be shared (at a profit).  </p>

<p>Shared / virtual server providers offering cost effective solutions paired with ability to add resources at a button click really was the big change - and is still applicable today (rackspace, anyone?).  <a href="http://en.wikipedia.org/wiki/Moore%27s_law" rel="nofollow">Moore's law</a> moves on..</p>

<p><strong>[EDIT - adding more]</strong></p>

<p>When talking about "cloud anything" I'm reminded about the <a href="http://en.wikipedia.org/wiki/Blind_men_and_an_elephant" rel="nofollow">three blind men &amp; the elephant story</a>.</p>

<p>Three different types of clouds are being discussed here.</p>

<ul>
<li><strong>Infrastructure as a Service</strong> - virtualized hardware, storage services, compute services </li>
<li><strong>Stack as a Service</strong> - Virtual Machine images (stripped-down Linux all the way to infrastructure support software - see <a href="http://elasticserver.com/" rel="nofollow">elasticserver.com</a>)</li>
<li><strong>Platform as a Service</strong> - AppEngine, Heroku, or potentially Cordys. </li>
</ul>

<p>I'll leave out <strong>Software as a Service</strong> - (SalesForce.com is the prime example) Further elaboration on the definitions can be found on <a href="http://en.wikipedia.org/wiki/Cloud_computing#Layers" rel="nofollow">Wikipedia</a>.</p>

<p>Now - My statement above was referring to IaaS, where most providers offer a virtual instance that mimics a virtual server. Benefits are that on demand you can add servers - but remember that such instances are ephemeral (they go away when terminated).  Something needs to be running somewhere to service requests.  </p>

<p>A <strong>Stack as a Service</strong> provider can help when you need to quickly deploy those additional virtual instances, but to scale this way you need to have developed a solution that <em>uses multiple servers</em> and knows when to add / remove them. IaaS providers can provide more powerful single instances, but you need to stop the current one, add resources &amp; and start. A few minutes downtime.  </p>

<p>So - essentially you have a virtual server in a cloud environment - and you are responsible for scaling.  That's fine - but understand that is what the product is, and not some elastic, auto adjusting resource that costs pennies to run.  </p>

<p>OF late, IaaS providers are starting to offer "cloud sites" (http://rackspacecloud.com is a good example) where specific types of applications can run on a cluster of servers.  Can't support direct SSL connections, and you need to do some interesting things to support credit card transactions and still be PCI compliant, but everthing does scale based on load. Such a service starts at $149 / month (50 gb disk, 500gb bandwidth and 10000 compute cycles) and has overage charges (.50 per gb bandwidth / .01 per compute cycle).  </p>

<p><strong>Platform as a Service</strong> providers go one step further that this and allow you to deploy at an routine level. Those in the know will likely run circles around me talking about the benefits of deploying in heroku vs a typical IaaS, so I'll let them weigh in on the benefits to startups.  My take would be that this is an excellent way to have a stable deployment platform to grow from.</p>



## Answer 8796

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-03-03
- score: 0

Your post has not made it more clear what cloud computing is. Can you be more specific about how it is useful to entrepreneurs?


## Answer 8805

- posted by: [Mike](https://stackexchange.com/users/-1/2696-mike) on 2010-03-03
- score: 0

This is my view... might not be 100% technically correct, but here goes! :)

You can look at cloud computing as having a complete IT data center without having to buy equipment and setting it up. 

What this means is that your server is available on the internet, and you can access it anywhere. You don't need to buy the server hardware, install the operating system and everything else you might need to run it. You select an "image" of what you want to have running there (for example Windows Server + SQL Server + ...) and then install the apps you need there. 

If you're creating a web application, you can host it there and people access it through the internet, transparently.

Hope this helps 


## Answer 8817

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2010-03-03
- score: 0

A startup could get by with a virtual host (you share a single server with other users). The problem is, when do you upgrade as your site grows? To grow the site you may be forced to buy/lease more servers. This is a big incremental jump in cost and development.

The cloud really adds benefit by charging you on an ongoing usage basis (cash-flow). If there are usage spikes during the day, you're covered. Late at night, little to no usage, not a problem since you don't have to pay for it. Hosted solutions or buying your own servers doesn't really let you grow gradually (Your second server just doubled your expenses). If your site become so huge, it may be cheaper to buy your own servers instead of renting from the cloud.

The best analogy is getting electrical service to your home. You can pay a utility company (Electrical Cloud) for your power usage or you can make an upfront investment in a generator/solar panel/windmill/etc. (virtual host, co-location, lease, create your own data center.). 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
