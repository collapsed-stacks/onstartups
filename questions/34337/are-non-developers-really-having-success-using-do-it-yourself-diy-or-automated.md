## Are non-developers really having success using Do It Yourself (DIY) or Automated iPhone Development Tools?

- posted by: [Brett Miller](https://stackexchange.com/users/-1/15336-brett-miller) on 2012-01-02
- tagged: `software`, `iphone`, `webdev`, `android`
- score: 8

I own a small software development company that gets approached regularly by non-technical users who tried unsuccessfully to build their idea into an iPhone app using free (or cheap) automated development tools.

Sure someone that isn't a developer could try these tools, but I suppose they could learn to do maintenance and repairs on their own car as well.  Chances are it's not the best idea and they will run into limitations/problems quickly. 

Just curious of the opinion of some end users. 




## Answer 34343

- posted by: [Christian](https://stackexchange.com/users/-1/9952-christian) on 2012-01-02
- score: 1

I assume you mean: get a working iPhone app with the special cases you want to cover. It should work the way you can sell it.

I have not tried the iPhone tools. But I have tried several others tools in my software dev career. For example, Swing Builder for building Swing Applications. As an iPhone idiot I have worked with Phonegap, which lets you create a native app with javascript. And many more.

My conclusion is: there is a point in your project were you need to know something on programming or on the technical platform. After you are limiting yourself to the features of the tool, and in most cases you can cover 90% of your app with that, but the last 10% drive you crazy.

What if the tools in version 1.1 has a problem with iphone 3.1, but not with 3.2 or 3.0. Probably it is caused only on devices with enabled camera and disabled wifi. How can you deal with that? At most times your tool does not give you the cahnce to learn about the error. You need to dig the logfiles and learn on a deeper level.

That being said, look very very closely at your app. Is it something which does not need custom features? Then ok, probably you have a chance. But at the point you need a single feature which is not covered from the tool (or is buggy) then you are lost. You even can't reuse the code in most cases, because the code is sometimes not available or it is unhuman and not readable. 

That being said, these are technical days and if you want to produce applications you need to get into this technical world. I think these apps all promise to much and finally will end up in unhappy customers.

Probably other people have other experiences, I am eager to know.

Cheers
Christian



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
