## What are the options for remote desktop support?

- posted by: [Joseph Barisonzi](https://stackexchange.com/users/-1/8791-joseph-barisonzi) on 2011-06-30
- tagged: `infrastructure`, `it`
- score: 2

I am working with a client in the United States that as part of a comprehensive strategy to spin several divisions off as new start-ups is looking to outsource the IT department to a "remote desktop support" provider.  The new start-ups need to develop their own IT environment, just like a new start-up would need to get hardware and software. 

The client is not a technology company. the new start-up divisions will not be either. Technology is not their core competency. They have no desire to continue to maintain an internal IT department. The situation of these spin-offs creates an opportunity to do their IT differently. 

They have between 25-50 users with a mix of basic and power users. It is currently a Microsoft environment, through there are several key applications of an open source variety. they are challenged by their relatively remote location and the lack of reliable high-speed internet.   

I am having a difficult time finding local vendors and I am coming to this community for assistance. 

 - Based on your experience, how important is it for the "remote desk top vendor" to be local? And how local is local?
 - What are the key words to search for as I am unable to find competing local vendors?
 - What solutions are I not thinking of? 




## Answer 26991

- posted by: [Robin Vessey](https://stackexchange.com/users/-1/984-robin-vessey) on 2011-06-30
- score: 1

My company is a software/database maintenance company, we look after a range of customers around our city. We also engage an IT support company to monitor and maintain our servers, they are conveniently located a few streets away.

Local is important for the few times you actually need to be onsite. We meet regularly, 1-2 hours every week or every fortnight depending on the client. To understand their needs, build relationships and work through issues and new goals they have. 

When it comes to actually writing the code and fixing their databases normally we can do those things remotely, but very occasionally we have to walk in and press the reset button or drop off a new computer.

The IT services company that looks after us come in once a fortnight and talk to us about what is happening, what is running slow and while again, they can do most of it from the office there are some things that need diagnostics plugged into physical machines and externa HDD plugged in to sort out something.

**Put it in the cloud**.

If the startups are truly getting to start again, then depending on their operational requiremnets you could consider a "cloud" solution for nearly everything making the need for local support less.

You can host email with hosted exchange or gmail, document storage can be in a hosted sharepoint or if there is no legacy you could be better off with a hosted wiki / google docs environment. Looking at all the needs and identifying how you would apporach this is key. 

Stumbing blocks are likely to be custom built systems or high volume items like video, high res graphics, "design" style items which are going to be your key stumbling blocks and likely to still need in-house servers.

If they can get down to just peoples PCs on their desks and maybe 1 server to manage the domain with everything else mapped into the cloud THEN you can change the IT services needs a lot. 

This really comes down to what sort of businesses these startups are, what their needs are for the IT systems.

**Local backups**.

A key thing to include in your place is anything stored locally should have a constant backup service backing up the the cloud. Tape and other backups are very old school and should be avoided. There are services now which all your changes can be uploaded in the background and if you have a failure many of them can turn on a virtual machine which mirrors the one that has failed ... you can then keep working off it or get the things you need to restore the server. This is much better than waiting the 8 hours for the backup tape to restore the image back.


**Finding local vendors**.

For some reason most IT / Developers suck at marketing (self included) and it is hard work to find them even when they are there. Try google maps zoomed to your area and searching for businesses and guessing what they would have on their website.

 - IT Support 
 - Fix your computer
 - Outsource your IT needs
 - Having computer problems

I'm not really sure, we found ours through referals. 




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
