## Interpreting Invention Assignment: what does "is not related" to the company's business mean in employment contracts?

- posted by: [kamikaze_pilot](https://stackexchange.com/users/-1/6768-kamikaze-pilot) on 2011-12-25
- tagged: `software`, `intellectual-property`, `copyright`, `legal`, `bootstrap`
- score: 1

I'm talking about those Invention Assignment clauses in employment contracts (especially with regards to California labor code section 2870)

"Prohibiting employee assignment to an employer of inventions that the employee developed entirely on his or her own time without using the employer's equipment, supplies, facilities, or trade secret information, except for those inventions that either: (a) relate at the time of conception or reduction to practice of the invention to the employer's business, or actual or demonstrably anticipated research or development of the employer; or (b) result from any work performed by the employee for the employer."

Suppose the company makes windows software using C++ that specifically targets financial institutions in providing them financial data...and then a Windows C++ programmer that works for this company make a Windows minesweeper software using C++ purely using his own equipment and solely on his own time, will that be considered "related" to the company's business simply because it's also a windows software and is also written in C++ (ie. despite the fact that the program itself (minesweeper) is completely irrelevant to making financial software that provides data to financial institutions)? Ie. if that scenario occurs, will the company then have ownership of the minesweeper program source code?


## Answer 34157

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2011-12-27
- score: 0

Note that a company can sue you or come after you whether you are in breach or not.  They can make in painful and expensive if they want to, and I'm not a lawyer.

Programming languages do not correlate to any practice, or specific knowledge from an employer. Companies around the world use many different languages and your employers competitors also probably use it so it's not really part of any strategic advantage.  If they have custom libraries or frameworks that the employer created and you use those in your work that would be an issue. But since you are making a GAME and your employer works in banking / financials that would be a pretty clear separation.  If you were making a game based on an idea you got at work about a fun way to categorize expenses or organize finances then that 'may' be crossing the line.  But even then, that's not your employers line of business and they are not in the business nor are you in the business at their place of employment to make games.


## Answer 34209

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-12-28
- score: 0

I realize that this California statute is the subject of the question, but in general - 

I suspect (I am not a lawyer) that the intent of the law is for the employer to define what is meant by "related" business areas. 

When you sign a non compete or assignment of invention rights agreement, the contract should state very stringently what is the exact nature of the "related" area of business that the employer is interested in protecting. The California legal wording is generic because it's not possible to be more specific in phrasing a general law on the books. It applies to any business. The employer's task is to fill in the blanks of the phrase "related business means _______."

Here is an example of an excessively broad definition of "competing businesses". A past client of mine had language in his employee agreement that was a non compete provision binding his employees from writing any kind of **accounting software** after working for him.  His niche was tax preparation software but apparently he wanted to keep employees out of any software that involved dealing with money. Accounting software is an enormous sector of software development. Essentially he implied that ex-employees could not take over 50% (or some high percentage) of the available programming jobs after they worked for him. I doubt he intended to enforce this and probably could not do so successfully, but it was pretty intimidating stuff. 

I look for non compete language that is similarly abusive. Ryan has it exactly right - even if the employer is wrong, they can make your life living hell if they wish. 

It is always best not to sign employee agreements that are too sweeping. Of course, it is in the employer's interests to write agreements that as broad and restrictive as possible. 

> Suppose the company makes windows software using C++ that specifically targets financial institutions in providing them financial data...and then a Windows C++ programmer that works for this company make a Windows minesweeper software using C++ purely using his own equipment and solely on his own time, will that be considered "related" to the company's business simply because it's also a windows software and is also written in C++ (ie. despite the fact that the program itself (minesweeper) is completely irrelevant to making financial software that provides data to financial institutions)?

As Ryan said this is a stretch and I don't see that connection being made. 

However, you should know exactly what *is* considered "related to" this area of business, more for your own employability after leaving this job. Suppose your employer considers **any** financial data scraping or transmission function to be related to their business? 

I could see a court upholding a fairly broad interpretation in most states outside California. (CA has different employee protection laws than the rest of the country.)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
