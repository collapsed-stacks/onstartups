## How to accept payments from companies in India?

- posted by: [romkyns](https://stackexchange.com/users/-1/5899-romkyns) on 2012-01-24
- tagged: `payments`, `india`
- score: 2

Our business accepts payments via credit cards (Google Checkout + PayPal) and also via PayPal directly. We've had several requests from companies in India, stating that they cannot pay with a credit card. So far none of them ended up paying via direct bank transfer either.

Is this a real difficulty that Indian companies are having, or could they perhaps be after our bank details for whatever reason? In the former case, what might be a good way to accept payments from such companies?

I really should have mentioned this: we're located in the UK. Sorry about that.


## Answer 35236

- posted by: [Anurag](https://stackexchange.com/users/-1/4475-anurag) on 2012-01-25
- score: 2

I run a company based out of India and receive/send payments across currencies and countries. Based on my experience these are the easiest routes to remit money from India

1. The easiest and probably the cheapest is Credit Card. I do not understand why companies are telling you that they cannot pay by credit card. Probably they do not have one, but its easy to get one from any bank in India for people with a decent credit history

2. Paypal works fine, though recurring payments might be an issue. There are certain Reserve Bank of India restrictions on Paypal also, but it should work fine when linked to a Rupee denominated Bank Account

3. Wire transfers to international banks work fine, especially if the Indian company has an account in an international bank. Your company name, account number and/or SWIFT/IBAN(Europe) code is required. This process is pretty swift and I have seen remittances in under 24 hours

So basically I do not see any reasons why an Indian company cannot pay you easily using these 3 approaches. If I were you, I would insist upon the company to work out one of these approaches else stop dealing with them.




## Answer 35201

- posted by: [Napolux](https://stackexchange.com/users/-1/9006-napolux) on 2012-01-24
- score: 1

What about moving to https://stripe.com/ ??? Could be an easy way to accept payments via credit card.


## Answer 35204

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2012-01-24
- score: 1

Assuming you are in the US, you can accept payment by wire transfer, or by check. 

For wire transfer, you need to supply your bank's SWIFT code and your account number. Note US banks charge to receive international wire transfers. Always ask your bank how much it will cost to receive this type of paymenbt before indicating you will accept payment this way. The price can vary from $10 to well over $100. You have to decide who pays for that. Also note there are still some banks in the US that do **not** have their own SWIFT code. Payment this way is not instantaneous, it can take 1 - 5 days for payment to go through. Also not, most banks will not tell you when payment is received- it's up to you to monitor your account. In the US, there are enough problems with this payment method to make it not all that useful for small businesses.

The other option is payment by check. Your customer must go to their bank and request a check, **payable in US dollars AND drawn on a US bank**. As harsh as this sounds, it is not that hard to do in virtually every country in the world. Your customer pays the fees to get the check, and it clears in the US with no fees. Generally, the fee to get a check of this kind is much less than the fee to wire transfer money to the US.



## Answer 37157

- posted by: [Gary Rowe](https://stackexchange.com/users/-1/5259-gary-rowe) on 2012-03-14
- score: 1

<p><strong>You could try Bitcoin</strong></p>

<p>The process would be as follows (and would be fully automatic through your website):</p>

<ol>
<li>Determine how much the Indian company owes you </li>
<li>Visit a Bitcoin exchange and determine the spot rate for BTC to INR</li>
<li>Quote them a BTC value (valid for say 20mins to avoid fluctuations) and provide a destination Bitcoin address</li>
<li>They make the payment using a free and open source <a href="http://multibit.org" rel="nofollow">Bitcoin client</a></li>
<li>You receive the money about 10 minutes after they send it and immediately cash out on the exchange to get your local currency (GBP)</li>
<li>You make a local bank transfer to your company account when it's convenient</li>
</ol>

<p>Bitcoin carries very low transaction fees (typically &lt;0.01 GBP for a 100 GBP transaction) and has <strong>no chargeback risk</strong>. No credit card or registration with anyone is required which may suit the Indian company's requirements. You don't have to reveal any bank account details or anything else that could jeopardise your security arrangements.</p>

<p>You can find out more at the <a href="http://bitcoin.org" rel="nofollow">main Bitcoin site</a> or see a <a href="http://lovebitcoins.org" rel="nofollow">less technical description</a>.</p>



## Answer 37655

- posted by: [Priyank](https://stackexchange.com/users/-1/17204-priyank) on 2012-03-28
- score: 1

The problem is not about technology or cost. 

If you are dealing with anyone who is not a senior person, that person may most likely not want to use his/her personal credit card for multiple reasons - apprehension about not being reimbursed on time by the company, having to go through lot of procedures to get reimbursed or misuse of credit card details. 

Though credit cards are common in India now, most people don't use them. They use a debit card instead. It's a culture thing. Using credit cards is subconsciously seen as taking a loan or as living beyond one's means. Even though it might not apply to this case, that is the reason most people don't use credit cards. 

Online bank transfers on the other hand are pretty common. Businesses freely share their Bank Account Numbers, IFSC, SWIFT codes etc. with concerned people. Since you can't withdraw money with these details, it is considered safe. This might be considered private information in US but here it is ok.

Bottomline: Do something to keep the employee's personal money out of the transaction.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
