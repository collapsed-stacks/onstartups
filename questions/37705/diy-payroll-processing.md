## DIY Payroll Processing?

- posted by: [Michael Trausch](https://stackexchange.com/users/-1/5973-michael-trausch) on 2012-03-29
- tagged: `tax`, `getting-started`, `employees`, `payroll`, `employers`
- score: 5

I have tried (and been rejected by) a few online payroll solutions.  As I am about to start (very soon) working with real employees, I need to find a way to do payroll more or less manually (though I will eventually be automating the process—I am a programmer, after all).

My business is located in the State of Georgia, and to keep matters simple, for the time being, I am only going to hire employees in the State of Georgia.  While answers to this question with federal information are acceptable, those with answers that cover Georgia would be divine.

Insofar as federal requirements, I am aware of the following (for the 2012 year):

* The Corporation must pay 6.2% on top of an employee’s salary for social security tax for the first $110,100 of an employee’s salary.
* The Corporation must withhold 4.2% from the employee’s salary for the employee’s part of the SS tax for the first $110,100 of an employee’s salary.
* The Corporation must pay 1.45% on top of an employee’s salary for medicare tax.
* The Corporation must withhold 1.45% of an employee’s salary for medicare tax.
* The Corporation must pay 6.0% on top of the employee’s salary, for the first $7,000 of the employee’s salary, for FUTA.
* The Corporation must withhold Federal Income tax according to the tables and methods presented in [IRS Publication 15][0], [IRS Publication 15-A][1], and [IRS Publication 15-B][2].  I believe that I understand the tables sufficiently enough to write a function to compute this part of the withholding for an individual, but it seems to essentially amount to withholding up to 35%, depending on the bracket and whether certain IRS rules have been triggered.

So, to use an example of an employee that is making $20 per hour for 40 hours, is single, claims no withholding allowances, and is paid every two weeks, it would seem that:

* The Corporation pays 6.2% + 1.45% + 6.0% = 13.65% in taxes on top of the paycheck.  If the paycheck is $1,600, the amount to remit for the corporation’s part of federal payroll taxes is thus $218.40, correct?
* The Corporation withholds 4.2% + 1.45% for social security and medicare, thus $90.40.
* The Corporation withholds $187.15, plus 25% over $1,442, which works out to $226.65.

Therefore, for **federal only**, it seems that the corporation pays $218.40 of tax, while the employee pays $317.05 of tax.  Am I good so far?

Now the real confusion begins for me, for state processing.

With the State of Georgia, I have:

* Registered my Corporation.
* Registered with the Department of Revenue and received a withholding account number.

I have not:

* Figured out how to compute or remit state unemployment tax.
* Figured out how to compute or remit state workers’ compensation tax.
* Yet registered with the state for sales tax purposes, as I sell no taxable goods (I solely provide services; anything that I have to purchase for those services is submitted to my client for reimbursement, but the original vendor collects the sales tax, I do not).

I have a document that shows me the tax tables, and they are structured along the same lines as the Federal tables.  So for the situation above for GA it looks like I withhold $84.22 in state income tax.  Assuming that is correct, then I understand GA’s withholding requirement, at least there.

But I believe that I have to provide for other things, too: workers’ compensation, state unemployment tax... is there anything else?

And the $100,000 question: where do I go to find concrete information on this stuff?  For SUTA, I found the Georgia Department of Labor Web site for Employers, but I really don’t seem to be finding the information I need there.  Do I remit WC and SUTA along with other withholdings, in the same way as Federal?  Or do I have to do something special there?

Also, one other thing:  We do **not** run Microsoft Windows; we are a Linux shop.  Please do not suggest software unless it works directly on Linux systems without a virtual machine or emulator or Wine or similar.  Thanks for any help!

[0]: http://www.irs.gov/publications/p15/index.html
[1]: http://www.irs.gov/publications/p15a/index.html
[2]: http://www.irs.gov/publications/p15b/index.html


## Answer 37706

- posted by: [Karlson](https://stackexchange.com/users/-1/15252-karlson) on 2012-03-29
- score: 3

<p>I would strongly recommend that you look into payroll services companies like:</p>

<ul>
<li><a href="http://www.adp.com" rel="nofollow">ADP</a></li>
<li><a href="http://www.paycomonline.com/" rel="nofollow">PayComOnline</a></li>
<li><a href="http://www.payrollexpress.com/" rel="nofollow">Payroll Express</a></li>
<li><a href="http://www.irs.gov/efile/lists/0,,id=101120,00.html" rel="nofollow">And just for kicks the whole list of them from IRS</a> which includes several located in GA</li>
</ul>

<p>Or find an accounting firm that can do the payroll for you or talk to the bank where you have your account as most of them offer payroll services as well.  E.g. <a href="http://www.bankofamerica.com/small_business/online_banking_and_services/index.cfm?template=payroll_services" rel="nofollow">Bank Of America</a>.  Trying to find and do this on your own will cause you more grief then it's worth. </p>



## Answer 37707

- posted by: [Chris Fulmer](https://stackexchange.com/users/-1/17026-chris-fulmer) on 2012-03-29
- score: 3

So, first of all, get a copy of the Employer's Tax Guide (Publication 15 from the IRS).  That will point you to the frequency with which you have to make filings of withholding and employment taxes.  Also, look at the paperwork that came when you got your EIN -- it will tell you what federal forms you need to file, and when.

Secondly, Federal Unemployment Tax works hand-in-hand with State Unemployment.  If I recall correctly, the federal tax is reduced by amounts you pay into the state system.  Check with the Georgia Department of Labor about paying their unemployment -- see http://www.dol.state.ga.us/pdf/forms/dol4e.pdf .

Third, you asked about workers compensation.  Workers Compensation insurance is usually provided by private entities who you contract with, not by a state agency. 

There are a few other payroll issues that you haven't mentioned, which you may need to consider: (1) reporting -- you will need to issue form W-2s to your employees, (2) benefits -- these are sometimes reported on form W-2, (3) garnishments -- sometimes employees have their wages garnished by court order or administrative action.

If you're a one-person shop, dealing with your own payroll isn't a huge deal.  But, it gets substantially harder when you start adding people.  And that's why most people deal with a payroll service provider.


## Answer 37712

- posted by: [mhoran_psprep](https://stackexchange.com/users/-1/15626-mhoran-psprep) on 2012-03-29
- score: 1

<p>Talk to a very small business you know and ask what service they are using. If they are not using a service they may be able to give advice.</p>

<p>You are taking a risk by going forward without an expert. The deadlines and requirements are non-trivial, and if you mess them up their are penalties. </p>

<p>Talk to the <a href="http://www.georgiasbdc.org/" rel="nofollow">Georgia Small business development center</a> for other ideas.</p>



## Answer 37715

- posted by: [David Ogren](https://stackexchange.com/users/-1/16938-david-ogren) on 2012-03-29
- score: 0

You don't say why you were rejected. But my short answer is to not even consider DIY payroll processing. I know lots of people who have no employees other than themselves that still use online services for payroll. So, without some compelling reason that you would be rejected from all of them I can't see any reason to try and do this yourself.

The rules are just too complicated and variable and the penalties too severe to try and do this on your own. Remember that you aren't just going to have to write the checks to the employees and the government. You are also going to have to submit the W-2s and other tax forms.

This is the epitome of the kind of thing you need to outsource.


## Answer 37720

- posted by: [m7d](https://stackexchange.com/users/-1/17241-m7d) on 2012-03-29
- score: 0

You might consider the route I've taken with a couple corporations. Get ahold of PPC Payroll Deskbook (DVD or online) and a standalone payroll program. I suggest CFS 940/941 Payroll and their W-2/1099 program as well, taxtools.com. The other program that is very nice is by Pensoft (they have several different versions with increasingly more functionality). You only need one or the other. Both will keep you compliant with Fed and State forms given you also arm yourself with the knowledge a CPA possesses on this topic (via PPC Payroll Deskbook and Fed and State tax authority publications as others have cited above and below) and provide a nice organized way to fill things out and keep organized.  PPC Payroll Deskbook is an authoritative source, but be warned it does not cover state, just Federal. I choose to run payroll after-the-fact. Payroll is either done after-the-fact or live. Now that I think of it, a less expensive program, but one which does not handle Federal Form 944 is Medlin Payroll. Figuring out payroll was tough at first, but now I have the hang of it and am glad I took it back from the CPA. I have no affiliation with any of the companies mentioned. Lastly, if you get stuck and need some expert advice in a pinch, you can do as I've done in the past and use justanswer.com to ask a tax expert a question. Lots of CPAs hang out there. You have to know enough via a certain amount of study, a bit of a catch 22, to know if you're getting a good enough answer, but really, you should know anyway. You are responsible for payroll failures, regardless of whether a service is used. Some people don't realize that. The software I've suggested is Windoze only, but in this modern age we're all using VMs, right? Sure we are.


## Answer 39383

- posted by: [Dennis Tarrant](https://stackexchange.com/users/-1/18102-dennis-tarrant) on 2012-05-25
- score: 0

DIY payroll is a dangerous way to go. Not knowing why you are declined by payroll services, find a local accounting or bookkeeping firm that has experience handling payroll, tax-finings, W-2s, deductions, etc. I hope your comment about being a software developer doesn't mean you intend to write your own program!

What are you using for the General Ledger? Many have a payroll modual. In addition to the federal and  star taxes you list, many municipalities have payroll taxes. What about workers compensation insurance insurance, too? Not a payroll issue, but required when you have employees in Georgia and most other states. Be aware that there are strict federal and state laws regarding exempt and non-exempt employees. You cannot pay everyone a salary, most (all, at first) of your employees will be hourly. You  use have a way to track their hours (they sign the time sheets), even if they are exempt.

Do you see why DIY is not the best idea now? 

It gets more complicated when you add employees in other states



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
