## recommend free email client for synching desktop/laptop/blackberry

- posted by: [tim8691](https://stackexchange.com/users/-1/13002-tim8691) on 2011-08-28
- tagged: `email`
- score: 0

looking for recommendations for email eco-system allowing small-business to:

1. let users log into email from desktop, viewing multiple email domains, and reply to each where the outgoing email matches the associated email-domain being viewed; (e.g. replying to yahoo email sends outgoing email using yahoo email domain; replying to me@company.com sends outgoing email using me@company.com; etc.)

2. Desktop/laptop/mobile phone (blackberry) syncs with desktop/laptop (e.g. send email from desktop and can later view it online when traveling, or on blackberry, etc.)

3. Complete access to email on desktop as well as online (e.g. email synchs between online and desktop/laptop/smart phone).

4. Can read stored emails and reply to them offline, then send them once online (e.g. if on airplane, etc.)

Anyone familiar with Thunderbird and/or Zimbra, and how they work in these situations? Also, I'd prefer not to get targeted advertising (would even pay somewhat for this), but generally looking for alternative to Outlook. 
  


## Answer 29436

- posted by: [Craig Saboe](https://stackexchange.com/users/-1/12715-craig-saboe) on 2011-08-30
- score: 0

To expand on Autopulated's answer, you first need a mail server that supports IMAP. Unlike POP, which was once the more popular option, IMAP is a communications protocol that syncs the server's mail store to the client. POP simply lets you pull down what's on the server, and doesn't sync anything; deleting a message on your client doesn't affect the server, and many servers are set to delete emails once they are retrieved. All your clients, be they desktop, laptop, or BlackBerry, can use IMAP to communicate with the server and manipulate the email store there - marking as read, moving to a folder, etc. When you jump from client to client, whatever you do on one will then be reflected on the others when you let them sync with the IMAP server.

You need to check on each client how to configure an account, but pretty much all of them give you the option between POP or IMAP when you set one up. You then can configure options like whether you want your client to sync every message on the server, only certain folders, etc. These settings are just for your client, though, which means your desktop can pull EVERYTHING while your memory-constrained BlackBerry only pulls your inbox.

Thunderbird, Outlook, Windows Live Mail all support doing IMAP, and if you're using Gmail as your email host, you can use the web client as well. As far as servers, Gmail will do so once you enable it in the Options section, and Exchange will do so too - pretty much all of them will support IMAP.

For sending email, there's no difference - you still use SMTP, and most email clients will hold an email you write in your Outbox until a connection is available. And when you create an account in most clients, it will ask you for the default SMTP server to use, which should be part of the information you get when you set up your email system.  They should allow you to set other account-specific options as well, like different signatures.

The gist is that most servers you could use will support IMAP, and consulting the docs should tell you how to set it up as well as the settings to configure clients. Those settings can just be entered into most email clients you might want to use on pretty much any platform, desktop or mobile, and setting each one up will allow you to manipulate your email store however you wish. If you want recommendations for an email server, you should Google around or create a separate question with your individual needs. Hope this helps, and respond with any questions you have!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
