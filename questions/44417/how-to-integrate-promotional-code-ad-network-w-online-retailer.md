## How to integrate promotional code ad network w/ online retailer?

- posted by: [Jason](https://stackexchange.com/users/-1/21727-jason) on 2012-11-22
- tagged: `advertising`, `promotion`, `ads`
- score: 1

I would like to create a print ad network for online retail advertisers with the following features. The ads will be distributed as posters.

1. The printed ad includes a URL with a link to the ad network's URL, including the promo code: adnetworkname.com/T57

2. The potential buyer would then need to be directed to the retailer's site in order to make a purchase (I am unsure how to integrate this, since I will not be able to control the retailer's site)

2. The system has to be able to track which buyers make a purchase on the retail site (the advertiser's).

Should the promotional discount be given before or after the sale?

I do not want to get too deeply integrated into the order flow of the online retailer, however, I need some control over which buyer used a promotional code (ie. was directed from my advertisement) to make a purchase (without changing the code on the retail's site).

What is the best practice approach in this case?



## Answer 44422

- posted by: [Billy Chan](https://stackexchange.com/users/-1/21618-billy-chan) on 2012-11-22
- score: 0

The idea is basically like an affiliate program. If your online retailers has affiliate program, it would be simpler to utilize it to help tracking.

To track if a sale is successful or not, you can use sub id, which is a popular function in most affiliate programs.

Optionally you can also collect visitors' email, for their accumulating credits in your site, and you can notify them by email directly if any new deals.

###Let's mimic this process###

1. You spread the printing ads on the street
2. A visitor get your ad and find it interesting, then he goes to adnetwork.com/T57 to fulfil this deal.
3. He reaches a splash page when entering above link. Now you can assign him a cookie if this is his first arrival, containing two important info: The promotion code T57 and a unique id using as sub id for affiliate program. 
4. You system also generate a unique affiliate link on the page using above sub id as a GET variable.
5. Optionally you can ask him whether he would like to leave his email so that he will receive more deals in the future by email, and possible credits in your site.
6. Whether he leave email or not, he go ahead following the link/button on splash page, containing your sub id.
7. If he made a purchase, the retailer will give you a sales report containing which sub id made how much sales.

###Report###
Now you have following information:

1. How much printing ad you spread on street - the people received ad
2. How many people will actually follow the URL - By unique cookies you sent
3. How many people really made purchase.
4. The people sign up for your newsletter.

This should be good for your next optimization.

You can also change the promo code T57 to others, for testing different ad versions, different locations etc.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
