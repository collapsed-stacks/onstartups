## Doubt on open source

- posted by: [SS Hegde](https://stackexchange.com/users/-1/19234-ss-hegde) on 2012-08-15
- tagged: `open-source`
- score: -2

Ok. I have started to port an open source project from Linux to Windows.
My doubt is, can i sell it for money after porting to windows? is it ethical?


## Answer 41368

- posted by: [kizzx2](https://stackexchange.com/users/-1/4628-kizzx2) on 2012-08-15
- score: 6

IANAL. Most open source projects use one of the "standard" licenses:

- BSD/MIT (liberal, do whatever you want): you can use it in a commercial, closed source product.
- GNU/GPL ("copyleft" licenses), you probably can't -- these license state that your port ("derived work") must also be open source as well.
- CC (Creative Commons): has some variants that permit commercial use and some variants that don't. Read the subclauses.

In many open source projects there is a COPYING/LICENSE file which includes the license. Find out what license your project has. These keywords should be enough to get you started.

In many of these cases the license may require you to attribute the original author.

If the project does not explicitly state the license type, the author (copyright holder) has not granted you any right to use it in derived work. You must seek his explicit consent before using it in a commercial project. There is a slight possibility that your open source project uses a "custom" license that is not included above, in which case you need to read it in details.

Edit:

For completeness, there are certainly more types of "open source" licenses out there, like MPL/Apache/X11 just to name a few (heck, even Microsoft has MS-PL). The important thing is to read the limitations/terms of use part (most fall into the liberal/copyleft classification paradigm). Many of these open source licenses are written in a way to be easy to understand so don't be afraid to read them. Of course since they are standard you can probably Google around and find some "layman definition" of them for non-rigorous purposes.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
