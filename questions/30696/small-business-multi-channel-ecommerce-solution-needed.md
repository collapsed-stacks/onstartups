## Small business multi-channel ecommerce solution needed

- posted by: [MarkS](https://stackexchange.com/users/-1/13538-marks) on 2011-09-26
- tagged: `ecommerce`
- score: 4

I'm involved in a three-person start-up, selling physical products on the web via:

 - Our eCommerce store (either a high-end hosted cart (Lemon Stand? 3dcart?), or a cart we'll host ourselves (Magento?)
 - eBay
 - Amazon Seller Central

One set of inventory that all three draw sales venues draw on, some drop-shipping involved.

The main question: How do we keep inventory and other product attributes in sync across the three channels. How do we funnel all sales into a single shipping solution. 

While in the start up stage, we need to maintain a broad enough inventory, but not have to much cash wrapped up in inventory. So let me give a quick example: Let's say we have 4 of some expensive item in stock.  We want our inventory to appear to be 4 on our cart, eBay and Amazon. If a customer buys 3 of that item, I want the cart, eBay, and Amazon to now report that we have one in stock.  I can't have the inventory in three places reporting as 1, 4, and 4.

And we don't wand to deal with three systems to print invoices, handle shipping and posting back package tracking information. 

What's available for the small start up in this area?




## Answer 30864

- posted by: [juan2raid](https://stackexchange.com/users/-1/2537-juan2raid) on 2011-09-30
- score: 1

http://www.solidcommerce.com/

http://www.monsoonworks.com/

I haven't used either of them but i know they do at least some of what you are looking for.


## Answer 30905

- posted by: [Jontas](https://stackexchange.com/users/-1/11243-jontas) on 2011-10-02
- score: 1

Since you mentioned Magento here are some examples to get the flow you wish. If you go down this line, then Magento will be your "master" where the items, stock etc are managed.

You can develop custom modules for Magento to get you these integrations and any others you would like, or you can look into already existing modules.

Ebay: When we were looking at integrating eBay<->Magento we looked at m2e ($199);  when an item is sold on eBay the stock in Magento is updated, and when the stock (or item in the stock) is updated in Magento then the eBay store is updated.

I have not seriously looked into a Amazon Seller Central<->Magento integration but there is a module called Amazon Integration Module for Magento (http://www.camiloo.co.uk/shop/global-amazon-integration/tour/) (£239 or £33/month)

**A word of caution**, for any integrated solution like you describe you have the risk of 2 (or more) customers buying items that are listed on different locations and buying more than you actually have (example if you have 3 theProduct in stock, and userA buys 2 from eBay and userB buys 2 from Amazon at close to the same time, before the updates are pushed to both sides) ... you should be aware of this risk and make sure you are not penalized by the store in this case. I read "[...]Our learning was that if you go out of stock but take an order on Amazon Seller Central it will crucify you for it[...]" (in this blog post http:// star-digital.co.uk/magento-amazon-seller-central-integration) so make sure you know what the rules of eBay/Amazon/you store terms says of this case. 


## Answer 30699

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-09-27
- score: 0

It sounds like a custom development as I haven't heard of anything which does this across so many platforms. 

Each of the "stores" you deal with have APIs which you can use. If you have an inventory management solution alreay or your looking at a few you can get a developer (or do it yourself) to write the integration so that "updating the stores" is handled automatically when a change is made to the inventory management system. 

If you haven't decided on the inventory management solution I would recommend doing an analysis of the various APIs first and then using that as part of your criteria for choosing the final solution. 



## Answer 33457

- posted by: [Molly Griffin](https://stackexchange.com/users/-1/14897-molly-griffin) on 2011-12-07
- score: 0

I know this is a little delayed, but if you are still investigating a good solution that can integrate your eCommerce site (say Magento), eBay, and Amazon Seller Central.

Multichannel Order Manager from Dydacomp provides you the ability (with the an open API) to integrate with your eCommerce shopping cart, while allowing you to import order and synchronize inventory levels for your Amazon and EBay sites as well. M.O.M. enables your to reserve  and lock inventory for EBay and select the products availability for Amazon. This ensures that you keep an accurate inventory count that is synchronized across all sales channels.   Multichannel Order Manager will integrate all your orders into one location and enable your business to process, fulfill, pack and ship orders from one location. 

Multichannel Order Manager was created for small and medium sized businesses to provide the inventory and order management functionalities required at an affordable price. The flexibility of the solution enables you to select the functionalities that meet your businesses individual needs. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
