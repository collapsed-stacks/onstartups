## How to let customers download software automatically after payment through a website?

- posted by: [user6492](https://stackexchange.com/users/-1/6492-user6492) on 2011-01-14
- tagged: `website`, `software`, `selling`
- score: 7

I have a company that will be selling software online, and I'd like for customers to be able to pay online and then just click on a "Download Now" button and download the software automatically, without me or someone else from the company having to email the software program to the person.

Is there a site or device that I could use to do this?

Thank you!


## Answer 18966

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-01-14
- score: 6

<p>This is a good question, but I think you shouldn't limit the download of your app.</p>

<h2>Why you shouldn't limit the download of your app</h2>

<p>The reason you shouldn't limit the download of your app is that if you <em>do</em> you'll increase the amount of stolen credit cards being used to purchase your program. Thieves will be thieves. Limiting your app to "paying" customers won't stop a thief from buying 5000 stolen credit cards for $10 and running through the list until they get one that works.</p>

<p>If you have the download readily available then it will be fly paper for the thieves; they'll try to steal your app through normal reverse engineering means. You'll get less orders from stolen credit cards, thus you'll save money on the inevitable chargebacks once the victim realized they've had their credit card number stolen. Plus, hiding your software behind a private link is a hassle for legit users. Don't piss off your customers.</p>

<p>If you're keeping the download link private for renewal purposes (e.g. they can only update for a year), then you're better off solving this with licensing. The way you can do it in <a href="http://wyday.com/limelm/" rel="nofollow"><strong>LimeLM</strong></a> is by using custom license features -- we have a <a href="http://wyday.com/limelm/help/saas-and-time-limited-licensing/" rel="nofollow">full example that shows how to limit updates via licensing</a>.</p>

<h2>How to deliver product keys to your users</h2>

<p>Delivering the product to your user (whether a download location or a product key) is dependent on a couple of factors:</p>

<ol>
<li>The licensing you use</li>
<li>The payment platform you use</li>
</ol>

<p>Most payment providers have ways of calling a script on your website to let you know a sale has been made. For example, using <a href="https://www.paypal.com/ipn" rel="nofollow">PayPal's IPN (Instant Payment Notification)</a> can call a script on your website and from that script you can generate a serial then send your new customer an email with the product download site and serial number.</p>

<p>We actually have a full PayPal payment example written for PHP and ASP.NET (C# and VB.NET) that automates the entire process. It uses the PayPal IPN alongside our <a href="http://wyday.com/limelm/help/api/" rel="nofollow">LimeLM web API</a> to process the order, generate the product key on the fly, then email the user. So a user can start using the fully registered version of your software seconds after their order is processed.</p>

<p>If you update your question with the payment platform you use then we can point you to the right API or example code to use.</p>

<p>Lastly, if you're determined to keep your installer to customers only (even despite my advice not to), then you can do it with a simple script. Just pass the new customer's product key as a parameter to a script. For example: <a href="http://example.com/latest-installer.php?pkey=ABCD-EFGH-IJKL-MNOP-QRSTU" rel="nofollow">http://example.com/latest-installer.php?pkey=ABCD-EFGH-IJKL-MNOP-QRSTU</a></p>

<p><strong>Here's an ASP.NET C# snippet of what the script would look like:</strong></p>

<pre><code>//TODO: verify the product key is valid, if not show an error and bail out

//if the pkey is valid, deliver the latest installer:
Response.Clear();

// download the file and bail
Response.AddHeader("Content-Description", "File Transfer");
Response.ContentType = "application/octet-stream";
Response.AddHeader("Content-Disposition", "attachment; filename=" + Path.GetFileName(installerFile));
Response.AddHeader("Content-Transfer-Encoding", "binary");
Response.AddHeader("Expires", "0");
Response.AddHeader("Cache-Control", "must-revalidate, post-check=0, pre-check=0");
Response.AddHeader("Pragma", "public");
Response.AddHeader("Content-Length", new FileInfo(installerFile).Length.ToString());

// output the file
Response.WriteFile(installerFile);

Response.End();
</code></pre>

<p><strong>Here's what the same snippet would look like in PHP:</strong></p>

<pre><code>//TODO: verify the product key is valid, if not show an error and bail out

//if the pkey is valid, deliver the latest installer:
header('Content-Description: File Transfer');
header('Content-Type: application/octet-stream');
header('Content-Disposition: attachment; filename='.$installerFilename.';');
header('Content-Transfer-Encoding: binary');
header('Expires: 0');
header('Cache-Control: must-revalidate, post-check=0, pre-check=0');
header('Pragma: public');
header('Content-Length: ' . filesize($installerFullPath));
ob_clean();
flush();
readfile($installerFullPath);
exit;
</code></pre>



## Answer 18951

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2011-01-14
- score: 1

There are companies that provide this service; sorry I can't personally recommend any beyond a Google search.

You can ask the question on Stackoverflow.com to get technical expertise.

Your software can require a key that you provide in an email without sending the entire app.

You can create a hidden page on your site with the download link. 

Ideally, you send an email with a GUID that is a parameter on a page that has to be verified with the client record. After the client connects to this page, you can set a flag on the record that prevents them from accessing this page again.

If someone can download a file and install on their computer, what is to prevent them from giving the file to someone else for free? EReader uses the credit card number of the buyer to register a book. Not too many people would want to give this out to people they want to use the software for free.


## Answer 18953

- posted by: [TimJ](https://stackexchange.com/users/-1/1172-timj) on 2011-01-14
- score: 1

There are plenty of licensing services and products that will do this.  You can also write your own - I made a PayPal payment interface script that did exactly what you are asking about.  

I would not recommend writing your own though - it is a hassle and there are better things to spend your time and efforts on.


## Answer 18959

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-14
- score: 1

<p>I automatized the process with <a href="http://www.plimus.com" rel="nofollow">Plimus</a> in our of my companies.</p>

<p>I used a custom solution in the past, but only because I got high volume in transaction, and I was able to save <strong>a lot</strong> in transaction costs. Don't do it unless you have at least 20K a month in revenues.</p>

<p>There are many others such as <a href="http://www.swreg.org" rel="nofollow">SWReg</a>, <a href="http://www.Shareit.com" rel="nofollow">ShareIt</a> or <a href="http://www.regsoft.com" rel="nofollow">RegSoft</a>.</p>

<p>Check <a href="http://www.regmatch.com/comparison/refund/" rel="nofollow">this page</a> for a comparison.</p>



## Answer 19986

- posted by: [Natalie](https://stackexchange.com/users/-1/7195-natalie) on 2011-02-09
- score: 1

<p>I would recommend <a href="http://www.payproglobal.com/" rel="nofollow">PayPro</a>, an end-to-end eCommerce solution that is optimized to sell software online.  PayPro offers a variety of payment options for online shoppers. Your order pages can be completely customized to match your website design and make customers feel confident while purchasing. Confirmation emails can be also customized and include a link to download a product – it is sent automatically after purchase is successfully completed. PayPro provides a reliable fraud detection system preventing fraudulent orders without impeding valid orders. They have friendly and very responsive support for vendors and shoppers. </p>



## Answer 18952

- posted by: [Alex - Aotea Studios](https://stackexchange.com/users/-1/1744-alex-aotea-studios) on 2011-01-14
- score: 0

<p>I use <a href="http://getdpd.com" rel="nofollow">DPD</a>. They provide functionality to deliver activation keys so will be suitable for software. </p>

<p><a href="http://e-junkie.com" rel="nofollow">E-junkie</a> is a popular option but I had a problem with getting discounts working with them, and their user interface is subpar.</p>



## Answer 18976

- posted by: [Scott](https://stackexchange.com/users/-1/6594-scott) on 2011-01-14
- score: 0

I have  a simple technique that we use for secure PDFs.  You put the file in a directory that is not browse-able from the general internet traffic.  You then grant your web app permission to pull the file and then resend the file to the browser.  If they are not authenticated the way you want, they can't reach that download. 

Of course, I think some sort of "key system" where one download can only be installed X times might also be helpful.  


## Answer 19061

- posted by: [Dave](https://stackexchange.com/users/-1/6628-dave) on 2011-01-17
- score: 0

If you try to secure the download, how can you stop duplication. My answer was to limit the licence. Let them copy the software all they want, but lock down the usage. I used the rainbow technologies dongle. The updates were simple and unfettered while the licence was tied to the hardware.


## Answer 51945

- posted by: [Mooba](https://stackexchange.com/users/-1/29848-mooba) on 2013-11-29
- score: 0

<p>For years I have been using the free version of Locked Area (locked-area.com) for this purpose.</p>

<p>All you have to do is download the Locked Area files.</p>

<p>Follow the instructions they provide for setting everything up.</p>

<p>You will set up files in cgi_bin, and also create a members directory in your public_html.</p>

<p>Once you follow all the steps and install Locked Area it will automatically password protect your members directory, and you will have a registration link.</p>

<p>This registration link is what is sent to your customers after they make a purchase.</p>

<p>It is a registration form where they create a username and password so they can enter your protected members area.</p>

<p>The members area is where you have your download.</p>

<p>No one can enter that area unless they create a username and password through your registration form.</p>

<p>You can rename the registration form file to something else so people won't be able to guess it.</p>

<p>As people buy your download and create the username and password their email address is added to your Locked Area Admin panel so if you ever have to send out mass emails, then you can email just one email from within your Locked Area Admin panel and it will be sent to all your customers automatically.</p>

<p>Just be sure to follow the instructions on how to get all setup, and you can customize your registration form etc. from within your Locked Area Admin panel etc.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
