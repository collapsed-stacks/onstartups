## Website Graphics

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-10-28
- tagged: `website`
- score: 0

I'm building my marketing website to promote a SaaS product to be launched later this year. I'll have a small number of grahics on the website homepage. What's a better format to use (.jpeg, .png, .gif) for the graphics? 


## Answer 2624

- posted by: [Corey Maass](https://stackexchange.com/users/-1/325-corey-maass) on 2009-10-28
- score: 3

Gif's are best for vector-style images - blocks of color and text. They aren't good for photos or gradients. These days you'll usually use a png instead, unless you need transparency. 

Jpg's are best for photos. 

Png's can sometimes cover the best of both. Try doing one of the others, and then a png and use whatever is smallest and/or looks the best.


## Answer 2629

- posted by: [Duncan Wilcox](https://stackexchange.com/users/-1/869-duncan-wilcox) on 2009-10-28
- score: 1

The non-answer is to let a designer take care of it, it's a complex issue with many tradeoffs depending on the context.

The answer is that you should always use the file that comes out smallest for a given set of requirements:

- pixel-fidelity: JPEG is lossy so you won't use it for line art or text, etc
- color fidelity: 8-bit PNG and GIF can't render a continuous tone image, use 24-bit PNG or JPEG instead, depending on how acceptable compression artifacts are
- transparency: only GIF and PNG can do transparency, and only 24-bit PNG has a full 8-bit alpha channel (for partial transparency)
- animation: only GIF can do animation, with some limitations

So in general you'll use a JPEG with an acceptable compression for a picture, a PNG for a screenshot or small inline images or template graphics, and a GIF when you need animation.



## Answer 2622

- posted by: [blekkzor](https://stackexchange.com/users/-1/281-blekkzor) on 2009-10-28
- score: 0

GIF or PNG should be used for web graphics. If you're showing screenshots of your actual application, you might go with JPEG or PNG.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
