## Figuring out margin on fixed costs

- posted by: [James](https://stackexchange.com/users/-1/7272-james) on 2011-02-11
- tagged: `pricing`, `hosting`, `cost`
- score: 0

I'm currently hashing out my price points for a hosting service that I plan on launching on Amazon AWS.

The biggest line item in the budget is currently the machine time. I know that if I give a user x GB of transfer it costs me x cents, and the same with storage space. How do I calculate how much that customer costs me as part of the server hardware overhead?


## Answer 20131

- posted by: [darren](https://stackexchange.com/users/-1/7271-darren) on 2011-02-11
- score: 3

To be honest some figures are needed; for me at least, or some idea of if the machine time is really a fixed cost or if it will vary based on the number and size of the user accounts. 

I think more pertinent is what do your competitors charge and how can you be competitive (ie rapid deployment for RoR like Heroku)

But…

Mathematically [from scratch for readability to all, in the case others may search this with no previous knowledge in the future] 

profit(π) = total revenue(TR) - total costs(TC)

TR = price(P) x quantity(Q)

total variable costs(TVC) = (VC)Q

TC = fixed costs(FC) + (VC)Q

From your question you are stating that the machine time/server hardware is a (FC).

Also you have to assume that the FC is variable in the long run and dependant on the (VC)Q

Assuming that (VC) = 1 ie 1GB of transfer and storage per customer. You will then just need to find the capacity that each FC (one hardware) can sustain and divide through using VC and then multiply by Q

ie FC is $100 and VC is $1 (multiplied by 100 [the capacity that the FC can bare]) then

FC/VC = 100/100 = 1 then

(FC/VC)*Q = 1*Q = your TC

I realise that this answer is ridiculously simplified but based on the info provided i would be amazed if anyone could provide you with a better one.



Anyway I hope that this helps. 

- If you provide further info i will add more to the answer tomorrow. 


## Answer 20507

- posted by: [Community](https://stackexchange.com/users/-1/-1-community) on 2011-02-20
- score: 0

It depends on how much you want to subsidize your new customers, with the hope that once future customers arrive, you will make money. You need to spread machine costs across all of your customers. So, when customer #1 arrives, you cannot charge the entire cost of a system to them. You will need to figure out how many customers it will take to reach your break-even point for machine costs. Divide fixed machine costs by that number, to price it for your initial customer.  So you may sell the first one, but if you never get to the expected break-even number of customers, you do not make any money on machine fixed costs.


## Answer 20852

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-02-27
- score: 0

It's a fair and simple question. There isn't a simple answer.

Suppose you have a fixed cost of $1,000. You are confident that this will service up to 250 customers, and you have built a business case with an expectation of selling to 50-150 customers. What is the correct cost allocation per customer?

Maybe it's $20. That sets a conservative expectation - the $1,000 is spread across the 'low case' 50 customers.

Maybe it's $10. That's the midpoint expectation - $1,000 spread across the central view of 100 customers.

Maybe it's $4. That's $1,000 divided by the 250 customers the infrastructure could actually support.

And maybe it's $0. That's recognising that in the general case, a new customer is not generating new cost.

All these (based on that very basic sketch) are valid, but that range under-states real life complexities. 

For instance, what happens as you approach 250 customers? Maybe there's another $1,000 cost slug coming your way. Or maybe there are economies of scale, and the next chunk of cost will be $500. Or maybe there are dis-economies, and you'll have to spend $1,500. Each of those calculations needs revising, and there are some more methodologies that you could use to address that 'semi-fixed' character.

But then step back. If your expectation were 20 customers not 100, would you have done things differently - could you have chosen a fixed cost of $500 in this case, or even avoided fixed costs altogether? Often. So where does that leave those numbers?

Before you despair, life becomes rather simpler when instead of talking about 'cost,' you qualify by saying, for instance, 'cost from the perspective of the pricing decision.' And I suspect this is the type of cost you may be concerned about.

Then you should be looking first and foremost at the marginal cost - which is probably the lowest of all the figures you can work out. You should have alarm bells ringing if your pricing goes below this cost - and either eliminate these cases by price and proposition design, or build in risk management if, for instance, this arises from patterns of use you can't know in advance.

Then your pricing process will be (I would hope) pricing based on opportunity, which will be based on views including

* Your chosen target market
* Current competitor offerings
* Typical competitor cost bases (in this case, you'd probably look at hosting companies running their own systems and at main white label offerings offered for resale)
* Value of distinctive features (for instance, if the way you've built your offering allows you to offer higher uptime, stronger backup, better performance etc etc than market norms)

As a final note to anyone who's horrified by the thought that the cost floor might essentially ignore fixed costs, consider the following:

1. A competitor with access to the same infrastructure (and AWS isn't a secret!) will have similar economics. Other cost allocation approaches may feel prudent, but they may bake in a wholly artificial 'cost disadvantage' that closes off potential markets to no benefit

2. Even in highly competitive markets, there's a constant disincentive to charge 'at cost,' so that the apparent comfort in over-stating floor cost is unnecessary

3. In initial business cases, it's very common for variable costs to be overstated (in this case, does a customer taking a 20GB data transfer package actually use the 20GB that was put in as a 'cost'>) - and even in cases where sophisticated cost driver analysis has been carried out, it is generally the case that there's an inherent benefit in achieving some level of scale - which is one reason why new entrants will often use aggressive price offers

4. In this area of hosting, many of the underlying costs are on reliable downward trajectories, so that it's probable that each time cost is reviewed the new cost calculation will produce similar or lower costs. An aggressive and efficient competitor reviewing the same landscape may even choose to take this into account and discount expected actual costs to take into account customer lifetime factors.   



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
