## PCI compliance and Visa Third Party Agent requirements

- posted by: [Tauren](https://stackexchange.com/users/-1/4561-tauren) on 2011-04-20
- tagged: `legal`, `saas`, `hosting`
- score: 3

I own a web hosting company and maintain my own servers in a colocation facility. I do not resell the hosting services of another company. My new startup company is a SaaS provider that I'm hosting on my web hosting company's servers.

I'm working on getting PCI-DSS compliance right now for both businesses. I've been told by my merchant account provider that not only do I need to get PCI-DSS compliance for my web hosting company, but that I also am REQUIRED to register with Visa's Third Party Agent (TPA) program and pay the $5000 fee to register plus $2500 annually. And that doesn't include any sort of costs for compliance testing.

My webhosting company is small and would have a hard time with these fees. My other company is a startup and is barely making anything yet. I had thought I could submit a Self Assessment Questionnaire (SAQ) and avoid big fees, but if money like this is required, how do any small web hosting companies exist?

I understand that get PCI-DSS compliance is necessary. But is it true that registering for TPA is a *REQUIREMENT*? Or is it something I can do if I want to be listed on their list of compliant service providers? If I had customers insisting that I be listed at a TPA it would be one thing, but that isn't the case at this time. Can the merchant account provider require this? Is it up to them to decide if this is required, or is it mandated by some law?

Here's a snippet from the letter my merchant account provider sent to me:

> When looking at your account we
> noticed that you are providing a
> service(s) that is potentially
> applicable for registration with the
> Payment Brands, including Visa and
> MasterCard. Any merchant that
> transmits, processes, or stores
> cardholder data on server(s) that you
> own/manage/operate on behalf of (your
> clients)who are other merchant account
> holders, must meet the PCI Data
> Security Standard and follow
> additional steps to register as a
> service provider. **Applicable services
> commonly include webhosting, software
> as a service, or collecting payment on
> behalf of a client.**
>
> Any company
> providing these services must register
> with Visa’s Third Party Agent (TPA)
> program and MasterCard’s Data Storage
> Entity (DSE) program. 
>
> A Visa TPA is an
> entity that provides payment-related
> services, directly or indirectly, to a
> Visa client and/or stores, processes
> or transmits Visa account numbers:
> http://usa.visa.com/merchants/risk_management/cisp_service_providers.html.
> A great FAQ is available on the Visa
> website.  Please note that Visa does
> require an initial registration fee of
> $5000, with an annual renewal fee
> which is currently $2500. 
>
> A MasterCard
> DSE is an entity that engages, or
> proposes to engage, in the processing,
> transmission, or storage of account
> data, transaction data, or both on
> behalf of any merchant, Independent
> Sales Organization (ISO), or Third
> Party Processor (TPP) of the member:
> http://www.mastercard.com/us/sdp/serviceproviders/index.html.
> MasterCard does not currently collect
> registration fees unless the DSE
> provides services on behalf of a
> processor.




## Answer 23791

- posted by: [Mike](https://stackexchange.com/users/-1/9699-mike) on 2011-04-21
- score: 1

Great question. I'm thinking (hoping) it's the company providing the merchant services (ie your gateway processor/merchant account) that is required to register as a TPA. That said, this is an extremely oblique and confusing topic - tough to find simple definitive answers when reading Visa's agent FAQ (http://usa.visa.com/download/merchants/Agent_FAQ.pdf).

One resource that scares me a bit is http://blog.elementps.com/element_payment_solutions/mastercard/

> SaaS ISVs provide services that hosts the software that stores, processes, and/or transmits cardholder data on behalf of their merchant therefore they qualify as a TPA. 


Though it seems to speak of Mastercard... again... confusing.

I would also like to see someone with experience in the topic answer the question more definitively.


## Answer 24437

- posted by: [brettflorio](https://stackexchange.com/users/-1/10243-brettflorio) on 2011-05-05
- score: 1

<p>I can't speak to your new SaaS, but your hosting company would <em>not</em> need to register as a service provider. Nor would it need to be fully PCI compliant (by "fully" I mean with the SAQ D set of requirements) if you fully outsource the payment processing (meaning that your servers don't ever even touch cardholder data).</p>

<p>The key here is the difference between a merchant and a service provider. Your hosting company isn't a PCI compliant service provider, and you don't want it to be. Just because your users <em>could</em> upload osCommerce doesn't mean that you're required to be a PCI compliant service provider. You can check with any shared hosting provider out there and, at best, they'll say that you can be compliant for the SAQ A (which is "fully outsourced", like sending the customer to PayPal). PCI compliant hosting providers like Firehost or GSI are what's needed to host a PCI compliant application (like osCommerce or Magento or anything that actually <em>does</em> actually touch cardholder data). (Note that even most larger hosting providers aren't PCI compliant, and if they actually understand PCI they'll tell you. Rackspace's Cloud (at this point) isn't compliant, and they'll tell you.)</p>

<blockquote>
  <p>This means my CUSTOMERS could use the service to store or transmit credit card information. I can't monitor everything my customers do on my servers at all times. I understand and acknowledge that I need PCI certification to do this, but I'm unclear on if TPA/DSE is required.</p>
</blockquote>

<p>It's the responsibility of the individual merchant (your hosting customers) to ensure that they are using PCI compliant service providers (like you, for hosting). You're not compliant, so they can't host a compliant system with your hosting company.</p>

<p>As far as your SaaS goes, unless it's a service that actually handles transactions for your users, I think the same thing would apply. You'd be a merchant, not a service provider. And if you can outsource that payment processing to something like FoxyCart or Recurly you'd still (very likely) only need to do the SAQ A. Again, the act of hosting something for somebody doesn't necessitate PCI compliance as a service provider. It's only if you're hosting something like an e-commerce platform that you'd be a service provider. Check page 12 of the <a href="https://www.pcisecuritystandards.org/documents/pci_dss_saq_instr_guide_v2.0.pdf" rel="nofollow">PCI DSS Instruction Guide</a>.</p>

<blockquote>
  <p>MasterCard does not currently collect registration fees unless the DSE provides services on behalf of a processor.</p>
</blockquote>

<p>I don't know this for sure, but in the process of certifying with a large payment gateway we've been told that MasterCard <em>is</em> now charging the same $5k + $2500/yr ongoing that Visa is. I haven't confirmed this with MasterCard yet, but I wouldn't be so sure it's still free. EDIT: MasterCard's requirements are different, so you shouldn't have to worry about fees from their end.</p>

<p>To be very clear: What level of compliance you need depends on a lot of details we don't have, so it's up to you. But in general, just try to never touch credit cards at all and you won't have to worry about too much.</p>



## Answer 23747

- posted by: [Antony P.](https://stackexchange.com/users/-1/7812-antony-p) on 2011-04-21
- score: 0

I cannot answer directly to your question here but what a lot of startups od is to NOT "transmits, processes, or stores cardholder data on server(s)". If you have transactions outsource the process completely to Paypal or your bank and don't take this hurddle on you.. What if there is fraud and you become liable for all this.. I wouldn't even take the chance as a startup. I hope you are at least an LLC so you are yourself protected against liabilities..

I think you are asked and requirement all those fees because you are doing a business that requires them. Focus on your core, outsource the rest ;-)

I hope this helps.

Disclaimer: I'm not a lawyer, I'm not a CPA, anything I say is a personal opinion and could be plain wrong.. In fact I'm not sure I need this disclaimer at all but let's be cautious.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
