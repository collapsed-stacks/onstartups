## Operational email policy

- posted by: [Itai Sagi](https://stackexchange.com/users/-1/12742-itai-sagi) on 2013-05-04
- tagged: `legal`, `email`, `operations`
- score: 3

We've recently launched a platform and we start aquiring emails from users, partly from facebook and partly on their own merit.

We want to start sending operational emails to our users, for example: users which completed or haven't completed certain actions in some interval.

I see that a lot of services do so, for example: twitter sends you emails when someone follows you or a weekly list of tweets, I've looked through the terms of facebook for example, but couldn't find any reference in their policy for such operational emails.

So the question is: what is the legality of such emails, how often can I do it, and how can I alleviate any legal problems by doing so.
Of course we're going to implement an opt-out for emails.


## Answer 48972

- posted by: [drllau](https://stackexchange.com/users/-1/26055-drllau) on 2013-05-06
- score: 1

<p>I wish there was an easy answer (I did my law thesis on the <a href="http://www.acma.gov.au/WEB/STANDARD/pc=PC_310321" rel="nofollow">Australian Spam Act</a>). You mention opt-OUT (presumptively you're in US) but many other jurisdictions to opt-IN ... ie you need to get permission BEFORE sending them unsolicited messages. The EU recently debating &amp; revising the <a href="http://en.wikipedia.org/wiki/Data_Protection_Directive" rel="nofollow">Data Protection Directive</a>,  and if the email contains "personal" information (which under some circumstances could include addresses) then provisions may apply. Now you say you want to "prompt" users to complete actions (part of transaction chain) but if transaction, then it may fall into the general category of <a href="http://en.wikipedia.org/wiki/Permission_marketing" rel="nofollow">permissive marketing</a>. Contact your nearest Direct Marketing Association has they have suggested codes of conduct (though personally I wonder how they enforce them). </p>

<p>If you are worried about legal headaches, the one I point out to you is the legitimacy of harvesting contacts via screen-scraping or mailing lists. Certain jurisdictions forbid this, it may be easier buying a 3rd party "sanitised" list which may have an audit trail of <a href="http://papers.ssrn.com/sol3/papers.cfm?abstract_id=2239099" rel="nofollow">notice and consent</a> ... ie they've ticked off on receiving such information.</p>

<blockquote>
  <p>how often can I do it, and how can I alleviate any legal problems by doing so</p>
</blockquote>

<p>This is the <a href="http://en.wikipedia.org/wiki/Attention_economy" rel="nofollow">attention economy</a>, if you don't treat people's time (which is NEVER replaceable) with respect, why expect them to reciprocate?</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
