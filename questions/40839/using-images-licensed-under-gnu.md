## Using images licensed under GNU?

- posted by: [Jack](https://stackexchange.com/users/-1/18940-jack) on 2012-07-26
- tagged: `gpl`
- score: 2

Can we use images/emoticons published under GPL license in our commercial online app?
If we do that, are we liable to publish app under GPL?

Regards,
Jack



## Answer 40847

- posted by: [Brendon](https://stackexchange.com/users/-1/18947-brendon) on 2012-07-26
- score: 1

It's a little confusing because the GPL (2.0) is open to different interpretations. It's also not an ideal license to apply to images. I think the safest answer would be **yes** -- you do have to publish your app under GPL. Look at clause 2 (b):

> b) You must cause any work that you distribute or publish, that in whole or in part contains or is derived from the Program or any part thereof, to be licensed as a whole at no charge to all third parties under the terms of this License.

In this case, "the Program" is the image you are using and "work" is your application. An online app, I believe, counts as "distribution". This condition is necessary to allow you to form "a work based on the Program", which is your app.

There's also this statement following:

> If identifiable sections of that work are not derived from the Program, and can be reasonably considered independent and separate works in themselves, then this License, and its terms, do not apply to those sections when you distribute them as separate works.

This is the only get out clause. I don't think it applies in your circumstances because you are distributing the app with the images. If you are distributing the app for others to use locally or companies to use internally you can distribute your app without the images, and then say "obtain and install the images yourself".

I think the best way around this is to ask the owner of the images to license under something else if possible. You might have to pay them. Or, just look for icons you can use commercially without restriction.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
