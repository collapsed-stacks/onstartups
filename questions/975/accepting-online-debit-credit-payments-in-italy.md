## Accepting online debit/credit payments in Italy

- posted by: [friism](https://stackexchange.com/users/-1/573-friism) on 2009-10-12
- tagged: `credit-cards`, `payments`
- score: 2

According to Wikipedia, accepting online credit card payments is possible in Italy
<http://en.wikipedia.org/wiki/Debit_card#Italy>. Anyone have experience implementing such a solution? Who has a good, low-cost solution with a good API?

I realise other options are Amazon FPS, Google Checkout and perhaps VISA International (and I would love to hear your feedback on those), but we are really looking for a low-overhead, "familiar" and local solution.


## Answer 1979

- posted by: [Cameron McGrane](https://stackexchange.com/users/-1/1010-cameron-mcgrane) on 2009-10-20
- score: 1

If you are finding it difficult to implement a merchant account in Italy I would re-think what you are trying to do. Mobile payments are exploding in Italy and aligning with this market behavior could be an alternative strategy to consider.

http://www.tmcnet.com/usubmit/2009/09/25/4390419.htm


## Answer 4421

- posted by: [Henry the Hengineer](https://stackexchange.com/users/-1/1692-henry-the-hengineer) on 2009-12-01
- score: 1

<p>Take a look at <a href="http://www.planetauthorize.com/" rel="nofollow">PlanetAuthorize</a>. They offer an API and have a module for vtigerCRM (I learned about them through vtiger). I haven't tried them yet, but it's another option for you.</p>



## Answer 4728

- posted by: [Olivier Lalonde](https://stackexchange.com/users/-1/1030-olivier-lalonde) on 2009-12-07
- score: 1

<p>I believe <a href="http://www.paypal.com" rel="nofollow">Paypal</a> works fine in Italy. </p>



## Answer 9162

- posted by: [Dario Solera](https://stackexchange.com/users/-1/1539-dario-solera) on 2010-03-12
- score: 1

<p>We're based in Italy, and we accept payments via PayPal with no problems. If you want to handle payments directly via credit/debit cards, the most used service is provided by <a href="http://www.sella.it" rel="nofollow">Banca Sella</a>, which was the fist bank in Italy to support online payments, so it's very well-known. I'm not sure how/if they accept foreign customers however, nor have we ever needed their services, so I have no idea about their rates.</p>

<p>My personal opinion is that PayPal is the most trusted payment solution, but that really depends on your audience.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
