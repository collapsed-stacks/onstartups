## Commerical Open Source and Community Open Source

- posted by: [JohanSJA](https://stackexchange.com/users/-1/12113-johansja) on 2011-07-21
- tagged: `business`, `open-source`, `license`, `community`
- score: 1

I am thinking on working on an ERP system that I can sell or support on it. Currently, I have [OpenERP][1] and [Tryton][2] in my mind. Based on the comparison done on Wikipedia and other website, I was noticed by these two terms as mentioned in the title. I like the idea of Commercial Open Source as I can be more confident that someone is always working on that product. But my concern would be that will a Commercial Open Source be a proprietary software suddenly? How can these two models affects my business in future? 


  [1]: http://www.openerp.com/
  [2]: http://www.tryton.org/en/


## Answer 27782

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-07-21
- score: 1

I'm not sure how relevant the Commercial/Community distinction is here.  The most important question is the license that the open source project is distributed under, as that determines what you can do with it.

OpenERP is distributed under the Affero license and Tryton is distributed under the GPL.  Both of these licenses require you to make your changes available under certain conditions.  Are you ok with sharing the changes you make to this code?  If not, then make sure you understand the details of the licenses.

Even if the open-source code is later made proprietary you still have the rights to use the code that was released under the Affero and GPL licenses as the licenses are irrevocable.  You just won't have the rights to later versions.


## Answer 27803

- posted by: [danmaz74](https://stackexchange.com/users/-1/12083-danmaz74) on 2011-07-21
- score: 0

Many commercial open source projects start by giving a lot for free, to get traction, but later focus more and more on not-free versions to monetize their work. This doesn't mean that they'll take away from the free open source license what they already contributed - that would be impossible if they adopt any of the main open source licenses - but they start publishing new features only in the paid version so that more and more people will convert to it, and the free version starts to languish. At some point it can be abandoned altogether, but you can still use the last published free version.

In community-driven projects this can't happen, but it is always possible that the project loses steam and updates stop coming in. The web is full of abandoned open source projects; their fate is pretty much the same of an abandoned free version of a commercial open source project.

So in the end the risks are pretty similar: You could end up with a product that doesn't get any update, which in many cases isn't such a big problem. For ERP I think it is, though, especially if you want to use it also for fiscal purposes. At least with commercial open source you'll know that, if the developer company doesn't go bankrupt, you'll be able to get the paid version, if you really need it and can afford it at that time.

One last thing: You can also take a look at OpenBravo. Some of my coworkers work with it and they're happy enough with it.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
