## What information to gather when registering users

- posted by: [user3462](https://stackexchange.com/users/-1/3462-user3462) on 2011-01-17
- tagged: `saas`, `registration`, `user-interface`
- score: 1

We all know that it's really important for an impatient SaaS user to not make them spend too much time filling forms. Having said that there maybe some important fields that needs to be gathered during the registration process for future reporting purposes.

Currently, the registration form I have only asks for:

 1. Email Address
 2. Password
 3. Confirm Password

Should I be collecting info such as:

1. First Name
2. Last Name
3. Gender
4. Country?


## Answer 19055

- posted by: [Mat Banik](https://stackexchange.com/users/-1/6605-mat-banik) on 2011-01-17
- score: 1

I would say you should at least get First name or Nick name to make your communication to the user more personable. You can always collect the rest in stages, when customer will want something from you like free calculation or PDF doc or what ever.

Also now day I would suggest integrating facebook connect. It doesn't get any lazier for the user than that and you can get all the personal info they have in facebook.


## Answer 19079

- posted by: [Mike](https://stackexchange.com/users/-1/3475-mike) on 2011-01-17
- score: 1

Every additional piece of information you ask for will reduce the sign up rate. 

Therefore you really need to ask yourself how valuable each piece of information is to you.

 - A First/Last Name enables you to personalize emails and improve their deliverabiliy, so is probably worth it if you expect to email people.

 - Gender isn't relevant unless you are running a dating service.

 - Country you could infer from the IP address. So unless you need to bar exports to certain countries, it is better not asked directly.

 - Age / Income questions will definitely frighten a lot of people off.

Note that facebook connect apparently requires the user to authorize which information should be passed to your website. So it is useful as an authentication mechanism  but unless people have a reason to tell you the name of their favorite pet and music group, don't ask.





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
