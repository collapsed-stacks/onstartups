## E-Commerce Website for Retail AND wholesale

- posted by: [Erin Danahy](https://stackexchange.com/users/-1/13333-erin-danahy) on 2011-09-14
- tagged: `website`, `ecommerce`
- score: 1

I work for a clothing designer company (Kit + Lili) that has been in business for 5 years.  We currently sell our product wholesale using a company called Groupe BDM and retail through Shopify.  It is an incredibly inefficient system, and I'd like to find a platform for a website that allows both retail sales/pricing and wholesale login/pricing.

Things to consider:

-I do not having programming experience - in fact the ability to upload seasonal clothing, pricing, and sku's with minimal to no coding is essential.  Shopify provides the templates for this.  They just don't yet have an app in place to allow wholesale login/pricing.

-For the wholesale part of the site, we need the ability to place orders and check out, but not require payment through a shopping cart app. At the same time, we need the shopping cart for retail. With the clothing industry, orders are usually made 6 months prior to shipping and receiving payment.


Does such a platform exist or do I need to find a web designer who can create a site to our specifications?

Also, let me know if this question might be better posted in a different forum.  Thanks.


## Answer 30095

- posted by: [Angel Brighteyes](https://stackexchange.com/users/-1/13329-angel-brighteyes) on 2011-09-14
- score: 2

Even with a pre-fab shopping cart/content management system (such as a combination of drupal and ubercart) you are going to want to find a website designer/programmer that can customize the site to your specific needs requirements.  Using a system like joomla or zen cart (other e-commerce/cms pre-builts) is going to be much more cost effective, even with a web expert helping you along.

From experience, I have to say that trying to have your own CMS and E-Commerce solution built from the ground up is going to be very time consuming, costly (depending on who you hire and what they already have available in the way of solutions), and just all around is not what you want to do.

Unless you have the capital to throw into it.  Just make sure that regardless of the rout you take, that the web expert does not pidgin hole you with technology that will have you coming back to them only for future updates, releases, or configurations.  Talk to multiple web experts, preferably who specialize in e-commerce solutions.  Get their opinions, do some research on different e-commerce shopping carts that are available (I listed a couple, WARNING: I have heard nothing but bad reviews for zen cart), and make yourself aware of what is out there.  You don't' have to make it work, just understand how it works or how it applies to your clients.

As a web developer myself, I decided to use Drupal and Ubercart, because of how much customization both allowed, plus the availability for support and help within their own community.  There are many developers who can create custom drupal solutions utilizing the current foundation drupal already has as a hard hitting content management system.  I love drupal that much, which is why I mention it.

All in all, knowledge is power with this one.  Get all your options and lay them out on the table and make your decision based on your needs requirements.


## Answer 30098

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-09-14
- score: 1

<p>I have done a bit of work with <a href="http://www.magentocommerce.com/" rel="nofollow">Magento Commerce</a> they have a 100% free / open source version.  Magento will allow you to run multiple stores / store pricing within a single installation so you should be able to achieve what you are looking to do with your different pricing for wholesalers. Allowing them to order / checkout without paying may need some customization.  Or on that site you could just set it up for 'check' or do something kind of tricky / hacky to get it to work.  </p>

<p>Search around for some good Magento experts and pose the question to them.</p>

<p>Another non-'free' option is <a href="http://www.aspdotnetstorefront.com/default.aspx?" rel="nofollow">ASPDNSF</a> which I am 99% sure has tiered wholesaler pricing.  I've done a couple projects in it, prefer Magento.</p>



## Answer 35361

- posted by: [nahmed](https://stackexchange.com/users/-1/16017-nahmed) on 2012-01-27
- score: 1

Have just come across this question and since I am in the process of designing a similar solution for my own website, I thought I'd share an idea of how we have done trade and retail on the same site.

Essentially, we have created two types of user accounts. When a trade customer logs into the site, they see the trade price depending on the trade discounts we have allocated to them and when a retail customer logs into the site, they see the retail price. We go through the trade customer's account creation manually after credit checks etc so we can control the discount offered to the trade customers. This way we do not have two sites or shopping carts and can manage through one website that is already serving our retail customers. Our site is in Drupal/Ubercart since when we started we did not find any off-the shelf solution.
When it comes to the checkout and payment process, we just generate a proforma order that they pay off-line in case of a credit account. This is the point we are hoping to industrialise in our next iteration but given we only have about 25 trade accounts we can live with manually processing the payments.

Hope this helps.

Best of Luck!




## Answer 35366

- posted by: [Abe S.](https://stackexchange.com/users/-1/15559-abe-s) on 2012-01-27
- score: 0

I have to echo the calls above to go with a slightly more robust e-commerce solution. Turn-key platforms like Volusion are nice in theory, but as soon as you begin talking about using the same site for retail and wholesale, two very different customer groups with different needs, different messaging, etc., you need more flexibility and scalability in the long run than a 100% web based, managed cart can offer. 

The web is a technical playground, based on computer code of one language or another; to manage it correctly, as Angel Brighteyes notes, you need to have a developer on hand for the tasks you simply can't accomplish on your own. 

I recommend looking at Prestashop (http://www.prestashop.com) who is quickly creeping up on Magento's market share, but is much simpler and lightweight to use and deploy, while offering virtually the same features (Magento is generally viewed as powerful, but unnecessarily large and clunky). 

With Prestashop or most other open source PHP carts on the market today, you will be able to easily create multiple customer groups (ie. Retail and Wholesale) and assign different prices to each, including discounts for quantity purchases (often important for Wholesale) and even the ability to hide prices on the front end until a user is logged in, if that is an important feature. 

Bottom line is that on the web, everything is possible, so don't limit yourself by using a niche solution geared towards tiny businesses with purely non-technical staff where you are likely to spend far more time and energy in the long run creating the perfectly on-brand experience you need. 


## Answer 49227

- posted by: [Caroline](https://stackexchange.com/users/-1/26363-caroline) on 2013-05-23
- score: 0

I can say from experience, don't use nopCommerce and their tiered pricing.... it is cumbersome and filled with problems that required thousands of dollars of special programming to get a simple wholesale login and checkout.  The rest is fine, but login and checkout are a bear.  


## Answer 30093

- posted by: [Mike](https://stackexchange.com/users/-1/11945-mike) on 2011-09-14
- score: -1

Wow, that sounds just like something I was going to do... A did a bunch of up front work on the CMS end of it, what you're looking for is in the not too distant future. Well in fact was going to do much more than that... but... That project is on the back burner for now.

And no, I haven't seen anything else like it so far.

The thing is: Anything that is like this, isn't going to be easy to use. As long as people want to be able to configure it, need it to be fast, scalability and connect with other systems, it's going to get a little complicated at a bare minimum.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
