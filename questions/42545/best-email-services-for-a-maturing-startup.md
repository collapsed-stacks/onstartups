## Best Email Services for a Maturing Startup

- posted by: [CDD](https://stackexchange.com/users/-1/20086-cdd) on 2012-10-10
- tagged: `saas`, `email`, `ms-exchange`
- score: 3

I run a small but very successful startup, that has been around for 13 months now. We are a 10 person team, but are rely on an aging Exchange 2003 server for our email, calendar, and contact support.

Yikes.

The reason - our initial seed funding was by a private equity firm, that has a diverse portfolio, but unfortunately has been slow to upgrading their infrastructure due to the economy (they were heavy real estate investors, trying to make a jump into different industries). 

As an affiliated/child company, we were happy to get our email set up for us without extra cost or effort, but with such an aging system, its really starting to become a problem. If you needed further confirmation, Exchange 2003 does not work well with Mac OS Mountain Lion... At All.

So now that we're growing at a faster rate, and this email/calendar problem is starting to become a problem for the business. Luckily, its my job to solve it.

What are the recommended 'best practices' to get enterprise-grade email/contact/calendar support for a 10-250 person company? At the current rate, we think we may need to support that many users in the coming 1-2 years, so I'd like to develop a program that is going to work for us until we can afford to drop $50,000- $100,000 on our *own* Exchange 2016 server.

Something I've learned in my life (that has kept me away from Google, in particular) is that it is of utmost importance to *own and control* my information. I do not want anyone searching or using my email content for 'Big Data' initiatives, and I absolutely want the ability to delete, export, and update what I want, when I want, where I want. Obviously obeying any/all laws - I do not want that to sidetrack the discussion, please.

So I figured I'd ask the other businesses on Stack Exchange - Does anyone have some advice on what to do? I've looked at Rackspace, Office 365, and a couple of others, but have not yet made a real commitment. Anyone have experience conquering a similar problem and have any advice for a young startup founder?

Thanks for any comments,

Charlie


## Answer 42570

- posted by: [OnTheShelf](https://stackexchange.com/users/-1/17699-ontheshelf) on 2012-10-11
- score: 3

I am a year plus into my most recent start-up, having a background working in both start-ups and having worked as a senior manager in the biggest two companies in Seattle (airplanes and software). In those massive companies we had every bit of technical infrastructure we wanted (and some dog food we did not want). When I left to start my current company I was really concerned that I had become used to the luxury of having Exchange, SharePoint, IM, VOIP, etc.  I had looked into Office365 (formerly BPOS) while at MSFT and was sincerely impressed with the dedication to security and the Software as a Service model they were rolling out.  So now eighteen months or so later...

**Office365 is by far the best service offering I have seen in my thirty years, especially at the $6/person/month.**  You can start with as little as ONE seat (total bill $6), and add and remove people any time you want with instant web portal provisioning.

Each person has FULL Exchange 2010, connected to Outlook on the desktop, WebAccess, iPhones, Windows Phones (also incredibly good), Android, etc. We have full online presence information, so when you are typing an email to someone it tells you if they are online, etc.

Each person also has full Lync on their computers and mobile phones.  It includes full HD video chat, audio and instant messaging, and unlimited size file transfer. All encrypted.  You also get full screen cast and online meetings with Lync online. We even tested the file transfer functionality. For pure amusement we dragged and dropped a 4 GB ISO file of Windows 8 onto Lync and the transfer worked perfectly despite the size. Our filed tech even installed Win8 from that ISO file to confirm it worked.

The most underrated feature is SharePoint online. Even with only one seat (license) you get a public website that you can "back end" with SharePoint parts. Dead simple and easy to maintain.  You also have private internal SharePoint sites for your team, as well as any special projects.  We make a separate SharePoint site for each client project, so each project team has separated file storage, calendar, task lists, wikis and more. You can even invite NON-Office365 guests using free Windows Live/Hotmail or Outlook.com accounts.

I could go on for another several paragraphs about extra functionality you can use, such as building mobile web applications against Windows Azure, and your Office365 accounts already use Azure Active Directory. That gives you a fully deployed mobile web cloud that works across the world. Again that Azure Active Directory integration is FREE with Office365.

My one complaint (and they are working on this) is being able to upload my own SSL certificate for my public website. Everything else is already full SSL using MSFT (x.509) certificates.

I have found using a private Lync cloud so useful with one click screen sharing, etc. that I have bought a few $6 accounts for my non-technical parents. Now they can see my presence (including when I'm "busy" in a meeting), and I can have a quick (secure) video chat with them. From that conversation view I can take over their computer screen to offer assistance. The functionality is fantastic.

Just for extra information there are Exchange Online ONLY accounts (no SharePoint or Lync, etc.) for $4/person, and accounts all the way up to $20/person that include FULL Office 2010 (soon to be Office 2013) for up to FIVE computers per user seat. So if you have a $20 account for "Jane" she can install Office Pro on her work desktop, work laptop, home desktop, husband's laptop, AND her new Windows 8 tablet (you know Jane wants a new Surface tablet), all under that same one seat license.

So while I can get all the MSFT software including Exhcange essentially for free, and I know how to setup and manage Exchange, SP, Lync, etc., the Office365 price and features made it a no-brainer for my start-up.  I will never go back to the time and money to manage my own infrastructure for those services.

BTW, I think you get a free evaluation period with Office365.  Good luck and I hope this helps.


## Answer 42571

- posted by: [NeedAGeekIndy](https://stackexchange.com/users/-1/19608-needageekindy) on 2012-10-11
- score: 1

We have been extremely happy with Google's services.  They do not mine data of paying customers, or clutter their webmail with ads and such.  $50/user/year is extremely reasonable.  We were early adopters and have had no downtime that we have noticed.  We work with some companies that use Exchange and Office365 and they have all expressed issues with inefficient spam filtering.  We have had absolutely none of that.  No false positives, and I cannot recall a single bit of SPAM getting through to my inbox, nor have I heard of anyone mentioning that they have.

We really could not be happier.  It does everything that we need, for a great price and it just works.


## Answer 42582

- posted by: [Luis](https://stackexchange.com/users/-1/16751-luis) on 2012-10-12
- score: 0

While you don't buy the Exchange 2016 you mention, perhaps you can find [DavMail](http://davmail.sourceforge.net/) a very useful and cheap (no cost) solution.

From the website:

> Ever wanted to get rid of Outlook ? DavMail is a
> POP/IMAP/SMTP/Caldav/Carddav/LDAP exchange gateway allowing users to
> use any mail/calendar client (e.g. Thunderbird with Lightning or Apple
> iCal) with an Exchange server, even from the internet or behind a
> firewall through Outlook Web Access. DavMail now includes an LDAP
> gateway to Exchange global address book and user personal contacts to
> allow recipient address completion in mail compose window and full
> calendar support with attendees free/busy display.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
