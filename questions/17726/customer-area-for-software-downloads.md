## Customer Area for Software Downloads

- posted by: [Paul](https://stackexchange.com/users/-1/5940-paul) on 2010-12-12
- tagged: `crm`
- score: 3

We are selling software licenses and would like to allow our customers to login to our server with a username and password, and download their license keys, installers etc.

Are there any PHP/MySQ tools out there?

P.S. We can not use FTP accounts, non-technies have real problems with anything other than their browsers :(

Thanks, Paul.



## Answer 17728

- posted by: [Steve Hanov](https://stackexchange.com/users/-1/1958-steve-hanov) on 2010-12-12
- score: 4

I use HTTP authentication for this, because it only takes a few minutes to set up. Send the customer a URL, username and password, and the users have no problem entering it into their browser.

Are you aware that browsers can use FTP? Use an URL like ftp://myserver.com/myfile.zip or you can include the username and password as ftp://username:password@myserver.com/myfile.zip

But it gets cumbersome with more than a few orders at a time, and I will be moving to a PHP system soon, once I get a few minutes to write one.


## Answer 17727

- posted by: [Elie](https://stackexchange.com/users/-1/1752-elie) on 2010-12-12
- score: 0

Should be pretty straight-forward to set up a basic eCommerce site with something like Drupal with Ubercart (if you want them to be able to buy it online without any direct interaction with someone from your company), or just plain Drupal if the purchasing itself is done offline. 

I know a company that has set up pretty much this exact type of site before, so if you need someone to build it, get in touch with me.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
