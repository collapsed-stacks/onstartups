## Software Sales & License Billing for Small Startup

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-01-10
- tagged: `management`, `license`
- score: 9

I have just started a small software startup and one of my current headaches is the management of licenses that we sell / lease...

I am looking for a system that can manage the billing and contact details for each license - 

i.e. 
what version of a product a customer is on,
how we bill them
when their software maintenance contract expires,


Can anyone recommend a product that can assist in managing this?


## Answer 18776

- posted by: [Wyatt O'Day](https://stackexchange.com/users/-1/5714-wyatt-o-day) on 2011-01-10
- score: 7

<p>There are a few ways you can do this. I'll talk about 2.</p>

<h2>Method 1: Buy a professional license management product</h2>

<p>I'm the founder of the company that makes <strong><a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a></strong>, which can be best described as hassle-free licensing &amp; online activation. You can <a href="http://wyday.com/limelm/help/license-features/" rel="nofollow">associate customer data directly with the licenses</a>. For instance, for a particular product key you can add the customer's email, contact info, and when the license is no longer valid (or when they need to renew). Use the <a href="http://wyday.com/limelm/help/api/" rel="nofollow">LimeLM web API</a> to generate the product key (adding the data), get when a license expires, and update the data when they renew their license (or however you're selling licenses).</p>

<p>That is, you can automate the entire purchase process. Of course you can still manage things manually, but my guess is you're trying to make the licensing, renewal, and purchasing all automated.</p>

<p>This is a solution for people just starting out or looking for a better licensing system. However, from the tone of your post it sounds like you've got a licensing system already. This brings me to the second option:</p>

<h2>Method 2: Create a simple database table</h2>

<p>This method assumes you have some programming skill and perhaps even a touch of database experience. It's easy enough to pick up -- Google can fill you in on what's not immediately obvious.</p>

<p>The first step is to create a table that will store your product keys. Below I have a simple example table that will keep track of 5 main things:</p>

<ol>
<li>The product key (pkey)</li>
<li>When the product key was created (ts_created)</li>
<li>The email of the user (email)</li>
<li>The full name of the customer (name)</li>
<li>And when the product key expires (ts_pkey_expires)</li>
</ol>

<p>Obviously you can expand the table to keep track of more info. But this is a good template to start from:</p>

<pre><code>create table pkeys (
    pkey_id          serial         not null,
    pkey             char(34)       not null,
    ts_created       datetime       not null,
    email            varchar(320),
    name             text,
    ts_pkey_expires  datetime,

    primary key (pkey_id)
) type = InnoDB CHARACTER SET utf8 COLLATE utf8_general_ci;
</code></pre>

<p>After you've got the database table up and running you can write a few SQL queries to insert, search, and update the fields in the table.</p>

<h2>Which method to choose?</h2>

<p>It's a tradeoff. I personally recommend you go with a professional licensing solution, because it's far easier. But if you're anxious to start learning SQL then I'd recommend you try method 2.</p>

<p>I can only speak for my company's product, but using <a href="http://wyday.com/limelm/" rel="nofollow">LimeLM</a> to automate this whole process is truly simple. We have full integration examples both on the client side (C, C#, VB.NET, Delphi, Java, etc.) and the server side (ASP.NET, PHP, etc.). Plus we genuinely care about simplifying our customers lives -- if you need any help getting the integration up and running we will help you out.</p>

<p>We have a <a href="http://wyday.com/limelm/signup/" rel="nofollow"><strong>free plan</strong></a> if you want to kick the tires and see if LimeLM lives up to my hype.</p>

<p>Tell me if this helps.</p>



## Answer 18774

- posted by: [faB](https://stackexchange.com/users/-1/6486-fab) on 2011-01-10
- score: 1

Have a look at [thinkvitamin.com 's Business Category](http://thinkvitamin.com/category/business/). In particular [Recurring Billing for Web Apps](http://thinkvitamin.com/code/reoccurring-billing-for-web-apps/) lists several Billing Systems and Payment Gateways, with pros and cons.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
