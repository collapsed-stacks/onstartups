## Does an iPhone app need PCI compliance?

- posted by: [Ryan Michela](https://stackexchange.com/users/-1/16937-ryan-michela) on 2012-03-16
- tagged: `iphone`, `credit-cards`
- score: 0

I want to write an iPhone app that provides a common ordering interface for a number of disparate sites that do not have an ordering API. To ensure I can rapidly adapt to any changes in each site's ordering process without having to release a new version of the iPhone app, I need to build a service that serves as an ordering proxy.

The ordering proxy does not directly process credit card transactions. It only passes the transactions on to the various sites. To avoid keeping any credit card details on the central server, I want to have the iPhone app securely store the user's credit card data for future use.

 - Does an iPhone app that stores and submits credit card data need to be PCI compliant?
 - Does a server that forwards credit card details to another site, but doesn't process any transactions itself need to be PCI compliant?
 - Since I am not a merchant and don't directly deal with banks or credit card companies, does PCI even apply to me? Can I be fined even though I have no agreement with any banks, payment gateways, or credit card companies?




## Answer 37267

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-03-17
- score: 1

You have multiple questions here so lets address them one by one.

1. Does an iPhone app that stores and submits credit card data need to be PCI compliant?

Provided you (the app developer) are not a credit card processor and have no dealings with any credit card companies, then the answer is basically no. More on this later.

2. Does a server that forwards credit card details to another site, but doesn't process any transactions itself need to be PCI compliant?

If it did then every router, edge server, caching server etc on the internet would need to be PCI compliant. A server that merely passes traffic and does not store data is not covered ***provided*** it is not owned or controlled by a company that needs to be PCI compliant. So for example Amazon servers that take credit card data need to be compliant but the local ISP that services the end user does not.

3. Since I am not a merchant and don't directly deal with banks or credit card companies, does PCI even apply to me? Can I be fined even though I have no agreement with any banks, payment gateways, or credit card companies?

Once again, the answer is basically no.

**Now the proviso:** If you allow the user to store his credit card data on the phone using your app you are basically like a program that allows a user to store his passwords locally (on an iPhone, PC , Mac whatever). There is an expectation on the part of the consumer that you will do so in a responsible and secure fashion following industry best practices. If your application ever gets hacked or it can be shown that sensitive credit card data fell into the wrong hands because of a bug in your program you can expect some major lawsuits. Proceed cautiously and with full disclosure so that people can't claim later that they had no idea that you were storing their credit card data.

Further you would be well advised to insure that your iPhone app uses encryption and security at least as good as what PCI would require.

As a way of understanding the logic here, merchants are precluded from writing credit card numbers and names down on a piece of paper ant tacking it to the wall of their office. PCI is designed to insure merchants do the right thing. The is nothing however making it illegal for a consumer from doing something stupid like writing his credit card number on a post-it note and sticking it on his computer at work. You are not a merchant, and are not providing software for merchants. You are more like the company that sells pens and post-it notes to consumers.  


## Answer 37584

- posted by: [Joe Schumacher](https://stackexchange.com/users/-1/17172-joe-schumacher) on 2012-03-26
- score: 1


Definition by PCI Security Standards Council (SSC)<br>

 - For the purposes of the PCI DSS, **a merchant is defined as any entity that accepts payment cards bearing the logos of any of the five members of PCI SSC** (American Express, Discover, JCB, MasterCard or Visa) as payment for goods and/or services. Note that a merchant that accepts payment cards as payment for goods and/or services can also be a service provider, if the services sold result in storing, processing, or transmitting cardholder data on behalf of other merchants or service providers. For example, an ISP is a merchant that accepts payment cards for monthly billing, but also is a service provider if it hosts merchants as customers.
<br><br>
If you are developing applications to accept credit cards for processing (so your app connects to a service provider for processing) which you plan on selling to other merchants then your application must pass PA-DSS. If you are developing an application for internal use only then you are still required to complete PCI DSS. 
<br><br>
I would recommend you check out PCI Security Standards web site and look to see the level of compliance you must show based on their various requirements.  I recommend that you use the words of store and submit carefully as these words can change your requirements for PCI.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
