## Mobile Web development environment; build or buy?

- posted by: [Nicko](https://stackexchange.com/users/-1/7870-nicko) on 2012-01-24
- tagged: `software`, `development`, `hosting`, `mobile`, `platforms`
- score: 2

I already publish apps for the major platforms but our mobile development has lagged behind.  I have my developers working on enhancements to our mobile site functionality, but I'm not sure whether to 'roll our own' (meaning, hosting it ourselves) or using a platform like [wirenode][1] or [mobify][2].  Mobile Web is a 2nd-line platform for us but it's too important to be rickety.

My primary concern is managing the myriad compatibility issues; my strategic goal is to increase our platform reach beyond the iPhone and Android apps to deliver a stripped-down, yet functional version to as many users as possible.

Does anyone here have any experience with a dedicated mobile web development/publishing environment?  Any opinions (printable ones) appreciated. 

  [1]: http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&ved=0CCAQFjAA&url=http://www.wirenode.com/&ei=ENkeT-qyLYPv0gH02twF&usg=AFQjCNEFpNtXkb_enyo66EFA4G_88z48DA
  [2]: http://mobify.com


## Answer 39567

- posted by: [Jontas](https://stackexchange.com/users/-1/11243-jontas) on 2012-06-01
- score: 1

(*note*: I understand your question as you want to make a mobile website, not apps for mobiles).

In order to reach your primary goal I would recomend that you build it as what is called responsive web (in short, one page with many layouts that you make fit different resolutions) so that you don't need to worry about device detection, only about resolution detection [that the browser will help you with].
This also means that you don't need to keep track of all new devices and will decrease the chances of not recognizing or miss recognizing devices.

At a previous job I had (mobile game developer/publisher) we had device detection and redirection of mobile devices (and also different pages for different devices), I can only say that I don't recommend it; Yes you have total control of ow each page will be displayed on each device but we spent a lot of extra time with keeping updates, new features etc looking good on all devices. Also a lot of time was spent on analyzing user agents and making sure we knew what device the user agent belonged to in order to show a correct page.
The possible downside I see is that if you are targeting "older" platforms such as pre android/iOs smart phones, dumb phones, pda's etc - then I don't know how well this will work as I recall that a few browsers on those sort of devices sometimes did things in there own way.

I would suggest that you don't do what we did - but instead either go for a solution where the same pages (and logic) is used for all visitors and it is only the layout [and possible what parts of the content] is changed based on the visitor device. From the two options you link to I would suggest mobify for this reason, they are speaking of one site for all visitors whereas wirenode more looks like one site per device.

To use a existing platform or make it yourself, that I think will depend on what your team know, have time for, how much "control" you want over the site and a few others things like that - so I won't wish to give more of a recommendation there than to speak to your team and to mobify and see where you wish to go.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
