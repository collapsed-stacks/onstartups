## Web Based or Desktop application for managing your licenses / serial numbers?

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-10-27
- tagged: `license`
- score: 8

I am planning on using a third party component/software for managing the serial number /licenses for my software. I have two options for the third party applications; a web based application that I can use to generate and manage my serial numbers or a desktop application that I can install on my PC and use it to generate and manage serial numbers locally on my laptop or PC.

The advantage with the web based app is that I can manage the serial numbers almost from anywhere where I have a web access. With the desktop software, I have to travel with my laptop or have a remote access to my PC to manage the serial numbers.

What is your experience with this? 
Is any one using web based apps for managing their serial numbers?
Any suggestions comments? 

Thanks,

Jambo


## Answer 16395

- posted by: [Prateek Mishra](https://stackexchange.com/users/-1/5208-prateek-mishra) on 2010-11-12
- score: 5

<p>I have used all of the following apps in the past while working with different companies as a freelancer. Never had a problem with anyone. You should check them out.</p>

<ul>
<li><p><a href="http://productkeymanager.codeplex.com/">Product Key Manager</a> - Still in Beta</p></li>
<li><p><a href="http://www.x-formation.com/lm-x_license_manager/index.html">LM-X License Manager</a> - Easy to use with great functionality</p></li>
<li><p><a href="http://licmax.com/concepts.html">Limax</a> - Great for small apps</p></li>
</ul>

<p>I hope that it was helpful.</p>



## Answer 16476

- posted by: [Adrian Schneider](https://stackexchange.com/users/-1/4434-adrian-schneider) on 2010-11-14
- score: 2

I've used KeePass (desktop app) with a few web companies in the past.  If high security isn't a huge concern, I've had great success just using Google Docs spreadsheets for passwords.  It's super convenient and is easy to share with others.


## Answer 17244

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2010-11-30
- score: 2

<p>I'm the founder of the company that makes <strong><a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a></strong>. We have an online product key manager. But you can also use the web API to generate product keys during your order process. We have full example code in PHP and ASP.NET (C# and VB.NET) showing how to use our web API.</p>

<p>Also, the licensing protection that integrates with your app works with all languages (C, C++, C#, VB, Delphi, Java, etc., etc.). Plus it has no external dependencies.</p>

<p>We <strong><a href="http://wyday.com/limelm/signup/" rel="nofollow">have a free plan</a></strong> (no credit card needed) if you just want to kick the tires and see if it's right for you. Also, we publicly list our prices -- no need to haggle with annoying salesman.</p>



## Answer 15699

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2010-10-27
- score: 1

For my prior project I wrote my own serial number generator, database and management tool first as a command line interface, then migrated it to a server with a web front end.  Users could request numbers and get the numbers they were issued and I could control/query it all via the web.

There were a couple reasons I migrated it:

- I was not always able to get to the desktop machine when I needed to when there was a request or issue with a serial number.
- I was able to allow OEMs to do serial number management and sell licenses using the one web system.  This was a great help to me in offloading some sales and marketing.  

I would not think of doing a non-web solution, though of course it presents security issues that a desktop solution does not have.  

I would likely find an off the shelf or hire someone else if I had to do it again.  My licensing scheme was not that sophisticated but it was effective enough.

It was a simple mySQL database with a few php scripts on a machine at the web hosting company.  It was integrated with my paypal purchase/checkout so that users automatically got a license/serial number after they purchased.  


## Answer 16397

- posted by: [Denys S.](https://stackexchange.com/users/-1/5299-denys-s) on 2010-11-12
- score: 1

<p>Even though I don't need to manage licences/serial No, I do have experience of developing a system which was doing exactly what you've described.</p>

<p>So as to if anyone is using web based apps for managing their serial numbers - yes, a lot of people, I guess. In particular system that I've developed is running through secure connection and is used by support specialist, sales managers and general managers (though rarely by the latter). And in the scenario of company, getting money from software sales, it is actually the kernel of everyday activity - if it goes down, support is down, managers are half productive, clients are disappointed, etc.</p>

<p>With world mowing toward SaaS products, web app is the best choice. I have no idea what terms you will get with a third party soft, but you can read more about SaaS <a href="http://en.wikipedia.org/wiki/Software_as_a_service" rel="nofollow">here</a>.</p>

<p>As to what <a href="http://answers.onstartups.com/questions/15698/web-based-or-desktop-application-for-managing-your-licenses-serial-numbers/15699#15699">Tim</a> said about: "it presents security issues that a desktop solution does not have". You need to take into account, that any solution <strong>has</strong> a security issue, if it doesn't it was never built.</p>

<p>So if I were you, I'd take a closer look at the web based option.</p>



## Answer 16401

- posted by: [newyuppie](https://stackexchange.com/users/-1/1961-newyuppie) on 2010-11-12
- score: 1

<p>You didn't mention what language you are programming in, but I've used <a href="http://www.infralution.com/licensing.html" rel="nofollow">Infralution Licensing System</a> before. It's a very powerful .NET component to generate and manage license information.</p>



## Answer 16534

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-11-15
- score: 1

<p>I was in the same case than you. After 4 years using desktop software, manual emails and even paper, I decided to write <a href="http://www.shopmvc.com" rel="nofollow">my own web based backend software</a> for this (and for other daily tasks done by a microISV). I'm a .Net guy so I have done it in asp.net MVC. License codes are now generated on my shop web site when a sale occurs. I can generate new ones from there (I purchased a 3rd party licensing engine), read, edit and delete them on the web.</p>



## Answer 16555

- posted by: [Nir](https://stackexchange.com/users/-1/4237-nir) on 2010-11-16
- score: 0

There's one important point nobody here mentioned, if you ever sell your product using an automatic system (user pays and automatically sent license code in e-mail) you have to have a web based system because the server processing the sales has to access the license key system to generate the new code.

BTW: I highly recommend setting up an automated system has soon as possible, the simple fact that every customer immediately and automatically gets the license code makes a huge difference from both a support perspective (you will get customers complaining they didn't get the code 5 minutes after the sale even if it's written in large bold font that it takes up to 24 hours) and from a peace of mind perspective (didn't check e-mail for 2 days? maybe didn't answer a few support e-mails on time but people only get really pissed off if they payed and don't get what you promised).




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
