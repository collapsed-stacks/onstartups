## How can I prepare an invoice from the command line?

- posted by: [Steve Hanov](https://stackexchange.com/users/-1/1958-steve-hanov) on 2009-12-18
- tagged: `business-process`
- score: 2

Making invoices in Openoffice, and saving as a PDF file is annoying and taking too long. Is there any command-line software for Linux that can generate a high quality PDF invoice? 


## Answer 5245

- posted by: [Jarie Bolander](https://stackexchange.com/users/-1/585-jarie-bolander) on 2009-12-18
- score: 2

<p>Check out <a href="http://www.latex-project.org/" rel="nofollow">LaTeX</a>. It has a command line interface and I think can read Open Documents but I am not sure about that.</p>



## Answer 5259

- posted by: [Jason](https://stackexchange.com/users/-1/2-jason) on 2009-12-18
- score: 1

<p>If you don't mind writing a little code, you could use <a href="http://FreshBooks.com" rel="nofollow">FreshBooks</a> as your invoicing system, and then use their (very simple!) API to create invoices and/or download them in PDF format.</p>

<p>The nice thing about this solution is that you also have a great non-automated system for dealing with invoices.</p>



## Answer 5238

- posted by: [Matt](https://stackexchange.com/users/-1/1653-matt) on 2009-12-18
- score: 0

I don't think this can make invoices from command line, but it's a good tool to know about: http://www.gnucash.org/


## Answer 5250

- posted by: [Dane](https://stackexchange.com/users/-1/1441-dane) on 2009-12-18
- score: 0

<p>This might be a question you want to post on <a href="http://stackoverflow.com/" rel="nofollow">StackOverflow</a> which is more programming oriented and they might have better idea of how you could do this.</p>



## Answer 5653

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-30
- score: 0

<p>I would recommend you to use <a href="http://www.invoicera.com" rel="nofollow">Invoicera</a>, it is an easy to use Invoice billing application with so many advanced features like Invoice scheduling, multiple currency support, multiple payment gateways support and time &amp; expense tracking management. You can easily create high quality PDF invoices and send those PDF invoices to your clients in attachment.</p>



## Answer 6672

- posted by: [Steve Hanov](https://stackexchange.com/users/-1/1958-steve-hanov) on 2010-01-17
- score: 0

I ended up using my own solution. I create the invoice as an RTF or other openoffice file. Then, using a custom script, I replace certain keywords in it.

The <a href="http://linux.die.net/man/1/unoconv">unoconv</a> utility can convert any openoffice file to PDF.




## Answer 9938

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-04-07
- score: 0

I use http://bambooinvoice.org/. Its free, easy to use and can integrate with your emailing system.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
