## Captcha vs. Email confirmation vs. None

- posted by: [Chris](https://stackexchange.com/users/-1/412-chris) on 2010-02-11
- tagged: `website`
- score: 11

So we are a site that provides a free trial for our web-based service. We don't have any affiliate marketing that would pay based on leads or sign ups for the free trial. 

Right now we just require an email, password, security question and captcha to complete the registration. I know the simpler the sign up, the better the conversions. Someone recently told me each field added can often drop conversions by 3 - 4%. So I would love to simplify and the only place to simplify any further is the captcha.

What are the real pros and cons of Captcha vs. email confirmation vs. not doing either? What actual experiences have you had?

Thanks,



## Answer 7975

- posted by: [jimg](https://stackexchange.com/users/-1/2380-jimg) on 2010-02-11
- score: 15

<p><a href="http://stackoverflow.com/questions/1495032/do-we-really-need-email-confirmation/1495133" rel="nofollow">Stackoverflow</a> had an interesting conversation about this email confirmation &amp; captchas.</p>

<p>I think the jist of it can be summed up like this:</p>

<ul>
<li>captchas help protect against automated signups</li>
<li>email confirmation helps protect against impersonation</li>
</ul>

<p>I think though, the real question is - how to increase conversions. </p>

<p>Take a look at this article in a list apart that talks about <a href="http://www.alistapart.com/articles/signupforms" rel="nofollow">how signup forms must die</a>.  A bit harsh, but the core idea is to engage the prospect, capture as little info as possible, then automate the signup. </p>

<p>The fewer the fields the better - and the later in the process, the better.  </p>

<p>Here is another article - smashing magazine - about <a href="http://www.smashingmagazine.com/2008/07/08/web-form-design-patterns-sign-up-forms-part-2/" rel="nofollow">web form design best practices</a>.
(click to page 1 of the article - talks about the methodology and players)</p>

<p>To get to the specifics of your question, you could potentially simplify your signup to a single email field (password could be auto-generated, username could be added in profile) - if you believe that would make a difference. </p>

<p><strong>[edit]</strong></p>

<p>Some may say, jeesh, its just a simple field, why the bother?  Take a look at this article from user interface engineering entitled the <a href="http://www.uie.com/articles/three%5Fhund%5Fmillion%5Fbutton" rel="nofollow">$300 million button</a>.  Takeaway: people resist giving information away and abandon signups if presented at the wrong time.  Usability testing can confirm this - there are crowdsourced service providers (<a href="http://www.usertesting.com/faq.aspx" rel="nofollow">usertesting.com</a>, for example) that can provide valuable input for under $100 (i think $29 / user x 3).  </p>

<p>My favorite line from the article - usability reviewer: "I'm not here to enter into a relationship. I just want to buy something."</p>



## Answer 8000

- posted by: [Doug Martin](https://stackexchange.com/users/-1/2126-doug-martin) on 2010-02-12
- score: 4

I would really think about making your app have zero signup and just have a "try it instantly" button that auto creates an anonymous account tracked with a cookie.  On each page after that have a top of page div (like StackOverflow) that gives the user a reason and link to click through to create an account or click a survey about why they don't want to.  Remove all obstacles for users to try your app for themselves.


## Answer 7994

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2010-02-12
- score: 2

<p>+1 to jimg's answer, which I think is excellent.</p>

<blockquote>
  <p>So I would love to simplify and the only place to simplify any further is the captcha.</p>
</blockquote>

<p>How about removing that "security question" you have? IMHO these can often <em>reduce</em> security as the example of <a href="http://www.wired.com/threatlevel/2008/09/palin-e-mail-ha/" rel="nofollow">Sarah Palin's email hack</a> illustrates.</p>



## Answer 7980

- posted by: [Doug G](https://stackexchange.com/users/-1/2107-doug-g) on 2010-02-12
- score: 1

I would definitely try to simplify that sign-up page. Since it's a credit card free registration why even ask for verification on email or password, if they mess it up they can sign up again. Also the trend these days seems to be to make the 2 sign-up fields with a larger font. You could add a passive verification email with additional marketing material etc.

Best of Luck,
Doug


## Answer 8024

- posted by: [Jeff](https://stackexchange.com/users/-1/876-jeff) on 2010-02-13
- score: 1

Get rid of the the captcha and see what happens. If it doesn't cause a problem leave it off.


## Answer 8578

- posted by: [Gary Valan](https://stackexchange.com/users/-1/2650-gary-valan) on 2010-02-26
- score: 1

I'll add my perspective to the very good answers ahead of mine: For a "new" startup, if that can be a term, getting users/customers is paramount so a frictionless model of signing up is always a great idea. A colleague pointed me to sites like http://hunch.com/ and others including this one, where they don't require the user to sign up but over time it becomes addictive and people may be persuaded to sign up. If its interesting users will sign up over time. 

We're also added/ adding 3rd party sign up methods as well, such as FB connect and OpenID (still a mystery to a lot of people and poorly marketed). It may be useful to add Google, Yahoo, Twitter as well. In other words most people online already have one of these accounts so go where the people are.

As far as Captcha goes for a new startup, maybe hold off and just go in and delete the robot sign-ups till it becomes a nuisance and when the growth happens with a lot of activity on the site implement a good Captcha system. I say good because there are some that have images so obscure that it defeats vision challenged humans and the last thing you want is to aggravate the user base.

I hope I added something useful.


## Answer 41517

- posted by: [Ed Pichler](https://stackexchange.com/users/-1/6860-ed-pichler) on 2012-08-21
- score: 1

Without email confirmation any people can signup in a site with a email of other person. When that person would sign up the site too, the email will be already in use. The true email owner will need to ask to resend password.

An good way to avoid email confirmations is providing Opend Id And Facebook Connect log in.


## Answer 50574

- posted by: [Dmitri Zaitsev](https://stackexchange.com/users/-1/27575-dmitri-zaitsev) on 2013-08-24
- score: 0

Email confirmation varies. 
In the worst cases (still happens a lot) plain text password sent back to the user. 

In the best practice that is nowadays standard, all it takes is to open your email and click on the link. And if no email arrives, resent the confirmation. Can't be easier really. Even with the slowest possible internet connection. So why would one ever want to avoid it in first place? The benefits are obvious.

---

As for Captcha ... it gives some of the worst user experience. So use it with great caution at the risk of pissing off a lot of users. And don't forget users with disabilities. If Google gets away with lots of fed up users, it doesn't mean small startup will. Also the benefits are far less obvious.

If you are really worried about robot sign-ups, there are ways to deal with them programmatically. E.g. block or delay too frequent requests from the same IP address. Or anything else "suspicious" if it really causes problems. Or, if you are afraid to lose users, react with Captcha _when_ suspicious activity occurs.

---

More recently, another common technique of asking "security questions" became popular, but has been also received critics as not very effective and bad user experience.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
