## Hosting images outside main site?

- posted by: [martin's](https://stackexchange.com/users/-1/16979-martin-s) on 2012-10-29
- tagged: `website`, `seo`, `hosting`, `forum`
- score: 1

I noticed that sites like StackOverflow host user-submitted images outside their site, (in the SO case, at imgur).  I've also seen forums do the same thing.

Are there advantages to taking this approach?

On first inspection it would seem that one would be in danger of having content compromised in some way by the image hosting provider.

I understand that one advantage might be that some of the bandwidth required to deliver a page would now be split between at least two servers.  Is this a bandwidth play?  Or is there another issue (legal, security, liability, etc.).

SEO consequences?



## Answer 43923

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-10-29
- score: 2

Usually sites like SO use so called CDN:
http://en.wikipedia.org/wiki/Content_Delivery_Network

**Potential usecases:**

Imagine you have a single, physical computer serving as a webhost in the UK. When a visitor from the UK comes, he gets connected pretty soon. Images transfer from London to Bristol maybe and its all pretty nice and decent.

But what happens if a visitor from southern australia comes to your site. The image, which is sometimes having a huge size needs to go to down under. Not only that connection making is taking a good while. When there is much data to transfer it is most likely that some packages of data are lost. Lucky that the protocols can check if something gets lost and request the chunks of bytes again. But well, reasking takes another good while.

Another scenario. Imagine you have two physical computers in London. One is only hosting the app, the other one hosts the images. You have chosen that architecture because the images take a huge size and maybe for some other reasons. Anyway, your image server is going down - your visitors sees your site but without images.

Another scenario: you wrote a blog post with many images. It becomes famous and suddenly your host goes down because of the high load of customers.

**That are only three cases in which CDN does help.**

A CDN does **replicates your data** to various hosts on the world. For example, one in Japan, Australia, US and so on. They give you a single url for that and well for you its all the same as usual. But the CDN takes care that an australian visitor gets the image from the australian server and the UK people gets them from the UK server. This is pretty much faster. We speak of optimal caching and maybe even DNS optimized stuff.

If one server, for example in Australia goes down, no problem. The other server will respond. It's always better to a bit more delay than a failure.

In the last case, a CDN takes care that there is **always enough bandwidth and cpu resources** to process all the requests, no matter how many.

Some companies create an own CDN, using Amazon AWS S3. Others use ready to use solutions, like for example Amazon CloudFront:

http://aws.amazon.com/de/cloudfront/

There are many others, not just Amazon. Make sure you check several offers if you want that.

**Compromising** Everything can be compromised. The likeliness that your own little webhost is compromised is pretty much higher than for example Amazon CloudFront. A CDN is like your hair-dresser: you need to trust. That said, many people use CDN, i have not heard of compromised images so far (but well, world is big and my inbox is small).

**Legal** Please be aware that if you use CDN and host images in for example Germany, german law applies. This is surely the case for every other place. Make sure you know what you host. I assume you are doing legal stuff, so not so much to matter here. Downloads are usually not stored on a CDN btw. You want legal control about downloads.

**SEO** I don't think there are any. Nobody knows, but it simply doesn't make sense. Google itself is a CDN provider. That said, better car on your alt-Attributes then on CDN links. In addition, if an image loads faster Google rewards it, as people say. Guess Bing etc does the same.

**Potential Drawback** I recently that about CDN in terms of cost. If your shop hosts images on CDN and a competitor wants to do some harm to you, he could download a huge image from your CDN a million times. Usually you are charged by traffic, so this might be an issue. That said, there are many CDN providers who give you some kind of fraud insurance. They would block such kind of requests if they think this is an attack against your business/account.



If one does not need/use CDN and stores images on an external server it might be an architectural solution (streaming images is not so resource-hungry as a java app and thus cheaper servers can be used). Or he simply thinks it organizes better. But there is no extraordinary reason to do so.


## Answer 43945

- posted by: [B Seven](https://stackexchange.com/users/-1/14522-b-seven) on 2012-10-30
- score: 0

There are 2 main advantage of using a CDN to host images:

 1. It's fast. A service like Amazon S3 has tens of thousands of servers.
 2. It reduces the amount of work your server has to do. It makes your whole service faster.

SEO should not be affected, and security is not really an issue either. However, there are certain best practices that should be used when connecting to the CDN. For example, Amazon secret keys should not be stored within the code.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
