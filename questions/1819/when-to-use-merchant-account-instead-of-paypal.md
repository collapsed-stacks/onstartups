## When to use merchant account instead of PayPal?

- posted by: [Oleg Kokorin](https://stackexchange.com/users/-1/968-oleg-kokorin) on 2009-10-18
- tagged: `payments`
- score: 19

I wonder when it makes more sense to open a merchant account and use a payment gateway instead of old plain PayPal option? This should depend on the revenue processed, because merchant account has higher setup costs, but lower operating costs. What is the breakeven figure for revenue? Are there any other factors to consider?
 




## Answer 2969

- posted by: [dlynton](https://stackexchange.com/users/-1/482-dlynton) on 2009-11-03
- score: 17

Unless I missed something, no one here has mentioned PayPal Pro. It's just like a merchant account - you get a virtual terminal and API to charge cards *as your company name*. Customers never know PayPal is involved. It costs $30/month and the transaction fees range from 1.9% to 2.9% + $0.30 USD. See https://www.paypal.com/cgi-bin/webscr?cmd=_wp-pro-overview-outside.

In my experience, PayPal Pro is the most cost-effective option for a merchant account, unless you're charging high volumes and can negotiate low fees with your merchant provider.

Most merchant companies will force you into a 2-3 year contract with high cancellation fees. You might pay as much as 5-6% on business cards. Monthly fees could exceed $70. Cardservice Int'l, the company I was using, charged $20/month just for a "customer service" fee.

My opinion, don't get a merchant account until you're making a lot of money, or unless you have problems with PayPal holding funds (I've never had that problem). And in some cases, PayPal Pro won't accept you. I think you need to collect your funds somewhere on your website (in a store or some other payment form). It's definitely the best value.


## Answer 1843

- posted by: [Ade Olonoh](https://stackexchange.com/users/-1/317-ade-olonoh) on 2009-10-18
- score: 9

<p>Generally speaking, if your customers are going to be paying with personal finances, I recommend sticking with PayPal.  People are more apt to trust putting their credit card info into PayPal than your startup, and it's a pretty familiar process for many.</p>

<p>However, if you're targeting businesses, then I would highly recommend just going with a merchant account.  Businesses where more than one person has purchasing power usually have multiple credit cards, but rarely have a good solution for sharing PayPal accounts.  Paying from a PayPal balance can be a hassle from an accounting perspective as well.  Businesses still have to trust you, but if it's a business-oriented product you probably already have to build their trust for them to rely on you for part of business operation (versus something consumer-oriented like a game).</p>

<p>This was a few years ago, but when I launched <a href="http://www.formspring.com" rel="nofollow">FormSpring</a>, it was PayPal-only, and I received <em>frequent</em> complaints from businesses about the hassles of paying via PayPal.  We switched completely to credit billing via merchant account, and it's been extremely rare that someone's wanted to pay via PayPal (almost all were individuals outside the US).</p>



## Answer 1840

- posted by: [Chris W. Rea](https://stackexchange.com/users/-1/953-chris-w-rea) on 2009-10-18
- score: 8

Here's another factor to consider:

After you open a merchant account, you *should keep PayPal as a payment option*.  Many people are familiar with PayPal and are comfortable having PayPal as intermediary.  I often use PayPal even when a credit card is an option because **I don't like to give out my credit card number if I can avoid it.**

Part of making it easy for your customers to do business with you is offering multiple methods of payment, so your customer can choose what fits their preferences.  Consider, even though most credit cards insulate customers from fraudulent charges, many customers still like to guard their credit card numbers when going online.  For that reason alone, PayPal remains a useful option.


## Answer 2044

- posted by: [2_ghosts](https://stackexchange.com/users/-1/337-2-ghosts) on 2009-10-20
- score: 7

The thing I like the most about handing the customer off to PayPal for payment is that if they are not an existing PayPal member, the default option is for a credit card payment with *an option* to create a PayPal account. The page they land on has the full credit card payment form right there.

If it were the opposite and they had to click through a PayPal solicitation in order to get to the CC form, I think that would be a deal-breaker for me.

Other factors: 

- The fact that I don't have to take their CC on my site is a win in my particular case. PCI compliance on a site I am responsible for is one of those things that would keep me awake at night.

- The (relative) simplicity of dealing with one entity for payment processing.

Disclaimer: We haven't actually launched our shop yet (going live within a month or so), so take my words with a large grain of salt. If PayPal Standard turns out to be the wrong choice for some reason, I will absolutely switch us over to a traditional merchant account & payment gateway solution.




## Answer 1837

- posted by: [Yakov Fain](https://stackexchange.com/users/-1/691-yakov-fain) on 2009-10-18
- score: 6

The other advantage of using Paypal in online payment processing is that you don't need to worry about developing and adding a secure HTTP payment page to your application. Paypal has it, and if the customer CC number get stolen or there is any other security-related issue - Paypal is liable, not your application.

Paypal invested millions into providing secure payment infrustructure, and it's fair for them charging asking additional processing fees for this. 



## Answer 2876

- posted by: [Joel Spolsky](https://stackexchange.com/users/-1/4335-joel-spolsky) on 2009-10-31
- score: 5

PayPal is too closely associated with ebay in most consumers' minds. It makes a site seem amateur. It is appropriate for friendly companies selling $1.99 applications to add colorful frames around family photos. If you want to seem more professional than that, get a real merchant account.


## Answer 1853

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2009-10-18
- score: 3

All of the other answers give some points to consider, but **why not just use both?** 

Personally, I can't stand PayPal and avoid using it whenever possible. Honestly... I will spend more on a competing product/service just to avoid it. I would much rather give you, an unknown merchant, my credit card number (zero liability, etc).

A merchant account isn't that expensive, especially if you have the volume. I think our minimum fee is $15 and Authorize.Net charges like $12 or something. I suggest getting a few quotes, and then seeing if you can swallow the monthy fees.


## Answer 1823

- posted by: [Neil Davidson](https://stackexchange.com/users/-1/210-neil-davidson) on 2009-10-18
- score: 1

Like you say, it will depend on the fixed and operating costs (which will differ depending on your operating costs). Should be fairly easy to model in Excel.

Don't forget about the extra time and hassle involved in setting up a merchant account too. You'll also need a separate merchant account for Amex. Depending on how much history you've got, your bank might want some sort of deposit or personal guarantee.


## Answer 2045

- posted by: [Winfield](https://stackexchange.com/users/-1/1020-winfield) on 2009-10-20
- score: 1

I would echo the advice of Ade/BasicallyMoney above.

There's been good description of the technical implications of using your own Merchant account and processor vs. PayPal, but the cost in bureaucratic paperwork and hoop-jumping has been largely overlooked.  

I saw the establishment of a Merchant account with a bank as a small web startup turn into a laborious and long delayed process that ended up taking almost 2 months.

Also, although PayPal charges higher fees, it's a much more simple fee structure than the complex or convoluted rules you may encounter with a traditional merchant account across all of the different credit card account types.  If accurately predicting/tracking fees is important, this can be a complex process.


## Answer 1859

- posted by: [Rick Montgomery](https://stackexchange.com/users/-1/974-rick-montgomery) on 2009-10-18
- score: 0

All the answers here have some merit. However I am a Merchant Services provider for small to medium sized businesses. I am also an entreprenuer with other business enterprises so I see both sides of the coin. Fact is a Merchant account is relatively inexpensive compared to paypal. Our company MCCS can set you up with a Virtual Terminal fully encripted and PCI Compliant for about $50.00. Monthly charges are about $20.00 including gateway like Authorize.net. Per transaction charges are 2.29% + $0.35. Paypal has $0 set up but its $30.00 per month and 3.10% +$0.45. So by going with paypal you could spend more in the first 2-3 months than it would cost to go with a merchant account. All systems MUST be PCI -DSS (Payment Card Industry - Data Security Standards)compliant by February 2010. No processing company is setting up anything that is not compliant, so no worries with security. But the fact still remains, if a hacker wants in they will find a way no matter if your paypal or anyone. just ask Heartland Payment Systems they got hacked in 2008 millions of cards were compromised.
The other thing is YOU DO NOT have to go through your bank for a merchant account. You can set that up with any company you want. Banks get a cut of the profits so you can save money by going with an independent ISO for a processing company such as myself (little plug!). Never sign a contract locking you into a 2-3 year term, nor any termination fee. Over 40% of your Gross Revenue will come by way of credit card and the fee expense is a direct hit to your profit margin. Set up with a good reputable merchant account you will be much more efficient and profitable. Email me at rick.mccswi@yahoo.com and I will be glad to help you out!


## Answer 2875

- posted by: [pbreit](https://stackexchange.com/users/-1/239-pbreit) on 2009-10-31
- score: 0

Your decision should be *very* customer driven and less cost or security driven. If you are a brand new business, customers may be more comfortable paying with PayPal but if you are more established, PayPal may make you look less professional. PayPal is the best for multi-currency. There's not going to be a major cost difference, especially if you start out with only Visa/MC on a merchant account.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
