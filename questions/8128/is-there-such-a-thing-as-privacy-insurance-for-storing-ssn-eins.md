## Is there such a thing as Privacy Insurance (for storing SSN/EINs)?

- posted by: [Yasmine](https://stackexchange.com/users/-1/2564-yasmine) on 2010-02-16
- tagged: `privacy`, `software`
- score: 3

Part of my service includes storing social security numbers (SSNs) and employer identification numbers (EINs). I went through the proper protocol of setting up a separate server to store them, ensuring they're encrypted, adding hash functions, making sure the data is secure and writing a PCI compliance policy. I recently heard I'll need insurance as well in case my data was compromised. Does anyone know if this is true and if so, what type of insurance I'll need? 


## Answer 8211

- posted by: [James Black](https://stackexchange.com/users/-1/1074-james-black) on 2010-02-18
- score: 1

You can find companies that will give insurance on just about anything, but, is it worth the cost?

For example, if you have your critical info encrypted, and the key or passphrase is not on the computer, then even if someone stole the hard drive they will not have anything that will help them, but, you may want to protect that the key wasn't flushed to the hard drive when the computer went to sleep, for example.

The basic idea is to ensure that if someone with infinite resources, except time, had the hard drive, could they recover the social security numbers?

If they can't then don't worry about it.

There are so many instances of companies losing this type of data, that it is unlikely they are required to be insured, otherwise they would have taken more steps to protect the data.

Is your server behind a firewall?

You may find that using something like truecrypt may be helpful, in that you not only encrypt the hard drive, but you actually hide the fact that the data is there, so, you log in, start your database, it works fine, but should the computer be stolen, when they go to log in, the thieves won't even know that there is a hidden partition with sensitive data.


## Answer 8215

- posted by: [Gabriel Magana](https://stackexchange.com/users/-1/1158-gabriel-magana) on 2010-02-18
- score: 0

I think you need to state which laws you are trying to comply with in order to determine if you need insurance. How do you know you "need" insurance for that stuff?


## Answer 11961

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-06-10
- score: 0

Are you trying to sell a product you made that complies with PCI credit card rules for holding transaction inforamtion?  If so a company may not want to buy the product without some type of protection from fines.  There maybe other legal pieces as well so I'd suggest seaking attornies advice on what the impacts are and then see if this is a marketing decison or a legal one.  (Do I need it to sell or is it a feature as a gaurantee.)


## Answer 15412

- posted by: [Frank](https://stackexchange.com/users/-1/4858-frank) on 2010-10-21
- score: 0

BEST PRIVACY INSURANCE...
Incorporate your business in PANAMA!!!  You will not be subject to the same rules and regulations that can put you out of business.  Worst case you fail.  You get hacked.  Even with PCI compliance, and all security measures you always risk getting hacked. 

Best not to store it, but if you have to, try to minimize your legal risk by using a more friendly jurisdiction.  





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
