## Are Any Companies Doing Anything Interesting / Creative / Fun with their Phone System?

- posted by: [Kyle West](https://stackexchange.com/users/-1/4267-kyle-west) on 2011-05-26
- tagged: `phone`, `copywriting`, `writing`
- score: 1

My company is implementing an automated phone system (press 1 for sales, 2 for support, etc.) which I absolutely despise. We've gotten to the point that transferring calls around, getting in touch with the right person, etc. has become a huge PITA. Hiring a receptionist or putting everyone "on call" is not an option.

I am determined to make our system less crappy than the typical:

> Thanks for calling ACME Corp, this is out awesome slogan. To serve you as quickly as possible please select from the following options. Press 1 for sales, 2 for support, 0 if this makes you want to kill yourself.

BUT I don't know where to start. It has to be similar enough that people know what's happening but less lifeless and corporate. 

Has anyone had a good experience with this sort of system? Does anyone have ideas for the script or interactions?

Thanks!

Kyle


## Answer 25541

- posted by: [Jeremy Parsons](https://stackexchange.com/users/-1/4291-jeremy-parsons) on 2011-05-27
- score: 1

Like code, automated attendant features must be DRY. How often have you got frustrated by two or three stage voice menus that are just plan dumb, or been asked to speak or key information that the person who eventually answers the call seems not to have access to? 

The other point where people get sloppy is that, when you record a new message, you should generally be re-recording all the other messages too, so that the user experience is consistent. That's true even if it's the same person's voice every time - the tone, the feel and the background noise will vary for messages recorded at different times and from different places, which just increases the sense of an impersonal system. 

Where the core issue is trying to get the customer to be specific about where the call needs to go, in my view the main options should also be available as separate phone numbers. So the first time I call your general number I hear the options, but when I select 1 for customer services, either the auto attendant tells me the number I can dial next time to go straight through, or the person answering the call tells me (assuming they can tell I called in on the general number). Whether I actually note that number and use it in future or not, I know the option to bypass the system is there.

In a startup context, you often end up sharing call handling across functions. Again, take care first that the system is set up so that people can know who the caller is trying to reach, and document how to take calls so that people respond appropriately. It's frustrating and unnecessary for me to call for technical support and have the person answering the call not already know that.

As important as having clearly voiced, simply expressed choices is what happens when the call is ready to be answered. You may have a system with sophisticated support for hunt group logic, or you may have limited capabilities. Think through whose phone(s) should ring first, and how quickly incoming calls should be escalated to alternate or wider groups. Documentation and procedure is vital here too: most people are pretty good at judging how long it takes for a ring tone to get frustrating, but it's easy to forget the customer has already spent 20 seconds listening to your recorded messages.

When you're planning the structure and writing the script, although there aren't universal standards for how to do this, there are certainly conventions. Doing things differently is usually going to be more irritating, however much 'better' you think that will be. For instance, one of the reasons most auto attendants start by giving you the company name is that it's good to reassure a caller they dialled the right number - but there are usually a few words before that because a proportion of callers aren't really listening the moment the system cuts in.

Finally, you should be paying just as much attention to the data that comes from your phone system as you do to web analytics. You need to care about abandoned calls, the time people wait for an answer, how often calls are forwarded and so on. Reviewing the data regularly gives you the best way to improve both the system and your (human) call handling - which translates into more and (hopefully) happier customers!

It's right to have an instinctive aversion to these systems. That's a reminder that what you want when you call another company is to find yourself talking to a real person, and the right person, in the shortest possible time. Set your system up to achieve that goal for your customers and you won't go far wrong.


## Answer 25540

- posted by: [Calvin Froedge](https://stackexchange.com/users/-1/10772-calvin-froedge) on 2011-05-27
- score: 0

If you folks have a strong development team and want to build something insane, take a look at Asterisk: http://www.asterisk.org/

It's a totally open source project for building communications systems.  In short, it's amazing.

If you're looking for something quick, cheap and easy, I've used onebox and RingCentral before.  Both provide a pretty cool experience, maybe a bit better than the average customer is used to.


## Answer 25578

- posted by: [Kenneth Vogt](https://stackexchange.com/users/-1/6736-kenneth-vogt) on 2011-05-27
- score: 0

Have you ever called Geek Squad? They have a campy Agent 007 kind of vibe going on. It is very engaging and yet the fun doesn't get in the way of getting you where you need to go. Call them and wonder around their IVR.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
