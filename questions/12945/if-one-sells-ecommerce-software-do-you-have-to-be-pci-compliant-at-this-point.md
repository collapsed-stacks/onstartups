## If one sells ecommerce software, do you HAVE to be PCI compliant at this point?

- posted by: [UnStartup](https://stackexchange.com/users/-1/2189-unstartup) on 2010-07-21
- tagged: `ecommerce`, `software`
- score: 3

If one sells ecommerce software, do you HAVE to be PCI compliant at this point?

I read it costs upwards of 40K to get your ecomm software PCI compliant.

And some of the requirements have things like source code review, which means that your company is larger than 1.

Any thoughts on this?

I guess this industry is locked from 1-man operations?


## Answer 12948

- posted by: [John Bogrand](https://stackexchange.com/users/-1/3577-john-bogrand) on 2010-07-21
- score: 2

Per the document on PCI DSS first line is about software developed for off the shelf sales.  The answer is yes.  
https://www.pcisecuritystandards.org/pdfs/pci_pa_dss.pdf 

http://en.wikipedia.org/wiki/PA-DSS


## Answer 12955

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2010-07-21
- score: 0

It's strongly recommended and sometimes needed.  One key to becoming PCI compliant is not storing credit card numbers, something you want to avoid anyway.





## Answer 12970

- posted by: [thesp0nge](https://stackexchange.com/users/-1/627-thesp0nge) on 2010-07-22
- score: 0

<p>I think you've to be PCI compliant only if you store credit card numbers, in other cases (if you let third party app to manage them) maybe you just want to run penetration test or code reviews just to be safe against crackers break-in.</p>

<p>Remember to check out <a href="http://www.owasp.org" rel="nofollow">Owasp</a> material about how to write safe code. You can use also great <a href="http://www.owasp.org/index.php/Category%3aOWASP_Enterprise_Security_API" rel="nofollow">ESAPI</a> project from Owasp to embed security in you app with great library provided by security specialists. from all around the world.</p>

<p>However being PCI compliant is always a plus but maybe you want to reach the compliance by gentle migration.</p>

<p>Feel free to ask me more details about both penetration test than code reviews.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
