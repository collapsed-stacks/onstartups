## Is there a service I can use for cheque mailing?

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-07-16
- tagged: `payments`, `affiliate`, `webservices`
- score: 3

I am keeping track of commissions earned by my customers in a database. Each month, I have the amount they earned and their Names and Addresses.

I can easily automate the generation of the lists of people and how much to send. What I don't know is an easy way to send the cheques out to these people.

Is there a way for me to automate this, to minimize my time involved? 

If one exists, I'd be happy to use a service and send them one list each month if they would send out cheques in the amount I specify to each person, with my business listed as the payer.

---

Additional info: 

I want this system to require nothing from the user. They don't need to sign up. They don't need to provide any authorization or bank account number. They don't need to have a specific account type, such as PayPal.

What would be idea would be an online service that somehow just gets money to them without mailing costs, maybe like wiring money. I don't mind paying a service charge, even a few dollars 
per payment. 

Is there such a beast?



## Answer 15135

- posted by: [Tauren](https://stackexchange.com/users/-1/4561-tauren) on 2010-10-15
- score: 3

<p>I'm in the market for this exact same thing. I asked a <a href="http://stackoverflow.com/questions/3004023/api-based-solutions-for-sending-payments-to-people-without-bank-accounts-closed">similar question on SO</a>, but had it closed.</p>

<p>Since then I've found a possible solution called <a href="http://batchex.com/" rel="nofollow">BatchEx</a>, but don't know how trustworthy it is. A while back I attempted to contact them, and got a response, but it was many days later, so it didn't leave a great impression. I haven't followed up yet.</p>

<p>I also found <a href="http://webmasterchecks.com/" rel="nofollow">WebmasterChecks</a>, but know nothing more about them yet besides what is on their site.</p>

<p>There are also these API mailing solutions, but it doesn't look like they will mail checks:</p>

<ul>
<li><a href="http://www.postful.com/" rel="nofollow">http://www.postful.com/</a></li>
<li><a href="http://www.postalmethods.com/" rel="nofollow">http://www.postalmethods.com/</a></li>
</ul>

<p>The lack of this type of service shocks me, and it seems there must be a solution out there for all of these affiliate marketing systems. Makes me think I should investigate the market some to see if such a solution would be a worthwhile venture.</p>

<p>If you learn more about any services, I'd love to hear about your experiences! Please share pricing information, reliability, and so forth with me.</p>

<hr>

<p>UPDATE:</p>

<p>I had a conference call with several specialists at my bank today (US Bank, usbank.com) and spoke in great lengths about doing ACH transactions. We also touched on the possibility of mailing checks. It sounds like they do have a service for this, but they did not know all the details and are researching it more.  </p>

<p>What they did tell me is the following.</p>

<ul>
<li>US Bank does have a check printing service</li>
<li>Can send payment information in a batch file via FTP (maybe SFTP and HTTPS as well)</li>
<li>Can issue checks from any number of my own accounts, but not sure if there is a per account surcharge</li>
<li>Checks must come from a US Bank account</li>
<li>Unsure if they can issue checks from another organization's checking account number</li>
<li>Fairly expensive</li>
<li>$1250 setup fee</li>
<li>$0.20 - $0.47 per check depending on quantity</li>
<li>Minimum of $175 per month (will cost $175 for the first 373 checks)</li>
<li>Unclear on if there are other costs, such as postage fees</li>
<li>$12/transmission (per batch file)</li>
</ul>

<p>I started looking into all this last June, so it has taken me months to even find out that my bank offers such a service. I would check with your bank and other banks you would like to work with and see what you can find. They might have something similar.</p>

<p>Good luck!
Tauren</p>



## Answer 15184

- posted by: [Benjamin Chambers](https://stackexchange.com/users/-1/4835-benjamin-chambers) on 2010-10-16
- score: 2

Ask your local bank.  I guarantee they can provide the service for you.

Alternatively, buy blank checks, and print them yourself.  Most professional accounting software will do so.  Again, check with your bank about what types of checks to order.

Alter-alternatively, hire a payroll service.  Many banks provide this as well.  So do many accountants.  For that matter, if you're growing (congratulations!) to the point where it's a hassle to be sending out so many checks, maybe you should consider hiring an accountant and/or payroll service at this point anyway.



## Answer 15370

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2010-10-21
- score: 1

Bank of America provides free check mailing to third parties via its Bill Pay system. All you need is a name and address to send the check to. You could get someone to write a script to fill in the BoA form automatically. Recurring payments can be scheduled in advance. Not sure if there's some API that can be used to integrate with a website, but you might want to ask them.


## Answer 13608

- posted by: [abenetis](https://stackexchange.com/users/-1/3397-abenetis) on 2010-08-23
- score: 0

you could use PayPal or similar services to pay your customers. They allow mass payments, so you could take your list and pay all customers with just one payment.

Well, they are only sending money to your customers email-address. However, if you have international customers, the above mentioned solution will make it easier for you. Furthermore, you don't need to worry if a cheque might get lost.

Otherwise you need to search for a solution provided for your Country, as accepting cheque payments may vary from country to country

Hope this helps.


## Answer 15202

- posted by: [lkessler](https://stackexchange.com/users/-1/1491-lkessler) on 2010-10-17
- score: 0

<p>After searching a long time, I think I found a better way. </p>

<p>Cheques involve something physical, and mailing and handling costs are an unneeded expense. In addition, cashing the cheque can sometimes involve a bank charge for the recipient (something I don't want) if it is not in their currency.</p>

<p>But there are some online ways to transfer money. The one I like the best is HyperWallet at: <a href="http://www.hyperwallet.com" rel="nofollow">www.hyperwallet.com</a>. They create an online "wallet" where the person in the other country can get the money and deposit it into their bank.</p>

<p>Charge is only 1.00 (or less) per transaction if you decide to pay sender's cash out fee, which you should. That is much more convenient and much cheaper than the $2.50 or more it will cost to send a cheque.</p>

<p>HyperWallet is a Canadian company and has direct connections to Canadian banks and credit unions. Since I am in Canada, it is a no-brainer for me.</p>

<p>When I get to the point of using them for this, I'll try to remember and come back here and add my experiences.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
