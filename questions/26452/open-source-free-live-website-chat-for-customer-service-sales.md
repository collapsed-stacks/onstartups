## Open-Source / Free Live Website Chat - for customer service / sales

- posted by: [Justin Levy](https://stackexchange.com/users/-1/11322-justin-levy) on 2011-06-18
- tagged: `sales`, `conversion`, `customer-service`, `chat`
- score: 1

I was wondering if anyone has come across a free / open-source website chat? I'm interested in something similar to oLark or Live Person, without the monthly fee's... 

Has anyone ever come across anything? Would Jabber.org work?

Also, I'd like to minimize integration time / development costs... (so I won't be creating one from the ground up)

Thanks in advance,
Justin


## Answer 26458

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-06-18
- score: 1

Justin,

Jabber is a protocol implementation of XMPP. This is an instant message protocol. So you can set up a Jabber server of course, but people will need Jabber clients and know your server. That might be to complicated for your users. Maybe you can find a website jabber client, but this might not support to many connections. GTalk by the way does use Jabber too.

You could try IRC instead. IRC is a chat protocol. There are many providers, most of them provide web clients too (probably in Java).

As starter you could try freenode: http://freenode.net/using_the_network.shtml
Or Quakenet: http://www.quakenet.org/

Then there is: http://www.pjirc.com/demo.php as client.

Then you can try a Java chat: http://www.javazoom.net/jzservlets/servlets.html
This is pretty OK; I have tried it myself. But also basic.

There are several Ajax / PHP Scripts out there too. from the PHP stuff I heard they are very resource hungry. Not only providers allow it. The Ajax stuff might need HTML5 to work fine.

So, if you have only a weak server or just want it for some nice chats at the evening you probably go with IRC. It is cheap (aka free in most cases) and with the webchats they provide easy to use. AND you can use it with your own Chat-clients, if you wish, like Miranda or Adium

Hope that helps you a bit.

Cheers
Christian



## Answer 26522

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-06-20
- score: 0

Most of the live chats use XMPP at the backend normally through a Jabber server, the front client is normally a javascript client, which communicates to the server via BOSH or web sockets.

While I don't know of any project that specifically set up as sales chat system, their are several open source jabber servers such as EJabberd and numerous BOSH clients out there, the paid services are obviously designed to give you much more control of the operators, multi user pickup etc but these can be found using added on extras.

Obviously going down this route you have to maintain the jabber server, so will need a suitable host, set up the additional plugins + setup the javascript client. Meaning a lot more work, though you can customise it far more.

The reason the paid services are there is even for tech companies it can be a lot of work, while for example the company I run is perfectly capable of managing such a stack and have at times pondered doing so the guys at Olark (who we use) make it so easy, and are so helpful and responsive it makes it easy to justify the expense. The live sales aspect paid for itself within hours of going live and continues to do so.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
