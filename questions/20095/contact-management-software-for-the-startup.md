## Contact Management Software for the startup?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-11
- tagged: `software`, `crm`, `contact`
- score: 6

I am curious what very small companies and solo types here use for contact management.

What I am going to do with this system is the following. I sell a B2B service. I intend to call businesses and present myself. (It's cold calling - PLEASE don't hijack that related topic, I'm not here to debate that.) I then want to collect the business contact information for the places I have called and send them a personalized follow up letter. That's my current plan: a simple "drip" marketing campaign.

I want to start marketing my services and I believe that a usable contact management system is at the top of the list of must-have tools. I do not expect to expand beyond one user (myself.) I want to have something that can support mail merge and linking to external files. Decent usability is a prime consideration. 

I've evaluated a few products so far. My impressions of each follow. Also, some accompanying entertaining, subjective rants. 

SugarCRM and vTiger (a Sugar derivative) - way - hideously over the top for what I need.
"Too" configurable. Too intrusive on my desktop system, requiring an Apache/MySql stack to
be installed. Both are "slow" by desktop standards because both rely on web access. 

Initially I was enthusiastic about vTiger, but an attempt to import CSV files much over
100 records caused the import process to bomb with a blank screen. I attempted to research the issue and even after following comments on the vTiger support fora I never got it to import more than a few dozen lines of my data at a time. 

In my strong opinion, you really need a separate support person role for Sugar or vTiger.
The logic I employed here is that when I run into a hurdle with a relatively simple function in an open source tool, I know that the entire product will be similarly challenging to deploy. These Sugar variants are big, complex, and require tinkering. And vTiger is just too rough around the edges for this one man act to bother with. 

Zoho just seemed limited, although very nice for what it is. 

ContactPlus - very jarring, dated, ugly UI. Looks like a 1996 vintage Delphi application
(I used to love Delphi, that's another story.)

Maximizer - a 1.2 gigabyte download, installs SQL Server on your desktop. ARE YOU KIDDING
ME! The eval copy expired after I didn't touch it for 15 days so I suppose I will never
know. :) The product had an "overwhelming" feel to me, another "too much" product. 

There is the rest of the field, of course. Google returns hundreds of distinct hits for
"contact manager". Also, everyone wants to sell a "CRM" as SaaS and charge monthly prices. Regardless whether the business model of the CRM vendor is SaaS, I really think that I want a desktop application that I buy outright. 

Finally, I found one program that I actually like, very much so far:

Chaos Software's "Intellect" - an advanced version of "Time and Chaos". 

Importing my data was a breeze. It actually worked. One thing I didn't like: Intellect
does not have a way to save an import field mapping. So you must redo the field map every
time you import. vTiger has this feature, and it made importing the same kind of file multiple times very easy.

The UI is clean and lightning fast. 

The UI is not very configurable. However, it's pretty close to what I would want ideally. 

The user defined fields can work OK for me. 

The "Find" feature is a bit clunky but usable. The "tagging" feature could stand some
spiffing up but is usable as well. 

I can compromise on these things. I just believe that Intellect "nails" what one person
actually does with a contact manager.

So my questions to you folks are:

What contact management systems do you use? 

Anyone here use Chaos Intellect? 

Anyone here use something else much better, and want to defend it as a superior tool? (I
am not going to debate. I am simply interested in experiences and other people's
judgement.)

In essence, I want to know if I am about to choose "the best" product for purchase and
incorporation into my workflow. And please note, I really don't care about multiuser operation, outsourcing the data, or accessibility everywhere. 

Also, price is not a huge deciding factor. "Intellect" is $60 and Maximizer is $200 but the major expense here will be the effect on my own effort over the months in using whichever program I choose. 

Thanks for any insight, experiences, etc. 


## Answer 20158

- posted by: [darren](https://stackexchange.com/users/-1/7271-darren) on 2011-02-12
- score: 3

37 signals have a great ecosystem of products with Highrise being their CRM solution. I went through a similar process checking what was available around 14 months ago and choose Highrise and still have solid conviction in my choice today.

While there may be more fully featured alternatives, Highrise concentrates on one thing and does it superbly.

Highrise plays well with not only other 37signals products [basecamp, campfire and backpack] but also is within a SaaS ecosystem (through APIs) that includes,

Zendesk http://blog.zendesk.com/blog/2008/08/integrating-wit.html

MailChimp http://www.mailchimp.com/

Wufoo http://wufoo.com/

Harvest http://www.getharvest.com/ (built with Rails)

Gmail https://mail.google.com/mail

and many many more, see: http://highrisehq.com/extras#service - make of this what you will but to me it shows a real strength in market position and has made my life easier as I use all of these also (they are really all great products! and also wonderful to use!).

This product works both with iPhone and Android, and each of 37signals products has an API so you can extend the product however you feel.

…also its free to start using (2 users, no files, 250 contacts) or up to $99 a month

The guys that built this have pedigree, David Heinemeier Hansson [a partner at 37signals] is the creator of Ruby on Rails, a NYT best-selling author… and more

Jeremy P's mention of http://rapportive.com/ is a great to see some extra info in gmail also

I hope this helps, and good luck


## Answer 20110

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2011-02-11
- score: 2

The best one I have used is Highrise by 37 Signals. 

Sugar CRM can be installed free but it's pretty heavy weight. We found that Highrise was good enough for our small company and it was worth the money. They do have a free option.


## Answer 35473

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2012-01-30
- score: 2

After some stumbling for months with Intellect by Chaos Software I am dumping it and I cannot recommend it to anyone. 

There were many issues in day to day use. The single largest issue is that the searching functions are primitive and idiosyncratic. Also, Intellect in general felt like a disconnected island with respect to the web and for connecting to external data sources. Also, the UI was really cumbersome. I found that in practice it was agonizing to use. Fighting this each time I used the program *really* wore on me and I avoided using it. 

I had a Zoho account and I played around with it. While I liked the overall structure of it, some of it seemed quite mysterious, particularly how to search on custom fields that I defined. Also, I want to own my data, not host it on someone else's cloud. Lock-in was an issue for me. 

Ok, here's the answer to my original question: SugarCRM, installed into either a virtual machine on the desktop, or on a web host (even shared worked OK but it was slow.)

I found that the current beta release of Sugar installs with no real problems. Installing it is almost exactly the same as installing any other web thing like a message board or a CMS or Wordpress. Just bigger. 

It is relatively straightforward to customize its field structure and UI to exactly what I need. It's big and heavyweight but quite logical. 

And unlike Intellect and other lower end applications, it supports the notion of multiple lists for leads and allows targeting and segmentation of groups. 

Also, I found that while I am an "old desktop guy", the web interface of Sugar is really much more usable than a fat client GUI. Just one example - the ability to highlight fields and do "ad hoc" web searches is quite useful. With a desktop app, all of those things are just beyond your grasp. 

If one has the technical skills to handle setting up and configuring a relatively complex PHP/MySQL application, then I recommend adopting Sugar and giving it a serious trial. 

I am looking forward to working with it. 

I am not certain if it is fair to accept my own answer, but perhaps the best answer to me back then probably would have been "install and learn Sugar." Even though I rejected it at the time. 


## Answer 20097

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-11
- score: 1

Two solutions that you didn't mention are easy to learn, low cost and powerful. I have used both and either one will let you stop worrying about contact management/sales activity tracking and just get busy building your business.

 - Microsoft Outlook 2010 with Business Contact Manager
 - Sage Act!

MS Outlook with Business Contact Manager is the one for you if you are familiar with Microsoft Outlook and like it.  There is almost no learning curve and you can get to work on your business right away.  If you like Outlook just download the update and move on.  You may also be able to synchronize your tasks/schedule/contact management to your blackberry via exchange server or a desktop sync.

Sage Act! is the one for you if you don't like Outlook, or if you are very interested in fully supporting a mobile/cellular device as an extension of your contact management. Act! is fully featured, more so than Outlook, but it is also very well organized and will guide you through working with it so it's easy to get up to speed.


## Answer 20100

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-02-11
- score: 1

<p>If desktop apps are totally your thing, the default choices for solo stars are:</p>

<p><a href="http://www.sage.co.uk/software_and_services/customers/act_by_sage.aspx" rel="nofollow">Sage Act!</a></p>

<p>...and I was going to add Goldmine, which was always more geared to teams but had a following with more campaign-oriented sales people, but it looks from their website that FrontRange may be positioning out of the solo market.</p>

<p>You may want to consider cloud solutions as a complement, even if your experience right now is that you're not getting the responsiveness you need for the your campaigning. If you use gmail (or Google Apps), take a look at <a href="http://rapportive.com/" rel="nofollow">Rapportive</a>, which puts some useful CRM functionality right by your inbox. </p>



## Answer 20360

- posted by: [Marcy Hoffman](https://stackexchange.com/users/-1/7026-marcy-hoffman) on 2011-02-17
- score: 1

<p>As a disclaimer, I will talk about my company. The products listed above are excellent but too many of them are single use tools. From my own experience in start-ups, you need to use tools that can not only expand quickly but tie in with other essential tools such as calendar, task management (excellent for dev teams), knowledge base where you can store your docs, presentations etc. And all these apps need to synchronize your data. Check out <a href="http://www.infostreet.com/cloud-apps/" rel="nofollow">Infostreet</a>- it is priced for the SME market and is ideal for your needs.</p>



## Answer 20387

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-02-17
- score: 1

I'm surprised nobody mentioned salesforce.com.. If you are looking for a solid solution, that's definitely the leader. Disclaimer: I work there. just have a look and make an opinion for yourself.



## Answer 20390

- posted by: [Nilesh](https://stackexchange.com/users/-1/6985-nilesh) on 2011-02-17
- score: 1

If you use Google apps for your domain then recently I have been trying insightly that is available in the google marketplace and it is a free application. It integrates with your google email.


## Answer 23130

- posted by: [BerggreenDK](https://stackexchange.com/users/-1/5577-berggreendk) on 2011-04-10
- score: 1

I agree with those mentioning HighRise, but also remember another important thing. You mentioned that it should be easy to import contacts. Think EXIT strategy too. It ought to be easy to EXPORT contacts too, so that you arent stuck with whatever solution you decide on.

I would recommend to go with any product that seems to fit your needs (money, time, features) as long as it has a good IMPORT and more important EXPORT capability.

Once you can test something quickly and also exit the thing once you grown, then you are pretty safe.

http://37signals.com/ is a good place for StartUp's if you ask me. I used Basecamp for a few years, and then decided to go for a custommade solution afterwards.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
