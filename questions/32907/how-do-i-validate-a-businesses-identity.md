## How do I validate a businesses identity?

- posted by: [Paul Riker](https://stackexchange.com/users/-1/14597-paul-riker) on 2011-11-23
- tagged: `business-services`, `validation`
- score: 0

I'm developing a website that allows businesses to register. Any ideas how to automate the validation process of the business? For example, to identify an individual you could use a credit card (not 100% accurate but close).


## Answer 35166

- posted by: [Sean Moubry](https://stackexchange.com/users/-1/15912-sean-moubry) on 2012-01-23
- score: 1

<p>You're just going to have to take their word for it, or check manually, because there's no good way to automate this.</p>

<p>Here is a list of every country/state/province's business registry websites, which is the best way to <strong>manually</strong> verify a company exists:</p>

<p><a href="http://en.wikipedia.org/wiki/List_of_company_registers#United_States" rel="nofollow">http://en.wikipedia.org/wiki/List_of_company_registers</a></p>

<p>I received so much spam after starting my business, I figured there <em>must</em> be some kind of API that spammers are using to get business information, but I've been unable to find such a service. I suspect the information is being scraped from the websites listed in the link above.</p>

<p>Interesting: The USPS has an <a href="http://www.ups.com/content/us/en/bussol/browse/online_tools_us_address_validation.html" rel="nofollow">Address Validation API</a>. Which, admittedly, doesn't really solve your problem either, but might be tangentially helpful.</p>



## Answer 35174

- posted by: [pdjota](https://stackexchange.com/users/-1/1355-pdjota) on 2012-01-24
- score: 0

An additional approach could be to check information against an information provider such as 
Experian services [1], for instance you could query the credit ranking score and credit summary or something similar.

I have experience with integration with credit card check services and those integrate easily with standard protocols (we used SOAP). Once a customer is connected to our site, we do a background check against Experian database to prevent fraud.

You might contact them for additional information on your specific needs from a business.

[1]Example of Business check, you can freely check if the company is registered http://sbcr.experian.com/main.aspx?link=5502


## Answer 35176

- posted by: [Muthu](https://stackexchange.com/users/-1/13073-muthu) on 2012-01-24
- score: 0

1. Check the land line telephone number with the provider. Generally land line telephones cannot be transferred easily where as mobile phones can.
2. A private detective agency might be helpful as well but may be a little expensive



## Answer 35177

- posted by: [JeffS](https://stackexchange.com/users/-1/15873-jeffs) on 2012-01-24
- score: 0

Something that we have considered doing is verifying the essential business information, such as address with the state that they are doing business in, and then send them a physical letter with an online verification code. 

It takes a small amount of human interaction, and costs about $1 for the letter, but that cost is worth it to us.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
