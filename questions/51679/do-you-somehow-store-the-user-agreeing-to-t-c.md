## Do you somehow store the user agreeing to T&C?

- posted by: [iScotts](https://stackexchange.com/users/-1/10904-iscotts) on 2013-11-10
- tagged: `website`, `contract`, `terms-and-conditions`
- score: 0

<p>I am curious as to whether websites actually somehow store the agreement a user makes when clicking through the terms and conditions. This way there is no way they could deny agreeing right, should something go wrong? I want to implement this into my site but I want to do it the right way, so I am asking once again, when a visitor clicks on the "agree" button is this being recorded somewhere or do you just redirect them to a new page? </p>

<p>I feel this way would be good for both me and my visitors because this way should I change the terms and conditions without letting the visitor know it will show which they agreed to etc. I am just basically doing this to gain trust from my visitors as a reputable company. </p>



## Answer 51706

- posted by: [Ryan Doom](https://stackexchange.com/users/-1/5655-ryan-doom) on 2013-11-13
- score: 1

<p>I typically do store this.</p>

<p>One thing to consider is that terms sometimes change. </p>

<p>We typically implement a system part of the account creation and login process that checks what terms of service / when the user agreed to it and if they haven't agreed to any or the latest it prompts it up for them to accept before proceeding.</p>

<p>This is then saved with the users id, date they agreed, and what TOS they agreed to.  We also typically log the IP address.</p>



## Answer 51681

- posted by: [bhttoan](https://stackexchange.com/users/-1/23673-bhttoan) on 2013-11-10
- score: 0

<p>You could easily store their click in a database, for example, with their username or some other way of identifying them - if you want general surfers to do this then you may struggle as there is no way of proving that any individual did agree even if you were to track IP addresses etc</p>

<p>On the other hand, if you are referencing users as in those who signup/login then you can use their username along with IP address maybe plus date &amp; time - in our B2B app we have a tick box which says "I agree to Terms and Conditions" with a link to our terms and conditions and user cannot sign up without agreeing. Whether the actually read them or not remains to be seen but you can only lead a horse to water.....</p>



## Answer 51691

- posted by: [Max](https://stackexchange.com/users/-1/16514-max) on 2013-11-11
- score: 0

<p>You can simply build the functionality of showing an error each time a user is not agreeing with the terms. </p>

<p>If a user is in a members-only section, it means that the user already agreed with the terms.</p>

<p>Then you'll note a version for your Terms and Conditions agreement and the date when the user registered. Your agreement can have revisions (e.g. git) and you can match exactly which agreement a user agreed on based on its registration date.</p>

<p>In general you should notify users of any T&amp;C updates either by a simple notification or having a checkbox to agree to the new terms to continue using your website.</p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
