## Do you *mark* your products' installers?

- posted by: [Krasimir Evtimov](https://stackexchange.com/users/-1/2262-krasimir-evtimov) on 2010-01-21
- tagged: `application`
- score: 5

Do you use any unique markers in your products' installers in order to track if some pirated version of your app starts circulating on the warez sites?
What I mean is: do you put some customer specific information in every installation before the customer downloads the software, then if later you discover your program on some warez site, you'll know exactly which user to talk to.

I'm still way to early to worry about such things, but I just wonder.


## Answer 7045

- posted by: [Peter Olsson](https://stackexchange.com/users/-1/2161-peter-olsson) on 2010-01-23
- score: 2

We actually add the customer information in the installers, making each installer unique. The reason is to make it easier for the users, not to track pirated copies.

**I would not recommend it though.**

For us the choice was between having to several different installers, do some advanced scripting that alwasy would work on all OS combinations or to come up with a way to patch the included software (it took a while to get the vendors to agree to this).

The drawback is that you will have to build each installation from scratch or that you can't use most of the installers. We have found one installer that with a bit of tweaking allowed us to patch things into the exe-file while customer is downloading the file from our web server.

I would focus on making a good product and making the product as easy as possible for the users that want to pay for the it. Many users that would use a pirated copy wouldn't have bought your software anyway, they would just have used some other software. Isn't it better that they use yours? Some time in the future they might turn into a paying customer.

I'm not advocating to use pirated software. I'm just saying that a startup shouldn't worry to much about it. If it turns out to be a problem and that it is affecting the sales (i.e. it is easier to use a pirated version then to pay and use the real version) it is time to do something about it (probably to make it easier to buy and install the real version).

Finally:

The information about which copy that has been pirated is probably useless. Most customers are very loyal and don't leak copies to warez web sites intentionally. It is a lot more likely that someone copied the software without their knowledge.



## Answer 6994

- posted by: [Mark Beadles](https://stackexchange.com/users/-1/296-mark-beadles) on 2010-01-22
- score: 1

Well, first of all, remember that if you trust your customers, they will be more likely to trust you. Also, I assume that you have considered the cost of piracy vs the cost of whatever scheme you choose for software keys. 

Finally, ask yourself: if you did find out that a copy of customer X's software had made it onto a Warez site, what would you do then? You say you'd "talk" to them -- to what purpose? Legal action, etc.? You should consider the costs and benefits of whatever enforcement action you might take. Software tracking (a form of digital rights management/DRM) is a valid tool, but be sure that it makes sense in your particular case.

Now if you decide to do this, the standard way of doing it nowadays is via a product/license-key mechanism. Think of what Microsoft does with product keys, for example, or what most game software does with a license key. A license key will allow you to control who can use the software. Then when a license key becomes compromised/published, you will know exactly whose it is.

http://en.wikipedia.org/wiki/Product_key has more information on this mechanism.


## Answer 7044

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2010-01-23
- score: 0

Not sure how something like that would stand up in court if you were to pursue legal action but at least you would have the option.  

If you pass the internal serial number to your server as part of a "check for update" feature it can also prove to be a way to track how your software gets disseminated / how many different machines a single license is installed on.

At some point though you cross the thin line between protecting yourself and invasion of privacy so I would be careful.  Think about how you would react as a user.  

Personally, I sell our software as a service which is the easiest way to protect your software.  If that were not possible, would not bother with marking installers but instead focus more on making your software affordable and making it *very easy* to purchase a license.  Facilitating honest use is easier than engaging software pirates in an arms race.  



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
