## How to charge a customer for a tailor-made solution (ERP)?

- posted by: [DLlamas](https://stackexchange.com/users/-1/1599-dllamas) on 2010-03-10
- tagged: `enterprise`, `charging`, `pricing`
- score: 2

We are designing a tailor-made ERP application for a SMB customer whose processess are very specific and have been very succesful for the last 20 years. Question is: How to charge for the project? They don´t have any IT experience so the whole process is being requested from operations understanding up to project management for implementation.


## Answer 9084

- posted by: [Mike](https://stackexchange.com/users/-1/2696-mike) on 2010-03-10
- score: 1

If their process is working well for over 20 years, they probably have it well specified and documented, right?
If so, you should take it and come up with an estimate of the effort to implement that scope with the technology you use.
The problem here is:
- Is the technology you use capable of managing unforseen change requirements?
- Do you have a formal scoping and sizing process (besides your accumulated project experience)?
- Is it really a "take their processes and code them" kind of project, or is that what they tell you and then you end up having to figure out most of the requirements because things are not as well defined as they think?

At my company (OutSystems) the service delivery team uses a scoping tool based on user stories, that automatically generates an estimate of the effort based on patterns. Then they propose a time-boxed project where those features will be implemented. If the requirements change (new stuff gets added for example), the feature list is renegotiated, but the time-box is fixed. That means that the customer knows when he will receive the solution, and knows, upfront, that if he starts adding features (or asking for changes to original features) he'll have to drop some, to ensure the delivery date is fixed.

All the undelivered features usually make up a second version release, that will work using the same principle: a time-box with enough time to implement all those additional features.

We found this to work very well but requires educating the customer on this process. It will be too easy for the customer to try and shove all he can in the project, but if you manage to manage this well, the interaction and collaboration you have with the customer during the project will ensure you deliver THE solution they need, and not the solution that originally though they would need.

Hope this helps




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
