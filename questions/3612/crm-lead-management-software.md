## CRM / lead management software?

- posted by: [Joseph Turian](https://stackexchange.com/users/-1/423-joseph-turian) on 2009-11-13
- tagged: `software`, `sales`, `recommendations`, `crm`, `productivity`
- score: 11

Can anyone recommend CRM / lead management software?

We have a bunch of customer leads, and managing them using a Google doc is getting unwieldy.
We are looking for an inexpensive solution, preferably one with data portability.
We are a team of three.

SalesForce and Highrise look good (Salesforce seems slightly expensive) but I have not used them.

vTiger and SugarCMS appear to be the leading open-source. [edit: FatFree CRM seems like a good option, no one has discussed it yet.]

Does anyone have experience with CRM software for a team of three?


## Answer 6307

- posted by: [Kendall Miller](https://stackexchange.com/users/-1/2210-kendall-miller) on 2010-01-11
- score: 6

<p>We originally used Salesforce but found it unwieldy for a small team.  In addition, we balked that you have to upgrade to the Enterprise Edition ($125/user/month) to access the API for application integration.  In our view, this says that Salesforce.com is simply NOT targeting small software ISVs. </p>

<p><strong>We switched from SalesForce over to Highrise several months ago</strong> and have been very happy with it.  API integration is included in all editions.  If only one member of your team is working leads, you can get by with the $29/month solo edition.  But for only $49/month you can have up to 15 users.  You might also consider the $24/month Basic version, but beware that this limits you to just 10 deals – for us this was a “deal-breaker”.</p>

<p>One of the things we really like about HighRise is that it integrates well with a couple other tools we’re using.  <strong>Check out <a href="http://www.getleadspy.com" rel="nofollow">LeadSpy</a> for web site tracking</strong> – it integrates easily with your web site provides a unique view of the funnel from web traffic -> leads -> revenue.  </p>

<p>For example, you can use the Highrise API to create new contacts when a customer subscribes to your site.  LeadSpy will notice them filling in the subscription form and later notice that the email address entered on the form matches a record in Highrise.  With no effort on your part, LeadSpy will automatically provide a link to that Highrise contact (as well as a link to any associated deal) when you’re reviewing traffic in LeadSpy.</p>

<p><strong>Don't underestimate the value of this tracking to growing your business</strong>:  We can tell how someone initially found out about our site (from one of our ads, from an email we sent or someone else sent, etc.) and then track their activity through multiple trips to our site and ultimately whether they achieve any of the key goals we have (like downloading our evaluation, looking at our pricing, etc.).  This has helped us make key adjustments to what we do without spending a great deal of time on elaborate A/B testing and other techniques.</p>

<p>The best part for us with LeadSpy is that it took no programming considerations on our site to make that work - so we spent our web site development time on the core capabilities we needed without having to set aside time to develop specific sales support capabilities.</p>



## Answer 4203

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2009-11-27
- score: 4

vTigerCRM and SugarCRM both have data portability. They are capable of importing/exporting .CSV files so you can migrate your accounts from Excel to them and back. The import process requires renaming the fields or adding new fields to match the headers/category names in your Excel sheets.

I installed them on my laptop for testing first before migrating them to my server. I'd recommend doing the same to see if they're workable for you.



Below is a comparison of specific features from my experience (caution: Involves lingo!):

*vTigerCRM default package*

Pros: Field-specific editing function, Invoice PDF generator - generate invoices directly from a customer account, Free module addons, Can easily merge duplicate accounts.

Cons: The module editor is clunky and doesn't let you rename variables, Smaller development community

*SugarCRM default package*

Pros: Easier to use module editor, Larger development community

Cons: Can't edit fields individually -- you have to click on "edit" and modify all fields at once, Addons aren't free, merging duplicate accounts is a hassle.



Of the commercial providers, I've tried Highrise and Salesforce. Highrise is simpler to use but may not be able to import your existing customer accounts en masse. Salesforce looks good but the interface is a bit complex up front.




## Answer 3741

- posted by: [brianz](https://stackexchange.com/users/-1/1542-brianz) on 2009-11-17
- score: 3

<p>I'm working with a team of three right now...and we're bootstrapping so inexpensive is key.  Initially, we tried Salesforce since they had a $300/year for 3 seats deal going on.  However, I quickly learned that Salesforce's lower tiers are really just to get you hooked so you upgrade to their more powerful and full-featured versions.  I gather SF is great for larger companies with more money, but for us, it was extremely limiting.</p>

<p>We've just switched to <a href="http://zoho.com" rel="nofollow">Zoho CRM</a> which has been great so far.  It's free for three users.  The only thing I've paid for to date is integration with our Google Apps email..but that's only $5/user/month.  IMO, the Zoho user interface is much better than Salesforce as well.</p>

<p>I'm also a huge fan of software as a service.  So, I'd suggest against desktop solutions.  They make sharing more complicated, and it's much harder to get at your data unless you're in front of your own computer.</p>



## Answer 4077

- posted by: [Guillaume Justier](https://stackexchange.com/users/-1/1636-guillaume-justier) on 2009-11-24
- score: 2

We used to use vtiger but we found it to be really buggy, so we switch to SugarCRM which was the same under the hood.

One aspect to consider with opensource solutions is whether you have the skills to modify the system to match your needs: We are a web development company so the reason we went for an open source solution is because we knew we could:

 1. Fix problems ourselves.
 2. Develop the features we needed.

I have to say if we hadn't had the skills, I probably would have went with a more commercial solution, probably salesforce (although I agree with @brianz that their game is to upsell to the more expensive package). ZohoCRM might indeed be a good compromise between free and Salesforce.




## Answer 3613

- posted by: [Tall Jeff](https://stackexchange.com/users/-1/957-tall-jeff) on 2009-11-14
- score: 1

We use SalesForce.com for a staff of about 20 people accessing the system. It does depend to some extent on exactly how you are using the system, but in general it works really well. 

I agree it is expensive, but they have a good solution and are top dog in this space for a reason. They also have a customer support solution (support force) that can handle that piece of the equation as well in an integrated manner.


## Answer 4071

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-11-24
- score: 1

We are bootstrapping too, and the free version of Highrise has been working great for us. As we start bringing in revenue, we'll switch over to a higher (paid) plan of Highrise. I highly recommend that software, mainly to keep track of customer calls and leads.


## Answer 5107

- posted by: [Sachin Agarwal](https://stackexchange.com/users/-1/1784-sachin-agarwal) on 2009-12-15
- score: 1

<p>We've looked at a number of options, but every time we think about switching, we stay with BatchBlue's <a href="http://www.batchblue.com/" rel="nofollow">BatchBook</a> offering.  Has an iPhone app, and it seems to be well supported by and work well with other web-based services.</p>



## Answer 3688

- posted by: [Ahmet Kirtok](https://stackexchange.com/users/-1/1528-ahmet-kirtok) on 2009-11-16
- score: 0

I have heard pretty good things about InfustionSoft.

I haven't personally used it, but it looks like a pretty good solution for CRM+Lead Management+Email Marketing.

It might do the job for you.


## Answer 3732

- posted by: [Lyndsey Ferguson](https://stackexchange.com/users/-1/1549-lyndsey-ferguson) on 2009-11-17
- score: 0

<p>I've heard some good things about the free, Open Source <a href="http://www.sugarcrm.com/crm/" rel="nofollow" title="SugarCRM">SugarCRM</a></p>



## Answer 3735

- posted by: [Hector Sosa Jr](https://stackexchange.com/users/-1/10218-hector-sosa-jr) on 2009-11-17
- score: 0

<p>Have you looked at desktop solutions?</p>

<p>Both <a href="http://www.act.com/" rel="nofollow">ACT!</a> and [Maximizer][2] have been rewritten to take advantage of new technologies. They are both very good, and have tightly integrated features. I have supported both of them in the past. I personally prefer Maximizer.</p>

<p>The other three that I hear bandied about are [Contact Plus][3], [GoldMine][4], and [RightNow][5]. My first contact with CRM systems was Contact Plus many years ago. A lot of small businesses use that one, even though it looks dated.</p>



## Answer 4067

- posted by: [Giancarlo Corzo](https://stackexchange.com/users/-1/1606-giancarlo-corzo) on 2009-11-24
- score: 0

In my company we have used both sugarCRM and vTiger, vTiger has almost every package that you will have to pay for in sugarCRM.

I think it's the cheapest solution because you can download it and install it in your hosting or get a vTiger hosting instead (only 1 pay for the hosting and installation - 0 for support).

As usual when you evaluate software you should always list what you need and what the software provides.


## Answer 14092

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-09-15
- score: 0

I have Tradepoint and we have problems. Very scary and wish we could give it back.  


## Answer 23675

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-04-19
- score: 0

I would just like to state for anyone out there that I have used Tradepoint 360 and I would NEVER recommend it to anyone. My opinion is that the product is full of bugs, there are features we based our purchase on that appear in the software but don't actually work, and they really don't care when you complain. We have gone back to our old accounting system as Tradepoint 360 made a complete disaster out of our books and I really don't feel their developers have enough Accounting knowledge to make it work properly. Their support is horrible as they insist on communicating by email even if you have requested 10 times to speak with someone on the phone and when you submit a support request, you may not get answered for days. Imagine not being able to issue a credit to your customer for a week because of a bug you are waiting to be fixed. Imagine all your employees loosing access to the system for hours because of a mistake they made when releasing an update. I have a mile long list of critical issues. Anything that actually works properly in the system now is because we debugged it. I regret ever getting involved with this company and I only hope that I can stop others from making the same mistake.


## Answer 26135

- posted by: [Mike](https://stackexchange.com/users/-1/9699-mike) on 2011-06-09
- score: 0

<p>Our company went through the same phase and bounced around between Salesforce, SugarCRM, vTiger, Maximizer Enterprise, Zoho CRM, and Highrise. All will probably meet your needs (and beyond), but there are other factors to consider when picking a solution that will grow with you in the long term. We decided on Highrise for the reasons mentioned below.</p>

<p><strong>Cost, of course, is always an issue,</strong> and you'll want to consider a solution that will scale well without adding on a bunch of costs for every employee you add. Salesforce, for example, charges on a per user basis, whereas Highrise includes a number of users within a packaged fee.</p>

<p><strong>Another important consideration is integration</strong>. Choosing a more niche solution like FatFree CRM may limit you in the future when exploring other web-based tools to help make your business more efficient. For example, you might want to consider an online quoting system such as Socket (Full disclosure: I am affiliated with Socket ) to automate lead collection, an <a href="http://www.freshbooks.com" rel="nofollow" title="invoicing system">invoicing system such as Freshbooks</a>, or a <a href="http://www.zendesk.com" rel="nofollow" title="help desk system">help desk such as Zendesk</a>. The more popular CRM systems like Salesforce and Highrise have integration with a plethora of web-based tools out there (including the aforementioned). If you choose a more niche CRM system such as FatFree, you may be somewhat limited in choices for other time saving web-based software that plays well.</p>

<p><strong>Lastly, you'll want to consider support</strong>. I haven't had much experience with Salesforce, but Highrise really prides themselves on their support. They're a smaller company and that really is their competitive advantage IMO. vTiger or SugarCRM might be free, but to get any support, you'll have to pay consulting fees.</p>



## Answer 32001

- posted by: [Veronica](https://stackexchange.com/users/-1/13945-veronica) on 2011-10-28
- score: 0

<p>A good, scalable solution for tracking leads at a very reasonable price is <a href="http://www.apollohq.com/" rel="nofollow">Apollo</a>. Less focused on sales, it's a good blend of project and contact management. I believe that if you don't have a critical mass (lots of salespeople, thousands of customers, need for integration with other services) it does not make sense to adopt a full-featured CRM.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
