## Web based software issue submission and management?

- posted by: [Kim Jong Woo](https://stackexchange.com/users/-1/3650-kim-jong-woo) on 2011-11-20
- tagged: `crm`, `bug-tracking`
- score: 1

I am looking for a way to let my customers enter any issues they have, and be able to check the status of the issue. Sort of like what you see in the Google code issue tracker.

I want to be able to host this on my own domain if possible. 

I signed up for fogbugz but when I arrive at mysite.fogbugz.com there's no way for customers to sign up and submit issues.

built in CRM functions would be a huge plus.

I don't mind paying but would like to use a free plan to get a feel for it.



## Answer 32803

- posted by: [Paul Filmer](https://stackexchange.com/users/-1/14049-paul-filmer) on 2011-11-20
- score: 0

Helpspot is worth looking at - http://www.helpspot.com/ - we use both Fogbugz and Helpspot and the latter is much more customer and user friendly for the support desk staff. It has a built in portal that can also be customised (both design and functionality).

You can have address books for customers, and these addresses can come from a file on disk or another database, or another system entirely (such as a dedicated CRM or accounting system).



## Answer 32813

- posted by: [Van Gale](https://stackexchange.com/users/-1/14556-van-gale) on 2011-11-21
- score: 0

<p>I'm not sure it's good (from a customer perspective) to have customers and developers using the same bug tracking system.</p>

<p>In my opinion it's much better to let the developers use their favorite bug tracking tool on the back-end and have a customer support system on the front-end to handle "case management" etc. This will provide a much friendlier experience for customers with issues and you should still be able to tie the two systems together.</p>

<p>I haven't really seen any open source tools that I can recommend but there are some good commercial ones like <a href="http://www.assistly.com/" rel="nofollow">Assistly</a>, <a href="http://www.zendesk.com/" rel="nofollow">Zendesk</a>, and <a href="http://tenderapp.com/" rel="nofollow">Tender</a>.</p>



## Answer 32841

- posted by: [David Silva Smith](https://stackexchange.com/users/-1/6292-david-silva-smith) on 2011-11-21
- score: 0

I had the same requirement, enable customers to enter an issue they have and check the status.
I ended up using Atlassian Bitbucket.

You are able to host this on your own domain. It does not have built in CRM functions but does have a free plan.

Free sign up here: https://bitbucket.org/account/signup/?plan=5_users



## Answer 37657

- posted by: [Tim](https://stackexchange.com/users/-1/14914-tim) on 2012-03-28
- score: 0

I have used bugTracker.net > http://ifdefined.com/bugtrackernet.html and have had success with this platform. you can host it and it's source is open so you can build on to it. You can also set up groups and give access to users so your users can be throttled back to using and seeing what you want them to see, and it's free!!


## Answer 38573

- posted by: [Matthew Dorian](https://stackexchange.com/users/-1/5382-matthew-dorian) on 2012-04-27
- score: 0

I've used Mantis.  It's open source and allows you to do what you're asking.  However, I agree that a custom front end might be a better experience for your customers.  Mantis has come API's you can use to build this.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
