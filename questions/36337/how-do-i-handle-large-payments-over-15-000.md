## How do I handle large payments (over $15,000)?

- posted by: [Andrew Burnett-Thompson](https://stackexchange.com/users/-1/15348-andrew-burnett-thompson) on 2012-02-18
- tagged: `payments`, `international`
- score: 6

As a side-project to my IT Consultancy business, I have developed a software product which I intend to sell. The URL for the new product is at http://www.scichart.com

I am partnering with [FastSpring][1] as a payment processor. They charge a reasonable rate and can process credit card payments / purchase orders worldwide. 

Now I've just noticed during testing that the limit for payments is $15,000. However, my product is priced between £499-£1249 ($750-$2000 USD) per license and I have a few clients interested in buying a site license. I am wondering how I can process large payments like this. 

What is the protocol? 

Should I just send them a paper invoice and a SWIFT/IBAN code to do an international bank transfer? 

FastSpring has recommended that I split orders into multiples if it goes over the limits. I'm unhappy about this as it looks unprofessional. 


  [1]: http://www.FastSpring.com


## Answer 36339

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-02-18
- score: 7

<p>There are a number of questions implied by your your single question above.</p>

<ol>
<li>First, while Fastspring is a great company <em>(we use them)</em>, <strong>why</strong> would you use them to process a PO? POs are something you can easily do yourself and in the process save yourself 8% of that $15,000! <a href="http://answers.onstartups.com/questions/9424/late-payment-policy-best-practices">See my answer here for how to process a PO.</a> People sending you a PO do not expect an instant credit-card style turn around of their order.</li>
<li>For payments over $15,000, how you receive the money depends on where you are and where your customers are. If you are outside the US and your customers are in the US, that SWIFT/IBAN code is going to cause you infinite headaches. Many US companies just are not set up to do SWIFT transfers. They would <strong>much</strong> prefer to send you a US check, which may cause problems for you.</li>
<li>How many companies have credit cards for software purchases with credit limits of over $15,000??? Many companies pay for software with a credit card, but those cards have <strong>low</strong> credit limits. This keeps employees from charging $15,000 for themselves!</li>
</ol>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
