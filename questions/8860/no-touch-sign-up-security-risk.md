## No-touch sign up security risk?

- posted by: [Rich](https://stackexchange.com/users/-1/1501-rich) on 2010-03-04
- tagged: `saas`, `security`
- score: 2

My SaaS startup is considering implementing a new sign-up procedure, but we're worried about security and false accounts.<br><br>
<strong>Current Method:</strong>
<ol>
<li>Prospect fills out free trial form</li>
<li>We get an email from the system with their information</li>
<li>We manually confirm it's a human (an actual email, etc</li>
<li>We manually create the account for them, and the system emails them a link</li>
</ol>
The problem is that there is a delay between sign up and use, which is definitley a leak in our funnel.<br><br>
<strong>Proposed New Method</strong>
<ol>
<li>Prospect fills out free trial form</li>
<li>The system automatically sends our a free trial link without our involvement</li>
</ol>
We get a lot of spam from our contact form and free trial form now.  Is there any increased risk of the new method vs. the old method?  Does anyone have experience transitioning from one to the other?<br>
P.S. [You can check out our existing homepage here.][1]<br>
Thanks!<br>
Rich


  [1]: http://www.sagepointsoftware.com


## Answer 8863

- posted by: [Oleg Kokorin](https://stackexchange.com/users/-1/968-oleg-kokorin) on 2010-03-04
- score: 3

How come a captcha and an email with activation link don't work anymore? I suggest these 2 things - they are a de-facto standard, used by virtually all major sites.


## Answer 8867

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-03-04
- score: 0

<p>I understand the desire to block auto signup spam, but what type of security risk are you concerned about that wouldn't be there already with a captcha solution?  Sure, the user isn't validated - but i don't believe that your solution would have the same problem as a forum looking to minimize viagra spam postings would.</p>

<p>There was a good conversation about this topic - <a href="http://answers.onstartups.com/questions/7972/captcha-vs-email-confirmation-vs-none/7975#7975" rel="nofollow">captcha vs email conversation vs none</a> which may be of use.  </p>

<p>Is there a way to allow people to experience the product without signing up? Then after entering in information they have to create an account to save it?  I don't know if this is a valid approach for your offering, but it does work with some companies - once you've entered in some info to see how it works, you are more compelled to create an account to save your work.</p>

<p>Once could incorporate some form robot anti-spam techniques like bad <a href="http://www.bad-behavior.ioerror.us/" rel="nofollow">behaviour</a> to minimize your exposure, then integrate a manual validation process via mechanical turk to keep the list scrubbed.  </p>



## Answer 8884

- posted by: [Justyn](https://stackexchange.com/users/-1/605-justyn) on 2010-03-05
- score: 0

You definitely need to automate this process. You should be able to find several libraries for using a confirmation email process to activate the account. This is very common, automated and pretty reliable. Captcha is another option that can be used in addition to the email confirmation.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
