## Who handles sales tax on apps (android on google play, ios on appstore, android on amazon app store)?

- posted by: [S.A.Jay](https://stackexchange.com/users/-1/19190-s-a-jay) on 2012-08-10
- tagged: `sales`, `tax`, `apps`, `android`, `apple`
- score: 1

Ok, I am a one person developer and I have an android app on the google app store I also have it published on the amazon app store.   I plan on eventually publishing a version on the apple store as well.  My question is who handles the sales tax for the people that buy my app?  

I have found pages for Google, Apple, and Amazon about sales tax but they don't all make sense to me.  

 - [Amazon App Store][1]
 - [Google Play][2]
 - [Apple AppStore][3]

On the Google store it made it seem like I was completely in charge of it and told me how to adjust it.  The amazon app store seemed to say the same thing, but I had no place to enter sales tax rates for the different states.  Then for the Apple store it seems like apple handles that for you completely on their own.  Plus I don't even know where to start on foreign sales tax.  

Any help would be greatly appreciated... 


  [1]: http://www.amazon.com/gp/help/customer/display.html?nodeId=468512
  [2]: http://support.google.com/checkout/sell/bin/answer.py?hl=en&answer=73973
  [3]: http://www.apple.com/legal/itunes/us/terms.html


## Answer 41249

- posted by: [littleadv](https://stackexchange.com/users/-1/13808-littleadv) on 2012-08-10
- score: 1

You're responsible for sales tax, usually. You should only be charging the taxes you can remit to the appropriate authority, and only to the authority that has jurisdiction over **you**. So, if you're in California - you charge CA sales taxes, per CA laws (check what exactly is taxable and how on the BOE site). You shouldn't charge EU VAT if you're a California entity, for example.


## Answer 41297

- posted by: [Matt](https://stackexchange.com/users/-1/19221-matt) on 2012-08-13
- score: 1

On Google Play, for instance, you need to determine the rules that apply to you, for the combination of your location and each selling location.

Unfortunately this may vary not only by country but by US state.

For the US... Generally speaking, you will need to pay tax wherever you have 'nexus' (a physical presence in that state - e.g. building and/or staff).  If you are outside the US that might be nowhere. Things are changing in some states, however, so you need to keep on top of the news here.  In particular keep an eye on Arkansas, New York, North Carolina, Rhode Island and Illinois.

For the EU... I am researching this at the moment, but it looks as though you are required to charge and submit VAT on sales once you reach a certain threshold.  Again, this is different per country.  In most cases it's high enough not to worry unless you're making Angry Birds 2 - BUT in Germany and Spain it is 0 (!)
 
If you are located in the EU, you are able to register with your home country and charge VAT at their rate, for all EU sales (this changes above a threshold, whereupon you have to register in each country separately).  

If you are outside the EU then you can use VOES to avoid having to register in each country:  http://bit.ly/O0XDnv
Even if you are a low level seller, this might be worth considering if you are worried about Germany & Spain.


For other countries, guess what - it varies !  Note South America has some 0 threshold countries.

The majority of small-scale app developers seem to be unaware of the above and are doing nothing about sales tax outside their own location (yet selling worldwide).  Whilst you'd probably get away with this if your sales are not significant, I wouldn't recommend it if you're selling significant numbers.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
