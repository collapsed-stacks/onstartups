## How is Wattpad.com monetized?

- posted by: [Mark0978](https://stackexchange.com/users/-1/10006-mark0978) on 2012-06-27
- tagged: `venture-capital`, `monetization`
- score: -2

This is a link to the press release that Wattpad has received and additional 17+ million from come venture capital groups. [Wattpad press release][1] Those venture capital groups must see some way to make money at a service like this.  

All I've been able to discern is that Sony paid to have a story placed on Wattpad (but I don't know if they paid Wattpad, or just the author)  Sony then hosted a contest on Wattpad around the story they paid to place.  But the site has 1 small add at the bottom of the page, no ads in the margins or seemingly in the stories.  I can't for the life of me figure out how they managed to attract that kind of capital.

I didn't even know Wattpad existed until about 2 days ago, yet they were prototyping back in 2002.

I'm interested because I have an idea that is vaguely similar to [Wattpad][2] and [fanfiction.net][3] (which has many ads per page) but if Wattpad can do what they are doing without ads, I'd love to go that route, I just don't see how they can profit without either charging a membership fee, or showing ads....

EDIT

I've since discovered that Collusion for Chrome was blocking some of the ads, however the ads they have are the same kind of low value ads that haven't paid us a dime in the last 6 months because they are ads that no one would be interested in.  I have discovered a few things that might lead to an answer, if I knew how to connect the dots.

When you load a Wattpad page, you get the following JS code loading (No Script is a wonderful add-on)

I'm pretty sure these guys aren't paying wattpad to include their Javascript,

    facebook.com, fbcnd.com, facebook.net
    twitter.com, 
    pinterest.com
    googleapis.com, google-analytics.com, google.com, 
    quantserve.com     (Measure your audience for free)

I'm now actively wondering which of these "trackers" are paying.

    adnxs.com                (AdNexus/AppNexus, requires a pw to see more, AdNexusMedia?  [more info][4] )
    
    rubiconproject            (First choice for Comscore 500 publishers)
    scorecardresearch.com     (Creates your ComScore?)
    tribalfusion.com          (ads)
    revsci.net                (Audience Science
    fastclick.net, apmebf.com (Valueclick.com,  hodgepodge of ad like stuff)
    gwallet.com               (RadiumOne.com, social ads)
    addthis.com               (ClearSpring Technologies)
    exponential.com           (Advertising Intelligence)
    mediaplex.com             (Tracking)


Maybe I've been naive int thinking how you monetize a "free", I thought you displayed ads, hoped people clicked them, and made money that way, I'm beginning to wonder it some of these guys are paying just to track you, and what kind of backend info the get from the page, I'll have to dig into the JS they are running on the page tomorrow.

Anyone know if they really pay sites directly for the tracking info?  This seems like a monumental list for 2 measly ads on the page and one at the bottom of the frame......
 

  [1]: http://blog.wattpad.com/post/24538462109/wattpad-funding-17m
  [2]: http://wattpad.com
  [3]: http://fanfiction.net
  [4]: http://www.donottrackplus.com/trackers/adnxs.com.php



## Answer 40230

- posted by: [JohnZ](https://stackexchange.com/users/-1/18439-johnz) on 2012-06-27
- score: 0

Hmm, they could potentially charge authors to upload a story; like the Kindle store does...

What about mailing list with special offers, paid for by advertisers.  

Also, there seems to be a large user-base, they could find a new way to monetize that, such as by implementing new features.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
