## Should I agree to an indemnification clause?

- posted by: [Steve Hanov](https://stackexchange.com/users/-1/1958-steve-hanov) on 2009-12-16
- tagged: `legal`
- score: 6

I have a sole proprietorship in Canada, and sell software that I have created to corporations in the US. One of them has asked for an indemnification clause. First of all, I don't know how to write such a clause. Hiring a lawyer could take much of my year's profits. Secondly, if I agree to include one, what am I getting myself into? Is there any way to politely dissuade them from it without losing the sale?

Edit: Is it possible to limit the clause to the purchase price?



## Answer 5159

- posted by: [Alex Papadimoulis](https://stackexchange.com/users/-1/123-alex-papadimoulis) on 2009-12-16
- score: 12

**Be very careful with indemnification.** It *could* bring you into a whole world of hurt, especially since you're operating as a sole proprietorship.

Let's take a fairly cookie-cutter blanket indemnification clause:

> steve.hanov agrees to indemnify Alex Papadimoulis against all liabilities (including legal costs) which may arise from the usage of steve.hanov's software

Assuming it wouldn't be thrown out as unconscionable, this binds you to paying for all damages *and* the cost to sue you for said damages that *might* come out of usage of your software. Let's say your scheduling software has a JavaScript bug that causes an alert not to pop-up, which causes a missed appointment, and that causes a lost client.  You may very well have to pay for that... which may be 10x or 100x the cost of your software.

It's unlikely, since they probably won't go after a small, sole propietor... but I wouldn't risk it. If you're going to offer indemnity to another party -- and you're not even sure how to write the clause -- you should strongly consider bringing on a lawyer.

--<br />
**UPDATE**: In response to your update, you can phrase it however you'd like. The key thing is understanding what they want indemnity for. Do they want to be protected from people who sue you (e.g. you violate patent, they could get sued for using your product)? If they want general product liability, then you should absolutely limit your liability to the purchase price.


## Answer 5169

- posted by: [Dane](https://stackexchange.com/users/-1/1441-dane) on 2009-12-16
- score: 7

Alex makes very good points, you want to be very careful what you indemnify for.  My experience is that what companies are mostly concerned with is the case where your software infringes a patent and because your customer is using that software the patent holder can sue them (as they will probably have deeper pockets than you do).

This is where having a license agreement makes sense as it will cover these issues in a hopefully balanced way which provides protection for both yourself and your customer.

To answer your specific question here are the clauses we use with annotations,  feel free to use any of this language that works for you.

So in this part we specify what we are going to indemnify them form with limits of what we will cover:

*"Licensor will defend or settle, at Licensor’s expense, any action brought against Customer to the extent based upon a claim that the <company name> infringes any United States or European Union patent issued as of the Effective Date, copyright, trademark or trade secret, and Licensor will pay such damages and costs as are finally awarded against Customer attributable to such action, provided that Customer (i) notifies Licensor promptly in writing of any such action, (ii) gives Licensor sole control of the defense and/or settlement of such action and (iii) gives Licensor all reasonable information and assistance (at Licensor’s expense, excluding time spent by Customer’s employees or consultants) in connection with such action."*

Then we define what our options are for resolving the problem:

*"Should the Software become, or in Licensor’s opinion be likely to become, the subject of such an infringement claim, Licensor may, at Licensor’s option (i) procure for Customer the right to use the Software free of any liability; (ii) replace or modify, in whole or in part, the Software to make it non-infringing; or, if (i) and (ii) are not commercially practical, (iii) terminate this Agreement and refund a pro-rata portion of the license fees paid by Customer based on a three-year straight-line amortization of such license fees."*

And lastly we make sure that it's our software that actually caused the infringement:

*"Licensor assumes no liability for any infringement arising from: (i) any method or process in which the Software may be used; (ii) any compliance with Customer’s designs or specifications; (iii) use of other than the current unaltered release of the Software; or (iv) the combination, operation or use of the Software with any third-party programs, data or hardware.  THE FOREGOING IS LICENSOR’S ENTIRE LIABILITY AND CUSTOMER’S SOLE REMEDY FOR ANY CLAIM THAT THE SOFTWARE INFRINGES ANY INTELLECTUAL PROPERTY RIGHTS."*

Although if I was going to shorten this I would probably leave this part out based on how customers use our software.

You also asked about limiting your liability which Alex also brought up.  If you're going to add indemnification I would add something that limits your liability for all cases, including things like missed appointments as Alex mentioned.

This is what we use.  To make it more palatable we make it reciprocal.

*"NEITHER LICENSOR NOR ITS LICENSORS WILL BE LIABLE FOR ANY LOST PROFITS, LOSS OF DATA, COST OF PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES, OR FOR ANY CONSEQUENTIAL, INCIDENTAL, SPECIAL, INDIRECT, OR EXEMPLARY DAMAGES ARISING OUT OF OR RELATING TO THIS AGREEMENT, HOWEVER CAUSED AND UNDER ANY THEORY OF LIABILITY (INCLUDING NEGLIGENCE), EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.  Customer acknowledges that the amounts payable hereunder are based in part on these limitations, and further agrees that these limitations shall apply notwithstanding the failure of the essential purpose of any remedy.  Licensor’s total and cumulative liability arising out of or in connection with this Agreement shall not exceed the license fees paid by Customer hereunder."*

Hope that helps.

disclaimer: I'm not a lawyer and this should not be considered legal advice.


## Answer 5175

- posted by: [edwinoh](https://stackexchange.com/users/-1/1598-edwinoh) on 2009-12-16
- score: 1

I agree with Alex's overall comments.  I would just add that I would *never* accept any kind of open ended indemnification.  No business is worth the risk of putting your company under.

Second point:  If you do grant any kind of indemnification, get insurance.  Commercial General Liability (CGL) insurance is a commodity and pretty cheap.  E&O insurance might also be worth looking into but costs range from cheap to outrageous;  check with an independent broker.


## Answer 5229

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2009-12-17
- score: 1

Steve,

1. If you are selling software, you should invest in an standard licensing agreement.  Negotiating individual agreements with each customer on a case by case basis is not something that you are going to want to do for long (unless your price point is 50K+).  

2.  You have no business attempting to draft an indemnity clause yourself.  I dont say this to be rude; there are many parts of a contract that you could probably draft yourself, but this is one of the those areas that does require some actual legal knowledge.  The last paragraph of Danes' example is not actually an indemnity provision at all, but rather a limitation on damages. These both deal with similar issues (i.e. liability), but by no means are they the same - damages refer to losses suffered by the client as result of use of your product, while an indemnity covers losses as a result of your client being sued by a third party. Depending on how the indemnity clause is drafted, this limitation may or may not apply to the indemnity at all.  

3.  You definately can limit the indmenity to the purchase price (or any other number), if you can get the other side to agree.  Like I said, these limitations need to be carefully drafted. If you had a standard contract, this is the sort of thing you would want to try to include.  

4.  No one has mentioned this, but your problems are compounded by the fact that you are a sole proprietership.  If you are were a corporation or an LLC, then your potential loss would at least be limited to the company level.  As a sole proprietership, they can come after your house, yoru car, your savings, etc.  If you are at the point where you are signing deals with customers, you should get this done ASAP.  If you sign a contract with a customer, then incorporate your company afterward, you will NOT have the benefit of the corporate shield if the customer sues under the contract (since you signed in your personal capacity).  
   
You should try to find a small business laywer to help you.  You should be able to get them incorporate you and do a short licensing agreement for a relatively small fee (under $2k).  Or alternatively, you should be able find an incorporation service that will handle forming and registering your corporation or LLC or about $500.  Then you can probably find a cheap attorney on guru.com or elance to put together a license agreement.  If you are (a) really cheap and (b) really confident that nothing could ever possibly go wrong, then just get yourself incorporated ask the client to draft the indemnity.  You should expect to get the broadest indemnity that is legally conscionable, but at least you will be incorporated and not putting your personal assets at risk.

Wish you the best.

Disclaimer:  This is not legal advice.  If you need legal advice, please contact an attorney.

  


## Answer 5395

- posted by: [user2013](https://stackexchange.com/users/-1/2013-user2013) on 2009-12-22
- score: 1

I work for a software company and this is an issue we see coming up more frequently. Specifically we are seeing ip idemnity as the real customer concern and mostly it is being driven by lawyers. You should consider what ip you are covering. Is it just your own? Many products today are developed using lots of open source libraries, so you should probably carve out any third party open source and only indemnify your own. Also if you license any third party software that you include, you can transfer your rights that third party assigns you onto your customer.

If you do develop a standard clause I would recommend leaving it out of your contract and only adding it in if the customer requires it and won't back down. Each will be different and how strongly they feel about this issue is going to depend on the personality of the lawyer. 

good luck.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
