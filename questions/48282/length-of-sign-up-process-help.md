## Length of Sign-up process- help?

- posted by: [Stanford Sequeira](https://stackexchange.com/users/-1/19368-stanford-sequeira) on 2013-03-29
- tagged: `website`, `ecommerce`, `web-design`
- score: 1

I am starting a website consisting of info of local shops. now I am in a dilemma over the vendor sign-up process, I want to know should I do it one of the following ways - 

 1. just ask for contact info, email and get back to them ? or 
 2. ask for all details like shop name, type, address,website, contact person name? and then after I verify the details, activate the account and let them fill in the remaining details?

In short what is the best way to get maximum sign ups or how to develop a sign-up which doesn't ask for endless details?

How do I ask store owners during sign up if they sell genuine products? I mean how do I phrase the question ?

Thanks in advance!


## Answer 48285

- posted by: [Michael Nail](https://stackexchange.com/users/-1/25300-michael-nail) on 2013-03-29
- score: 1

To me, it sounds like by the time your user has started the signup process, he or she knows what the product/service which you provide is. If you we providing some kind of social widget, I might say that the signup process should be kept as simple as possible. However, what you're offering sounds like a business solution! In that case, my intuition is that you should get as much of your user's information up-front as possible.

When I think back to all the "business solutions" I've signed up for, most of which I didn't end up using, it turns out that most of the ones I didn't end up using had some kind of major break in the startup processes early on. The ones where I had to enter only a little bit of information and then wait for a phone call usually resulted in a bait-and-switch where the fellow on the other side of the line wanted me to pay something on the order of 4- and 5-figures for whatever they were offering.

These days, when the signup process breaks early and I have to wait for contact from somebody, I expect to hear from a sales person, even when the website says whatever I'm looking into is free. Because of this, by the time I get that phone call, I've already looked into a number of other solutions.

If your call is a sales call, I hate to say it, but you might have to do the same thing as the people I'm describing above, and withhold pricing information until you got someone on the phone. HARO uses GotoMeeting to give a powerpoint presentation to their prospects, and it seems to work pretty well for them, but HARO is the *ultimate* bait-and-switch operation. They lure you to schedule a phone call by making you think they're going to help you learn how to better use their platform to get in touch with reporters. Instead, when you get on the call, they sell you access to a $2k -$5k/year social media analytics and PR management suite. They certainly know how to pull in a warm prospect, but if I knew what I was going to hear about before the call, I wouldn't have even picked up the phone. I must say, after their presentation, I *really* wanted the social/PR suite at my disposal. I wanted it the same way I want a fast car and a king-size bed: not in a rational way. I just wanted it. I didn't wind up getting it.

Now, if you're offering a fermium service for businesses, then I'd recommend letting the user complete as much of the signup process as possible on their own. I don't know much about what you're making, I don't think you shouldn't be worried too much about the length of your signup process unless it takes more than, say, 3 minutes to complete. The shops that are signing up probably aren't going to scoff at the prospect of filling out information for 3 minutes to be on a directory. 

Here's an idea: take phone # information on the first page. If the user doesn't complete all of the forms, give him or her a call!

As for how to design a sign-up that doesn't ask for endless details, that might be a question for Stack Exchange>User Experience


## Answer 48286

- posted by: [Matthew Brown](https://stackexchange.com/users/-1/24003-matthew-brown) on 2013-03-29
- score: 1

This is possibly the most important question that you will ask. On the one hand you want the least number of barriers between a sign up starting and the account being created but on the other hand you need a lot more information that email and name.

User Interface designers often work hard to play on the psychology of laziness by making things appear easy and short. A low count of form items and bigger than average formatting (big boxes, big test etc) with short paragraphs and headings etc all help.

One way round this is to set up the form to ask for no more than three bits of information. Usually this would be email address, name of person and then in your case Business name. At that point you have a lead and you want to save that date so I would go ahead and have them submit that. On the landing page of that form I would be looking to direct my designer/developer team to place a progress bar indicating that the sign up is 25% done - this basically says that there are 3 more pages as easy as the last one. More importantly I would want the records created in the database so that if the user drops out they can be emailed a link that will take them right back to the page 2.

On the page 2 I would ask my developers to place a password creation form with just the choose and confirm password options. I would want lost s of nice UI elements like password strength indicators and basic validation and then pass them on to page 3.

As part oft he form processor for page 2 going into page 3 I would want the welcome email to be sent. This will direct the user to a profile page that they can edit. From a business work flow point of view I would want to nag the user at  a steady rate if they do not "complete their profile" and remind them that they are at a disadvantage compared to competition if they don't.

Page 3 I would use to hide the basic information grab. This is data that you largely cannot live without. Phone number, postcode/zip code, that sort of thing. 

Then page 4 is where you get all the juicy bits.

If they are with you on page four then your database already holds enough information for you to phone them and talk to them so saving this lead from going stale is easy from here on.

On page 4 I would want my developers to make a nice empty looking AJAX powered form. So they can add elements to their profile "to be more competitive". Again the profile completeness progress bar is a great idea for this sort of thing. Think how LinkedIN and others do this... While the user is, at this stage, free to add or not add they have invest all the time getting here and are, in their minds, committed to showing that they did not waste their time.

As long as your service can live with some local businesses not filling it all in you have balanced easy form with comprehensive form.

Most local businesses will do a poor job of getting the data all in place so I would suggest having field drives. So for example Monday we get all the users without an industry selected and we write a standard email explaining why they need this data on their profile and the "fact" that most businesses miss out through not having one (and how those that do have it do so much better). Because you are being specific and offering an advantage uptake will be quite high.




## Answer 48283

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2013-03-29
- score: 0

You should allow people to enter as much or as little information as they wish, with the understanding that certain details are required before they can be activated.


## Answer 48284

- posted by: [bhttoan](https://stackexchange.com/users/-1/23673-bhttoan) on 2013-03-29
- score: 0

What is the minimum they need to enter before their profile can go live? That should be your minimum otherwise you will need to add in validation before letting their profiles go live. Do try to keep it simple and focus on the real minimum and do not ask them to enter descriptions etc which require thought and planning as that will discourage signups.


## Answer 50579

- posted by: [Dmitri Zaitsev](https://stackexchange.com/users/-1/27575-dmitri-zaitsev) on 2013-08-24
- score: 0

It all depends on how much value they will see on your site.

If they are already motivated and eager to give you the info, go ahead and collect it. But make it simple - single form page with required fields clearly marked and JavaScript (and if needed AJAX powered) auto-validation so they don't waste time by submitting invalid data and waiting for response.

If they are less motivated and you got only little attention span from them, make it as easy as possible - Email/Password is the standard minimum or use Social/OpenID registration - even easier. However, the question is, what then? What do they get from that right away? If not much, then what was the point?

Now, the question about genuine products - they probably provide some guarantee, do they? Are they sending products themselves? 

You also mentioned the shops are local, then can you simply visit them once you have their address? Or you can check them online? Calling or emailing them is another option but they may feel it to be intrusive, esp. calling.
 



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
