## access to source code if the start up fails

- posted by: [noname](https://stackexchange.com/users/-1/798-noname) on 2010-03-25
- tagged: `risk`
- score: 8

I have begun developing packaged software for pharmaceutical manufacturers.
A BIG customer asked me "what if I install your software and your company is no more after 3 years?"
I am sure other packaged software companies go through this OR went through this.
What is the best way to mitigate this risk for the customer?



## Answer 9587

- posted by: [Gary E](https://stackexchange.com/users/-1/2587-gary-e) on 2010-03-25
- score: 11

<p>What you need is a <strong>software escrow service</strong>. You basically place your software package's source code with a neutral third party. This party will release the source code to your customer under certain specified conditions. <em>(One example might be your company goes bankrupt.)</em></p>

<p>There are hundreds of companies that provide this service. Here are just a few.</p>

<p><a href="http://digital.ironmountain.com/content/ipm_form_b?c1=GAW_SE_NW&amp;source=USA_IPM_B&amp;kw=software_escrow_phm&amp;cr5=3977607630&amp;gclid=CKe76PWo1KACFcrY5wod2DjXug" rel="nofollow">Iron Mountain</a></p>

<p><a href="http://www.escrowassociates.com/software-escrow.html?gclid=CJvmvIyp1KACFec35wodEz9EuQ" rel="nofollow">Escrow Associates</a></p>

<p><a href="http://www.escrowtech.com/software_escrow_lp1.php?cmp=gg-d-SE:02&amp;s_kwcid=TC|7858|software%20escrow||S||3827090711&amp;gclid=CJWQiMOp1KACFds45wodZghksw" rel="nofollow">Escrow Tech International</a></p>

<p>Typically you sign a contract that specifies under which conditions your software source code will be released to the other party. These services charge a <strong>fee</strong>. You typically have the big company, that is worried about what happens if you vanish, pay for the escrow fee. You also need a attorney to review this contract and you need to consider those legal fees as part of your bid to this company.</p>



## Answer 9590

- posted by: [Steve Wilkinson](https://stackexchange.com/users/-1/2177-steve-wilkinson) on 2010-03-25
- score: 3

Gary has written about escrow, and that is the proper formal way to provide your customer access to your source.  As a general rule though, source is next to useless to 95% of customers as there is a very small likelihood they will have the skillset or resources to deal with an issue in your code.  Somehow it provides a level of piece of mind though.

However, depending on the nature of the customers' business and to an extent your relationship with them, **you may like to consider giving them (or selling them) the source as part of the deal**.  This would be done under a tight agreement which requires them to keep it confidential and restricts their rights to using the code internally for the purposes which it was sold for, but this has the advantage that they can take a look at it from the start (if it's well organised, it boosts their confidence, etc), and you don't have the extra cost of escrow.  I would recommend a policy that forbids them from changing the code and deploying it, as that would bring you a maintenance nightmare.

You would still need to provide them with updates to the source every time you ship a new release (as you would with escrow) but it's probably a bit more straightforward.  

Of course, this is something you may not want to do if your source contains a lot of important proprietary secrets, or if you have something to hide in terms of code quality.  

Finally, if the system has some sort of license key restriction, you may want to think twice about giving them that bit (although with the source they could work round it).

I have seen this approach work well under certain conditions so I thought it worth mentioning.


## Answer 9588

- posted by: [Oleg Barshay](https://stackexchange.com/users/-1/1098-oleg-barshay) on 2010-03-25
- score: 0

Companies fail all the time.  Even doing business with larger companies, divisions close and product lines are often discontinued.  There are no guarantees anyone, no matter how stable, will be in business with the same product three years from now.  

You can be informal about it and tell them that should you go out of business you would be open to selling them the code.  However, if they are a large firm an informal agreement may not be sufficient for them.  

If this is big sale for you, you can include a right of first refusal and/or an option to buy in the contract.  Typically this is done in conjunction with a software escrow service.  Make sure you increase the sale price to account for this as this grants them a lien on your product.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
