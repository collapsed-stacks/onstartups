## Tips on open-source project - should it be free, licensed, etc?

- posted by: [Jason](https://stackexchange.com/users/-1/6650-jason) on 2011-01-17
- tagged: `software`, `open-source`, `free`
- score: 4

I have been working on this project [seen here](http://www.jasonleodurbin.com/blog). It is a Photography CMS (like WordPress). I cannot visualize a business model to provide funds to support the project. I want to release it as a free, open-source project. But I don't want to continuously make updates on it in my free time (it is much larger than I originally thought when I took it on) without generating revenue.

1. Is there a better way of going about it generate revenue?
2. Should I just focus on developing it in hopes someone will buy the project off later?

I considered having a free license and a paid license (full features). Though, I cannot visualize this being possible with the nature of the code (php, downloadable, self-hosted).

I would prefer it to be open-source so I don't have to deal with the lawyer side of it. But after reading other questions about open-source projects, this seems like a poor choice.

Any suggestions? 


## Answer 26918

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2011-06-29
- score: 1

Open Source software is a business model, which can work. But there is no guarantee on that.

You could build up your business around your CMS, like:

  - offering hosted CMS solutions
  - offering support with installations
  - provide customization service
  - provide import/export service
  - write a book on it and sell the pdf as docs
  - provide closed source modules (advanced feature xy for only 10$ or so)

But be careful - if choose the last option, you might need to take care on the licensing.

There are two common license types around: copyleft and non-copyleft.

Copyleft is for example GPL. The approach is, if somebody writes something on top of your software, he needs to publish the change as open source too.

THe other on is for example Apache Licsense (AL 2.0). You write the code, and everybody else can do whatever he wants with it. From own experience, you'll get tons of contributions back, even when people are not forced. Benefit: it is attracting business users more, because they can build a new product upon your softwares back.

Both software licenses require to leave the header intact (your name is there, for ever).

Both software licenses exclude any guarantees - use on own risk.

Personally I love open source and I am an active open source coder myself (apache license esp). I have seen business models like that working very well. 

You should consider one thing finally: you said, it is PHP. If you deliver your PHP script to a customer, he already has insight into the code. Even when it is not free, he sees the source code and could do nasty things with it. For example, copy it to another host without buying a new license. You could obfuscate, but, well customizations on customer side are not so good then. 

If you ask me, do something from the list above. Host it on github, googlecode or try to get it into the apache.org foundation and you will probably get a lots of contributions which makes your software wellknown. Hopefully people buy some of your services. If they don't do you don't want to continue you have at least some great code to show your new employer.

Cheers
Christian


## Answer 19494

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-01-27
- score: 0

<p>That's the open source dilemma in a nutshell!</p>

<p>If you go open source, there's a wide choice of existing licenses to choose from, each of which will avoid legal fees for a custom license, and each of which will have different implications in terms of the ownership of the code and what other people can and can't do.  </p>

<p>There's a useful maintained list <a href="http://www.opensource.org/licenses/category" rel="nofollow">here</a>.</p>

<p>But you've already been reading up on how difficult it is to monetize your hard work when you open source - and you'll have noticed how many open source projects wither on the vine.</p>

<p>There's no reason why you shouldn't offer this as a paid product. The fact that you're providing code is neither here nor there. </p>

<p>And there's no reason why you shouldn't offer free and paid licenses. One common approach is to insist that free licensees retain a prominent credit and link back to your site. It's easy, of course, for people to abuse this. They will be aware they're doing so in breach of their license - which is enough to restrain many people - and you can potentially pursue sites showing such misuse. </p>

<p>If you feel there's no real revenue potential that you care about, go ahead and open source. If you feel there may be, start out that way and open source it if the opportunity doesn't develop as fast as the burden.</p>



## Answer 19600

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-30
- score: 0

<p>Many open source sites started free and then started charging for use. Take <a href="http://www.last.fm" rel="nofollow">last.fm</a> for example, it was a free service till they started charging people (which is a little mean, if you ask me, since they got people to edit entire playlists etc and now if you want to listen to them you need to pay) for it. I think that's the main idea - get people hooked on your service (which seems really cool, btw!) and then you can starts charging later. OR simply get ads going on site and the larger it get the more money you will earn, just like facebook. In any case, I really like your project and as an avid traveler and photographer (well, amateur, but still!), I would love to watch it grow. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
