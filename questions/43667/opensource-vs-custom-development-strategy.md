## Opensource vs custom development strategy

- posted by: [gyrostu](https://stackexchange.com/users/-1/21177-gyrostu) on 2012-10-16
- tagged: `copyright`, `open-source`
- score: 0

The possible advantages of using something like Drupal is a dev time-saver. But if we were to develop a minimum viable product / proof of concept / prototype using Drupal, other developers could own copyright to their modules. This means that the product eventually would have to be rewritten to clear copyright issues. 

If we take the time to develop the proto with Drupal, add the rewrite time and measure it against just writing a custom application, could we come out better just writing a custom app using something like CodeIgnitor, Zend or Rails?

Also, by building a custom app we know the inner-workings and don't have to reverse-engineer anything nor sift through mountains of sometimes fragmented documentation.

Your candid thoughts are greatly appreciated.


## Answer 43702

- posted by: [hoosteeno](https://stackexchange.com/users/-1/21204-hoosteeno) on 2012-10-18
- score: 3

The most general answer to the "off the shelf vs. custom" question is pretty much what @robin-vessey says. Succinctly, is your product the audience you build, or is your product the technology you build? If the first, off the shelf works great (see countless valuable online publications for evidence); if the second, it probably won't long-term.

> ...if we were to develop a minimum viable product / proof of concept /
> prototype using Drupal, other developers could own copyright to their
> modules.

I think copyright is a red herring for this particular question. It boils down to this regardless of your technology: If someone besides you wrote something that you plan to sell, you must secure a right to sell it. For many libraries (I believe this is true in the Drupal community, too) that right is given freely, preemptively through license.

> If we take the time to develop the proto with Drupal, add the rewrite
> time and measure it against just writing a custom application, could
> we come out better just writing a custom app using something like
> CodeIgnitor, Zend or Rails?

Let's assume that no other variables are in play (which is a false assumption: _lots_ of other variables are in play, such as the skillset of your team, the location in the stack of your IP, the technology you eventually migrate to, etc.): You will probably spend more time building it in Drupal and then rebuilding it elsewhere than you would if you just started elsewhere. 

That being said, there is a strong case to be made for prototyping using the fastest possible prototyping solution, because doing so can give you rapid insight into things you can only learn from your market.

On that note, if you haven't already, consider prototyping in something even more lightweight than Drupal. Like static HTML. Or Balsamiq. Or paper. If you show the right people what you're thinking, you'll get more insight into this question and many others.

> Also, by building a custom app we know the inner-workings and don't
> have to reverse-engineer anything nor sift through mountains of
> sometimes fragmented documentation.

Well, maybe. A custom application built on one of the frameworks you mention may require engineers to sift through mountains of something, that's for sure. I think when you're building innovative products on the web, you're going to be sifting. That's why it's important to choose tools that your engineers don't mind fighting sometimes.

A couple other quick notes that may inform this discussion:

* It can be tough to find engineers who are productive and happy jumping from a "bought" to a "built" solution. Bridging the difference between a CMS and a framework can create some real frustrating inefficiencies that many developers choose not to fight. 
* While I can't recommend this from firsthand experience, since CodeIgniter is the framework underneath ExpressionEngine, and ExpressionEngine is arguably equivalent to Drupal in capabilities, you might be able to transition from bought to built that way.
* Anything you can do to avoid throwing something away wholesale may help you maximize your development dollar. If the product doesn't belong in Drupal at the end, using Drupal at the beginning means throwing away Drupal halfway through. But it sounds like your product will have some HTML, so using static HTML at the beginning might just mean coding your static HTML in your framework's views halfway through. One tool that can make this downright fun is a static site generator like Middlemanapp, especially if you're headed toward Rails.









## Answer 43700

- posted by: [Jeremy Tunnell](https://stackexchange.com/users/-1/21202-jeremy-tunnell) on 2012-10-17
- score: 2

I've gone through this thought process before, and I've spoken to many other founders who were tackling this question.

My answer would be a solid no, except in really unique circumstances.

Anecdotally, I remember speaking to a founder of a recently failed startup who faulted this decision as one that contributed to the failure. Essentially, using Drupal helped at the very beginning, but as time went on it became more difficult to work around the limitations of the system.

Why? Because Drupal is essentially a really flexible content management system. It's not a platform or framework on which to build a product.  Likely, it would enable you to get your MVP out the door very quickly, but you would soon be forced to work around its limitations. If you're lucky, you'll be able to re-factor as you go, but there will come a point at which you will need to replace the core of the system.

A much better idea is to use a programming framework like CakePHP or Django. These will allow you to use the components you will need (authentication, data access, security, parsing, etc.) without getting in your way.

Just a hit on a couple of other points:

I don't think you're going to have any copyright issues with any of these, including Drupal.

I mentioned earlier that I would only recommend Drupal in unique circumstances. An example of such a circumstance would be if your startup is essentially a business innovation instead of a technical innovation (and even then, you may underestimate the technical aspects of the former). For example, I think groupon used WordPress for a very long time because all they needed to do was display coupons in a blog format and allow people to purchase them. 


## Answer 43684

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2012-10-17
- score: 1

It depends on what your intended business model and target exit is.

If your business relies on having specific intellectual property, using your specific code as a barrier to others following you, then you want to own the components you build.

If your business model, income and reason for buyout are because you have a specific set of clients, a great brand name then the technology may not matter as much and you can go open source because it doesn't really change the value of what your business is.

That said the specific licences for open source systems have different rules around additions to the base technologies. If you pick the right one you can utilise what it has to offer and also keep your specific components private.

Really, when you think about it others can do a similar thing using the open source and overtake you. Think through would you try to get their code to make yours or would you stick with your code? 
You would probably stick with yours because generally it allows you to provide a point of difference, and they think the same way.

So I guess my general message is, don't worry about it to much unless its a critical factor to the long term value of your business. 

Make sure the open source licence enables you do keep hold of the key bits you want to and get to you MVP as fast as you can because your more than likely going to change a lot of it anyway the day after you release and start getting feedback.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
