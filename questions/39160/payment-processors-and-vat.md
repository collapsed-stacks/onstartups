## Payment processors and VAT

- posted by: [Paul Stovell](https://stackexchange.com/users/-1/13821-paul-stovell) on 2012-05-17
- tagged: `payments`, `vat`
- score: 4

I'm trying to understand how VAT responsibilities are handled by payment processors like FastSpring and SWReg. [From the HMRC website][1]:

> **What is VAT?**   
> VAT is a tax that's charged on most business transactions
> in the UK. Businesses add VAT to the price they charge when they
> provide goods and services to: 
> 
> - business customers - **for example a
> *clothing manufacturer* adds VAT to the prices they charge a *clothes
> shop***
> - non-business customers - members of the public or 'consumers' -
> for example a hairdressing salon includes VAT in the prices they
> charge members of the public

I create software, so I am a "software manufacturer" like the clothes manufacturer above. I use a payment processor like FastSpring to handle purchases. The payment processor normally collects VAT from the end customer. 

But doesn't the payment processor simply play the role of "retailer" in this example? As a wholesaler, am I not also responsible for charging VAT to the retailer? Should I send the payment processor an invoice with VAT due on every sale they make? 

If at the end of the year, if I've collected millions in sales and haven't collected a cent worth of VAT, isn't that going to look awfully strange to HMRC? 

How is the ISV/payment processor relationship any different to the clothes manufacturer and the clothes store above? 

  [1]: http://www.hmrc.gov.uk/vat/start/introduction.htm


## Answer 39179

- posted by: [Marnix van Valen](https://stackexchange.com/users/-1/13831-marnix-van-valen) on 2012-05-18
- score: 4

<p>I run a business in the Netherlands so I can't comment on the exact rules in the UK, but I can comment on the more general issue based on EU regulation. I have implemented an order processing system for an ISV in the past so I learned a thing or two on this subject.</p>

<p>The rules you've quoted apply mostly to <em>domestic</em> transactions. Once your business transactions go across borders, things work a little different.</p>

<p>As a general rule when you're a business and you sell something you have to apply VAT on your bill.</p>

<p>You'll then have to forward all the VAT you've collected to your local tax agency. However, as a business you don't have to pay VAT. So you get to deduct any VAT you've already payed to other companies from the VAT you have collected. The remainder is what you pay to your local tax agency.</p>

<p>That's the basic rules for doing business within your country.</p>

<p>When doing business internationally, different rules apply because VAT is a tax that applies to consumption of goods and services <em>within the territory of a tax agency</em> (usually a country). If you can prove you have bought something in say the UK but you'll be using it in another territory (the US for example), you don't have to pay VAT in the UK. This is what enables <a href="http://www.schiphol.nl/Travellers/ShopRelax/Shopping2/BenefitsServices/DutyfreeAndVAT.htm" rel="nofollow">duty free shopping at airports</a>.</p>

<p>So if you do business with companies or 'consumers' in non-EU countries, you don't apply VAT on the bill.</p>

<p>However when doing business with customers outside the UK but within the EU the same basic rules apply as for domestic transactions. Since companies in the EU don't have to pay VAT themselves a business client can reclaim any VAT you charge them from your tax agency (ie HMRC).</p>

<p>I think you can see this becoming a problem fast with bureaucracy being what it is. Imagine you're doing business with companies in several different EU countries and you have to reclaim taxes in each one individually. Your money will be stuck in those other countries for a while as the tax agencies review your claim.</p>

<p>To alleviate that administrative burden and financial risk, you are not required to apply VAT to invoices you send to EU business customers. Your tax agency will ask you for information how much turnover you've made on EU customers so they can collect the VAT from other EU member states directly.</p>

<p>You are however required to verify that the VAT number the customer gives you is indeed valid and belongs to the company you are doing business with. If you don't and it turns out your customer was not a proper business you are liable for the amount of VAT that wasn't invoiced.</p>

<p>This is why your tax agency requires you to maintain a proper financial administration so they can trace the (virtual) flow of VAT. The easiest thing to do is to make sure your invoices have your customer's VAT number on them.</p>

<p>So what does that mean for your business? Well if you only do international business, it's perfectly OK to collect no VAT at all. If you have the evidence to back that up there's nothing to worry about. You may even get money back for the VAT you payed to local suppliers.</p>

<p>The same rules apply to your resellers and payment providers. However, the VAT they collect is their business and irrelevant to you because it's a matter between your reseller and their local tax agency.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
