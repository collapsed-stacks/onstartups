## What email address convention does your SaaS startup use?

- posted by: [Kosta Kontos](https://stackexchange.com/users/-1/16592-kosta-kontos) on 2012-02-23
- tagged: `saas`, `strategy`, `email`
- score: 1

We run a small SaaS startup and we're using GMail for Business. Each member of staff currently has a personal email address using their first name. For example john@example.com, steve@example.com...

We also have Gmail groups: admin@example.com (this receives daily reports on the health of our system and is also used as a user account for our staff to log into our own systems), support@example.com (customer queries / complaints all come here), and info@example.com (this is what we advertise on marketing material including our website).

Emails sent to these GMail groups get distributed to the list of people in that group. For example emails sent to info@example.com get sent to both john@example.com and steve@example.com, but emails sent to admin@example.com only get sent to Steve.

Now we're considering dropping the groups / distribution lists altogether, and instead creating individual accounts for each function. In other words we'd have an account for support@example.com where all support emails can be archived, and then dedicated support staff can simply log into this GMail account.

Which of the above two strategies is better - distribution lists (current strategy) or individual accounts that are shared? Is the first name convention a bad idea for personal email addresses? And lastly what email address convention should we use for our billing / accounts. I currently send out invoices once a quarter from my personal email address, and I always add a personalised message for each client.

Cheers from Cape Town!


## Answer 36496

- posted by: [Jesper Mortensen](https://stackexchange.com/users/-1/1261-jesper-mortensen) on 2012-02-23
- score: 1

For the personal email adresses, I see `firstname@company.com` used quite a lot by startups. For  mature companies the form `firstname.lastname@company.com` is more common.

Between the two formats, I think it's a matter of taste and to some extent which signals you want to send between "approachable" vs "mature company". The only objective difference is that `firstname.lastname@company.com` is more scalable, i.e. you can grow to more people before you get a collision where two employees share the same name.

I think you are doing the right thing by using GMail distribution lists for `admin@company.com` et cetera. Switching over to shared accounts would be going backwards -- how about password security for the shared account, and how will you see who has answered to a specific mail?

> send out invoices [...] from my personal email address

That's fine, maybe getting a personalized email makes it more humane, and gets you your money faster... All right, the chances for that are slim. The main thing about such 'automated' emails is that they should come from an address *that can be replied to.*


## Answer 36500

- posted by: [Nick Stevens](https://stackexchange.com/users/-1/15902-nick-stevens) on 2012-02-23
- score: 1

Regarding distribution lists vs dedicated accounts, there is no right answer:

 - The good thing about distribution lists, is that all the people who should get the email, do.
 - The bad thing about distribution lists, is that many people end up reading the same email, whether they need to or not.

 - The good thing about dedicated accounts, is that only the people who actively check the account see the emails.
 - The bad thing about dedicated accounts, is that if no-one actively checks the account, no-one reads the emails.

Go with whichever system your team is most likely to get most value from.  Alternatively, instead of relying on email, see what alternative options there are. Perhaps a nice big dashboard screen in the office that displays the system health, for example.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
