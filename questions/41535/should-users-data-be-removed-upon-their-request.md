## Should users data be removed upon their request?

- posted by: [Dave Valentine](https://stackexchange.com/users/-1/19360-dave-valentine) on 2012-08-22
- tagged: `legal`, `customer-support`, `users`
- score: 10

I have a commercial web startup. From a legal standpoint does maintaining users record (database info) if they decide to delete their account outweighs  deleting their record?

- Maintaining the users record, even if they delete their account, can protect users and myself, from legal issues by having solid evidence.

But

- Deleting a account, can save some server space and prevent users from claiming that there is a privacy/respect issue.

What can be done to prevent users discomfort and always have a legal backup?
 




## Answer 41540

- posted by: [Joel Friedlaender](https://stackexchange.com/users/-1/5543-joel-friedlaender) on 2012-08-22
- score: 3

I don't think it's really viable to delete their information.  Even if you remove it from your application, you aren't going to go back to every back up that contains them and remove them from those as well.  With that in mind, claiming you have deleted them would be somewhat dishonest.

You can delete them from your database if you like (it is probably a good idea to help limit database growth), but don't claim in your terms that you delete all their data.


## Answer 41549

- posted by: [DJClayworth](https://stackexchange.com/users/-1/12762-djclayworth) on 2012-08-22
- score: 3

<p><strong>You should be very aware of the rules on data retention and data privacy for the legal jurisdiction(s) you operate in.</strong> Some places will give you a lot of legal trouble if you retain the information of a user who has 'deleted' their account. </p>

<p>For example the Privacy Commisioner of Canada conducted <a href="http://www.priv.gc.ca/cf-dc/2009/2009_008_0716_e.pdf" rel="nofollow">an investigation into Facebook</a> and found them to be in contravention of the <em>Personal
Information Protection and Electronic Documents Act</em>. She was able to effectively compel them to remove both deactivated and deleted accounts completely from their databases after a reasonable time or face penalties under the act. From the investigation: "The Act is clear that organizations must retain personal information only for as
long as necessary to fulfil the organization’s purposes, that organizations
should develop guidelines and implement procedures with respect to the
retention of personal information, and that such guidelines should include
minimum and maximum retention periods." A similar investigation in the UK led to similar results.</p>



## Answer 41546

- posted by: [JeffO](https://stackexchange.com/users/-1/1796-jeffo) on 2012-08-22
- score: 1

Be very clear in your cancellation policy. There are situations where a temporary 'soft' delete might be appreciated: accidents happen, accounts get compromised, disgruntled employees act maliciously. It would benefit you if an owner could verify themselves and have their account and data restored. You could keep it for 30 days. It could also be a great excuse to send a former client and email telling them their time is up, but if they would like to return as a customer, you have their data.

You are taking a risk when you manage client's data and there is little reward from former clients. Be dilligent and as Joel recommends, don't forget about the backups. Clients need to know they exist, how long you intend on keeping them, and that they are in a secured location.


## Answer 41539

- posted by: [Steve Jones](https://stackexchange.com/users/-1/12985-steve-jones) on 2012-08-22
- score: 0

In general, not much is deleted these days, as storage is so cheap. However, if you are concerned about server space, why not just archive the "deleted" data to an offline store?

Perhaps you should mention your data-retention policy in your terms, so that people know what will happen. If you are silent on the matter, the rules will depend upon your jurisdiction. Furthermore, in some jurisdictions, whatever you have in your terms is over-ruled by local regulations.

For example, it used to be required to delete telecoms call records within 12 months in Germany, while the UK allowed you to keep them.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
