## Should the first person in the pool pay for the water?

- posted by: [MDMoore313](https://stackexchange.com/users/-1/23558-mdmoore313) on 2013-04-03
- tagged: `getting-started`, `quote`, `purchasing`
- score: 1

I am providing a quote for wireless service to a client. Without getting too technical, suffice it to say that their site will need a computer to perform this service. The interesting thing to note is that this computer along with the software can be hosted in the cloud, and also has the ability to manage multiple 'sites' (which translates to clients in my case). Now, there are three possible scenarios that I can choose from, assuming I charged the same rate for either option:

>1)Give them their own computer for this task(little to no markup on the computer)
 Cons: -This will add quite a bit of cost to the initial quote. Also, I will have to maintain another piece of equipment, and replace in the event of failure, and this piece of equipment will likely be underutilized.

 

>2)Charge them for the computer, and use that to purchase a computer that I keep at my 'office' that does the same thing. This allows me to service multiple clients with the same equipment, while making the initial costs cheaper for the first client (first person in the pool pays for the water). In this case it would only be part of the water because I would still have to provide a portion of the capital required for the computer.
 Cons: -In the event of a power outage at my 'office' (read *house*), **all** of my clients would lose a portion of the service I provide. Obviously ***not good***.

 

>3)Lease a vps (computer) in the cloud, and charge the client for a fraction of the cost.
 Cons: -They are expensive for this application. I wouldn't turn a profit until I had enough clients to cover the cost of the VPS, which may never happen.
 
I'm leaning toward #2 or #3, if I went with #3 then I could still turn a *small* profit even if I used a portion to lease the VPS for an entire year. That would buy me time to get more clients, but of course, there is no guarantee. I will be charging the client for annual maintenance of the system, but what I had in mind wouldn't be enough to cover the cost of the vps. This would just cover the cost of potentially coming onsite to troubleshoot problems and/or replace hardware.

I'm looking for suggestions as to which route I should take, or if anyone has a better suggestion or a hybrid of what I mentioned above, whether from experience, deductive reasoning, shot in the dark, etc. This may spawn a deeper question of whether to quote high initially and provide low maintenance costs, or quote low and provide medium to high maintenance costs.....

**Update**

I've never come across digitalOcean, glancing at their website though they do have the best prices I've seen. But to elaborate, RAM is the premium when looking for a vps, and I've tested this system on a 376MB from interserve.net ($6/month) and the service wouldn't even *start*, so more RAM is definitely needed. DigitalOcean's 1GB is the best I've seen and I'd give it a shot, I wasn't trying to make this a shopping question :-) but that is the issue with the VPS, RAM is key.

I wanted to keep the client's annual maintenance costs around $150 max to stay competitive, and if a VPS eats all of that up then that lessens the benefit of using one.


## Answer 48422

- posted by: [Chris](https://stackexchange.com/users/-1/25297-chris) on 2013-04-05
- score: 1

First, I think you're putting the cart before the horse. Presenting this client with an at-cost or small-markup option that can then be transferred to a more cost-effective VPS once you acquire more paying clients is within the realm of possibility. Then you can acquire other clients that would use similar functionality, then start pushing them all into the "pool" as the demand warrants. Why overbuy now when server utilization is so easy to move around? (After all, we're talking about a $150/year wireless site project, not the Google search engine.)

Having said that, why not give these options to the client? Give quotes based on relative levels of robustness: the PC-at-home option, the PC-at-their-office option, the low-redundancy cloud service, and the premium-level cloud service. Give reasonable expectations for downtime and risk, then let them pick.

If I were a client, I wouldn't want to be sold a Ferrari when all I need is a Honda. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
