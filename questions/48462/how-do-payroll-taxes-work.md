## How do payroll taxes work?

- posted by: [leeand00](https://stackexchange.com/users/-1/5549-leeand00) on 2013-04-08
- tagged: `tax`, `usa`, `payroll`
- score: 0

This may sound like a very naive question for a site on Startups, but...how do payroll taxes work?

From what I can tell from doing database work at a company they seem to consist of percentages of net pay deducted from net pay on a Federal, State, and Local level (with local being the most complex based on the geographic coordinates of a particular employees home and work addresses).

From what I understand they are also very complex and based on [Tax Tables, whether or not you're single or married, how often you get paid and how many allowances you claim][1].  

Also they change alot....

And I also understand that there are no [free web-services][2] that will simply allow a series of these inputs to return a percentage to be taxed or calculated deduction for payroll tax.  I think the lack of a free web-service like this prevents alot of people from opening new businesses that could potentially provide jobs.

So I'm intrigued....how do taxes work?  Give me an example of how I would take one employee, take his pay (gross pay? net pay?) and either research how to tax his/her pay  at the federal, state and local level?




  [1]: http://stackoverflow.com/questions/14782415/payroll-tax-database-schema-united-states
  [2]: http://programmers.stackexchange.com/questions/194327/web-service-for-pulling-up-to-date-payroll-tax-information/194328?noredirect=1#comment375507_194328


## Answer 48464

- posted by: [littleadv](https://stackexchange.com/users/-1/13808-littleadv) on 2013-04-08
- score: 3

<p>For small businesses there are third party providers that can do all the hard work for you at a relatively low price ($25/mo with Quickbooks, for example). It is definitely not something worth doing on your own.</p>

<p>Larger companies either work with third party providers (like ADP for example) or have their own accountants do that for them.</p>

<p>Generally there are several different payroll taxes, and they are managed differently.</p>

<ol>
<li><p>FICA taxes - certain percentage of pay, divided equally between the employee and the employer. You <strong>must</strong> withhold these.</p></li>
<li><p>FUTA taxes - only the employer pays them.</p></li>
<li><p>Workers' compensation insurance - only the employer carries this. In some states its a tax, in others a required insurance.</p></li>
<li><p>State disability taxes - state laws vary, but it is usually a percentage of the pay up to a limit, with employer or employee (or both) paying it, depending on the State.</p></li>
<li><p>Income taxes - employee pays it, but employer must withhold. For Federal tax, how much to withhold is determined by the information the employee provided on W4, and the tax tables and formulas IRS publishes (<a href="http://www.irs.gov/pub/irs-pdf/p15.pdf" rel="nofollow">publication 15</a>). For State/Local taxes - determined similarly using the relevant W4 equivalents and publications from the relevant authorities.</p></li>
</ol>

<p>Not remitting the payroll taxes correctly is a serious offence, and the corporate limitation of liability doesn't protect the responsible individuals. If you fail to remit the payroll taxes correctly - you will be prosecuted <strong>personally</strong>, together with other individuals responsible.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
