## Licensing inactive units

- posted by: [bhttoan](https://stackexchange.com/users/-1/23673-bhttoan) on 2013-09-16
- tagged: `saas`, `license`, `licensing`
- score: 1

In an HRIS (human resources) application there are active and inactive employees - the inactive need to be kept for legal reasons but also for application effectiveness as employee id is used as a lookup in many modules.

From a licensing standpoint, the industry practice is to only charge for active employees - if a client has 100 active employees and 500 inactive they only pay for 100.

The problem is that at any time an employee could be moved between the two states which opens the system up to manipulation - for example, client above archives 100 employees and moves 100 of their currently archived employees to active hence never passing 100 active employees but, in effect, they are managing 600 employees but paying for 100.

This use case is specific to an HRIS but how do others approach licensing for inactive or archived components when that component is their main pricing meter? The only way I can think of is to either restrict the movement from inactive of active to x% of their total active per month or limit the number of inactive to x% of total active - any other thoughts how to do this without impacting the genuine customers?


## Answer 51025

- posted by: [Dave Feyereisen](https://stackexchange.com/users/-1/8565-dave-feyereisen) on 2013-09-19
- score: 1

<p>Consider letting them game the system, but make it very inconvenient.  For instance, consider things like only allowing for active employees to be viewed in Reports.  Or, only allow 1 employee to be moved at a time from Active to Inactive.  Or something similar...</p>

<p>I don't like trying to eliminate the possibility of them gaming the system.  And I don't like the idea of charging for every employee who was Active even briefly.  These approaches are often anti-productive because they tend to inconvenience the normal users who are NOT trying to rip you off.   </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
