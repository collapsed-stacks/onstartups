## Server costs for video startup

- posted by: [Zipper](https://stackexchange.com/users/-1/18034-zipper) on 2012-05-20
- tagged: `video`, `costs`, `server`
- score: 1

I've been going over some of the posts here regarding server costs but couldn't really find any information specific to my needs. I'm planning on creating a mobile app that deals with users uploading videos. I realize this will take more server resources than a typical application that deals with just textual content. I would like to know if anyone has an idea of what kinda of server I'll need to start with and how much should I expect to spend. I do not have any external funding, so it's all coming out of my pocket. So any useful information to keep costs low would be greatly appreciated.

Thanks!


## Answer 39252

- posted by: [DigitalSea](https://stackexchange.com/users/-1/7816-digitalsea) on 2012-05-21
- score: 3

<p>The costs depend on your traffic and code-base, based on my experience working with large-scale video websites you need quite beefy servers just to process the video and convert it into a more friendly format, then you need the bandwidth to play the video back to the end-user. I would advise against starting an online video site unless you have large amounts of cash to spend. You could use Amazon EC2 for both your converting and playback, you get charged for the bandwidth and processing power you use, at the start you'll probably want a server instance for processing video, a server instance for serving your pages running a reverse proxy like Nginx and a server for your database.</p>

<p>There is a lot to consider when starting up a video site, like I said I would go for Vimeo or Youtube and use their API's, if they don't meet your needs then you're going to need a bit of cash. At the beginning you'll probably be up for a few hundred per month in server costs, as your traffic grows so will your costs.</p>

<p><a href="http://aws.amazon.com/ec2/" rel="nofollow">Amazon EC2</a> is your best bet for something like this and the number one first choice for most internet startups that want to be able to scale.</p>



## Answer 39253

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2012-05-21
- score: 1

Mor eprecise to Dwayne - you need a lot of CPU and a lot p f processing power.

Unless you fail, amazon is stupid - clouds are extremely cost negative when you run a lot for a long time. FOr exmample, I am odffereed a 1 rack unit hosting for about 100 usad including 10.000 gb traffic in a large chicago data center. Beat that with Amazon ;)

What I would go with is:
* A SuperMicro 4 rack unit case that holds 72 discs possibly on a dual socket motherboard and a GOOD Raid card. The case already will put you back around 2500 USD - all in all without discs you talk of likely 5000 USD.
* A SUperMicro Twin2 case. That is a u2 rack with 4 "slots" that take dual socket mobos each, allows yout to put 8 CPU sockets into 2U.

If you scale that up, I would skip the Twin and go with a Del M1000e blade server case - there are new super small dual socket blades coming out where you fit 32 of them into one center (64 sockets total) and you can get a blade center for a decent price refurbisehd (the center itself does very litle that can break).

Finding hosting is another thing - you need a LOT of power, most data centers can not handle that outside of multiople tacks (kudos for CME Group new Aurora that has 12.8kw per rack distribution IIRC - but then, this is not normal hosting). I Know of a couple of US ddata centers where modern computers DO NOT RUN (ralk of 60 watt powre allowanc eper rack unit - a joke, most decent CPU have more power requirements).

There is always the tera box concept. someone was putting a LOT of vertically mounted discs into a special rack case.

A lot depends on your growth patterns and estiamted space. THis is the wrong place to ask - serverfault.com has mre info, but your local IT guy should know. THis is why senior popeople are senios.

But beware of clouds, their cost side is RIICULOUS expnsive for long term use. I am a big fan of private clouds (i.e. you OWN the platform) running myself on the 8th (next server delivered) 144gb with 6 sockets ;) The cost side I have is a nice joke compared what it would take Amazon or AZure every month to pay for that.


## Answer 39258

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2012-05-21
- score: 1

Your highest cost by far is going to be bandwidth.
Look for an inexepnsive colo.

I can recommend Calpop (los angeles)
Hurriance electric (by far the cheapest, in Bay Area)

Cloud offerings will cost you TOOO MUCH..
If you are looking to have a cloud, build your own using xen or hyper-v or vmware




## Answer 39259

- posted by: [Tom Squires](https://stackexchange.com/users/-1/11392-tom-squires) on 2012-05-21
- score: 0

The cost will really depend on what you want to do, converting will cost more also different formats will be larger/smaller and will cost a different amount to store. 

I suggest you run through a basic cost estimate yourself. Run through a typical use case and then estimate what you need at each stage. You then can multiply that by your estimated user base. You can then use Amazon as an estimate of what you need to fulfil those needs.


## Answer 39279

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2012-05-22
- score: 0

<p>Ah - cloud vs dedicated.  The debate continues. ;)</p>

<p>Agree this is more of a serverfault question.  But, since I don't really know what the primary business model / MVP is, I can't quite determine whether the encoding / transcoding is best outsourced or not. Or what bandwidth is required. Or what encoder makes sense.</p>

<p>"Users uploading video" isn't extremely helpful.  Are we talking about small 10 second clips or 2/5/10/15 minute clips?  Are you doing any special encoding at the capture device? Once you have the video, are you multicasting it?  public or private sharing?</p>

<p>All these things allow someone to figure out what architecture makes sense - otherwise we all are <a href="http://en.wikipedia.org/wiki/Blind_men_and_an_elephant" rel="nofollow">describing the elephant</a> from our own limited vantage point.</p>



## Answer 39339

- posted by: [Jez](https://stackexchange.com/users/-1/18079-jez) on 2012-05-24
- score: 0

To reduce some costs with server storage and data stream, have you considered any compression module in your mobile app? This will significantly reduce the file size before upload and also allow for a quicker upload time. 

The issue now with the later model tablets and smartphones, is the size of video they create. You may want to consider some form of compression in your app to alleviate some of the costs at server side and data costs incurred by the user (if not using wifi) + nicer user experience with decreased upload time.


## Answer 39508

- posted by: [John Clark](https://stackexchange.com/users/-1/18163-john-clark) on 2012-05-30
- score: 0

Depending on your expected volumes, you might be just as well to consider a dedicated hosting solution such as Viddler.com.  Whilst this would become more expensive as you grow, it might well be a short-to-medium-term option that would enable you to prove your concept to determine if it will fly or not.

On the other hand, if you are charging your customers to use your service, you might be able to determine an outline cost-per-xxx for a typical video.  I do this on my site, and generally factor in the cost of (third-party) video storage and streaming into the price.  Works well enough for me.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
