## OO-design req's for investment?

- posted by: [Xepoch](https://stackexchange.com/users/-1/4488-xepoch) on 2012-03-27
- tagged: `venture-capital`
- score: 1

I'm NOT seeking investment (legally stated for now), but I've pitched my business/goals to a few angels just for practice.  The business is in data processing and is very procedural.  As such, the code...is...well...somewhat procedural.  

There is no new shiny OO (choose your flavor/language) design.  It is basically a list of instructions employing numerous off-the-shelf tools.  The objections I have heard are not geared to market potential but more towards the design philosophy, opposite my expectation. 

It works, it is fast, it scales pretty well uses a scatter-gather & fork-join async durability method to avoid latency, and frankly, it'd be at least 9x the amount of sweat to get it coded and maintained in a "proper" OO stack.

Minus maintainability, at the "end of the day" do investors/VCs/angels care *that much* about the structure of the underlying design?


## Answer 37636

- posted by: [JonnyBoats](https://stackexchange.com/users/-1/3100-jonnyboats) on 2012-03-28
- score: 2

> Minus maintainability, at the "end of the day" do investors/VCs/angels
> care that much about the structure of the underlying design?

Xepoch, you need to understand that investors come in all sorts of flavors and what they care about can vary widely. 

Some investors only want to invest in ventures they can understand so a Doctor might be happy to invest in a biotech startup but not a copper mine for example.

Other investors care more about the management team and less about the specific details of the idea. The theory being that with the right management team defects in the original idea can be evolved into a winning product with time.

Then there are investors who would ask their technical Guru to review your architecture and opine on its viability. In a case like that they care more about their expert's opinion (who they trust) than about trying to understand the details themselves.

In the case of your software, in addition to maintainability, I would assume they would be interested in:

Scalability

Is the technology mainstream - can you easily hire people familiar with it as you grow?

Acceptability of technology to clients - Here perception is key. For example if you used a component (hardware or software) that is viewed as insecure by potential clients then this could be a show stopper irrespective of the reality of the situation.

Does it meet the "punch list" of required attributes such as PCI or SOX compliance as appropriate.


## Answer 37665

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2012-03-28
- score: 0

An investor isn't just buying into the existing code, but your ability to create future code. Although OO (Object Oriented) design has a strong following and may be appropriate for your situation, I'd be more impress if you could benchmark your app and compare a piece of it to an OO equivalent. You could also show the amount of time to develop is a cost without enough benefit. No design is perfect for all situations. Are they worried that this will make it harder to add more developers because your approach is not standard? 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
