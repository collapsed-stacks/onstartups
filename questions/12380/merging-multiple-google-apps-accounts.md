## Merging multiple google apps accounts

- posted by: [Shabda](https://stackexchange.com/users/-1/2973-shabda) on 2010-06-25
- tagged: `google`, `google-apps`
- score: 4

We have a few Google apps accounts at

domain1.com
domain2.com
domain3.com

Now I want to merge all them together. (All users at all domains are same).

However there is a 5 days waiting period between deleting one domain and when you can add it to other apps account, this is not possible for us as all are active.

Is there a way to resolve this problem.

(Also please tag it as google-apps, as I cant do this myself).



## Answer 12382

- posted by: [Branko](https://stackexchange.com/users/-1/670-branko) on 2010-06-25
- score: 2

We had the same problem. Based on the feedback we got during the beta test of our software we decided to use a different name for the final release. With the product name change we changed also the domain we use for the product. We wanted to merge the accounts for both domains, but later changed our mind due to the annoying waiting period. At the moment we have Google Apps  active for both domains, but actually use only the accounts on the new domain.

We downloaded documents from the old domain to our computers and then uploaded them to the new domain.  

For e-mail we configured forwarding from accounts in the old domain to accounts in the new domain. On the new domain we created filters that put a label on the messages that was originally sent to the old domain.

If you really need to close one domain and add it as an alias to another I would suggest you to use some temporary mail server. Change the MX records for the old domain to point to the temporary mail server. You can than close your Google Apps for the old domain and after 5 days add it as an alias to the new domain. When this is active you can point MX records back to Google servers again. During those 5 days you can use the temporary mail server to read your mail or even configure it to forward it to the Google Apps accounts in the new domain.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
