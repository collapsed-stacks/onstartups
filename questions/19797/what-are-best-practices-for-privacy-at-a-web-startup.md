## What are best practices for privacy at a web startup?

- posted by: [Jon Pincus](https://stackexchange.com/users/-1/7036-jon-pincus) on 2011-02-04
- tagged: `website`, `privacy`
- score: 4

Beyond the obvious steps -- having a privacy policy, encrypting stored data, supporting https logins and Tor -- what are other best practices for a web startup that wants to do privacy right?


## Answer 19831

- posted by: [Tim Nash](https://stackexchange.com/users/-1/7035-tim-nash) on 2011-02-05
- score: 4

Having a privacy policy is one thing, doing what you say you will in the policy is the important part. 

While individual laws are different country to country as good practice you should:

 - Identify the reason for storing individual personal data
 - Identify the period of retention for the data
 - What parties have access both internally and externally (does joe really need to see the CRM database?
 - Identify the mechanism in which a visitor/user can find out about what data you hold on them.
 - Identify the mechanism for destruction and removal of data.

If you share data with third parties (and that includes Google ;) ) it's important you know how the data is being treated and it is at least in part inline with your own.

By using the above you can then, work through the issues such as how are you storing data, who has access etc, and who is enforcing this?

In the UK for example a company should appoint a person who is responsible for enforcement of privacy, though the law was changed so that the person can be the company as a whole (in terms of liability) this is similar in Europe, in US I believe it varies state to state. 

As a company going through and saying, why are we collecting x, who is using it, how long are we storing it, do we have to store it can be a painful exercise, especially as even in companies which thought they were doing the right things, often find a large amount of highly personable data sitting in a spreadsheet on a laptop normally of someone who has no need for the data.

One final tip, CEO and other executives even in a small startup have no more need to access data as anyone else, try to avoid having master key holders especially ones with no one looking or auditing them, especially for very sensitive data, same goes (and even more so) for their PAs




## Answer 19798

- posted by: [Ryan Elkins - IActionable](https://stackexchange.com/users/-1/2566-ryan-elkins-iactionable) on 2011-02-04
- score: 2

I'm not sure if you meant privacy or security (your examples are really more examples of the latter), but as for privacy I would say one of the main things is to protect your user's data. Don't display their email publicly or in a manner that's easily scraped. If you ask for a lot of personal information, make sure they know what it going to be available to others and what is more for internal use only.

Along those lines, even though it may be in a a privacy policy, no one really reads those, so be careful if you start selling off user's data. In general I would say if you ever find yourself wondering if users would be upset if they knew what you were doing with their data then maybe you should reconsider. If you have APIs make sure users are aware of what is publicly available via these APIs. 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
