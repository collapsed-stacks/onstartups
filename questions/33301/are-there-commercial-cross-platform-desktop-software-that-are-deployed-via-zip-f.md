## Are there commercial cross-platform desktop software that are deployed via zip file with no installer (just let user extract and run)?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2011-12-04
- tagged: `software`, `desktop`
- score: 1

Due to technical limitations of a 3rd party library I am using, I am forced to deploy my application in a zip file, containing a .bat script that will launch the application.

How important is the installer for the user? Would someone not buy a product because they have to extract the zip file to a directory and run it directly from there?

I plan on purchasing installer generation tool AFTER I make the first couple of sales. They are quite expensive ranging from $2000~$4000.

So my question is could I get away with letting customers download software product bundled in a zip file? They need to extract it and run the .bat script inside to run the application. No exe files available.

The application still notifies the user if there's a new update available for download but the user has to download it themselves and this update doesn't happen automatically.

Update:

Application requires Java and is cross-platform (doesn't run just on windows but mac and linux), the OS specific native libraries are 32-bit. This means I have to bundle the 32-bit JRE with my application. Because there is no open-source free installer that does this very well (launch4j has this option but it does not support forcing the application to run with the bundled 32-bit JRE). JWS does not do this as well. My only option is to use zip or a commercial installer it seems. I left out this technical detail so I wouldn't get into the technical talk (I have SO for that) and to see if I could get away with just using batch file to launch app as my only other option seems to be purchasing the installer.


## Answer 33318

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-12-05
- score: 3

To directly answer your questions:

> Would someone not buy a product because they have to extract the zip file to a directory and run it directly from there?

If you are not offering a trial, most people would have bought the product before they install it. So, I don't think it's a factor of if they would purchase it or not.

> How important is the installer for the user? 

I think it is pretty important for installation to be easy when installing a product. And if you packaged it as a zip and I un-zipped it and there was a READ-ME-BEFORE-INSTALLING.txt I would read that. However, that's not a great experience.

But, if your product is great I imagine your users would deal with it until you get a solid installer. More important to start getting it out in peoples hands as soon as possible.






## Answer 33309

- posted by: [Propeller](https://stackexchange.com/users/-1/14813-propeller) on 2011-12-04
- score: 1

I don't get why you can't just create a self-extracting archive? That way they still get the "installation" so-to-speak without having to do any extracting themselves. I use WinRAR for these kinds of things. It has a built in SFX feature and it lets you customize what users see on the self-extractor. WinRAR is $29 to purchase but if you would like a free one, 7-zip also has this feature although, it doesn't let you customize the extractor.

If you are trying to achieve something specific, you can comment it below my post and I'll try to see if there's more I can help you with.


## Answer 33302

- posted by: [NetTecture](https://stackexchange.com/users/-1/3350-nettecture) on 2011-12-04
- score: 0

> Due to technical limitations of a 3rd party library I am using, I am forced to deploy my 
> application in a zip file, containing a .bat script that will launch the application.

As someone doing installation for 15 years or so that sounds ridiculous and wrong. Point. Because nothign says an installer can not doo pretty much just deinstallation. I would love you to rpoove me wrong here, but I dare saying it shows you are clueless how installer technology (under windows) is working and supposed to work - otherwise you would not say you are FORCED to to something in a zip file.

> Would someone not buy a product because they have to extract the zip file to a directory and 
> run it directly from there?

Pretty much every enterprise. And you never get windows application certification - which is a significant step either. At the end they willlaugh at you and do what you obviously dont want to do - package it up in an installer.

> I plan on purchasing installer generation tool AFTER I make the first couple of sales. They 
> are quite expensive ranging from $2000~$4000.

Yes, especially if ysomeone buys them who has no clue. See, some years ago MS was publishing their own installer open sourcee frameowkr for free - the same running the installations of like Visual Sdutio. WIX. It is now a free download. Makes 0 USD. It requires a little more knowledge than most do (no fancy UI but a XML file) but it is fully controllable. Oh, and you better know what you are doing.

> So my question is could I get away with letting customers download software product bundled in 
> a zip file? They need to extract it and run the .bat script inside to run the application. No 
> exe files available

Yeah. I mean, what is wrong ith screaming "unprofessional" all over your product? It takes 5 minutes to make an exe file that just does what your batch file does, and it allows you to set an icon for the file. You can get away with it. You can also get away with murder. CAN. Not advisable.

> The application still notifies the user if there's a new update available for download but the 
> user has to download it themselves and this update doesn't happen automatically.

I hope you only target private users for this. Self updating should be something admins disable with install.

In companies softare is centrally deployed and updated and users have no right to just start programs without installation.

PLEASE get basline professional.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
